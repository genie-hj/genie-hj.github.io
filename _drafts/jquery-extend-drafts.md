---
layout: post
title: JQuery Plugin 개발 - $.extend() / $.fn.extend()
summary: JQuery 사용자 정의 함수를 알아 보자.
tagline: "Supporting tagline"
tags : [JQuery, Javascript, IIFE]
---
{% include JB/setup %}

> ###extend [ɪk|stend]  
>1. 더 길게[크게/넓게] 만들다  
>2. 연장하다  
>3. (사업,영향력 등을) 확대[확장]하다

JQuery Plugin 개발에 주로 사용되는 `$.extend()` `$.fn.extend`.  
사전적 의미 그대로 확장의 뜻이지만 둘의 쓰임은 조금 다르다. JQuery Plugin 개발 과정을 통해 정리 해보자.

#준비
- JQuery 라이브러리를 기반으로 제작함에 있어 우리의 `$`기호를 걱정없이 사용하고 싶으므로 [즉시호출함수 표현식 *(IIFE-Immediately Invoked Function Expression)*]()으로 `$`를 플러그인 내부 지역함수로 정의 한다. 다른 라이브러리와의 충돌 방지와 가독성 유지를 위함이다.

{% highlight html linenos %}
<script>

(function($){
	//플러그인 코드
})(jQuery);

//혹은

!function($){
	//플러그인 코드
}(jQuery);

</script>
{% endhighlight %}


- JQuery에는 전역 함수로 사용되어 지는 자체 기능들이 있다. (JQuery 전역함수는 JQuery 객체의 메소드 이자, JQuery [네임스페이스(Namespace)]()의 함수.) [유틸리티 메소드*(utility method)*](http://api.jquery.com/category/utilities/)로 제공 되는 이 녀석은 `$.each()` `$.map()` `$.merge()` `$.ajax()` 등등이 있다. 이 녀석들 처럼 사용할 수 있는 나만의 사용자 정의 유틸리티 메소드를 만들어 보자. 이것이 플러그인 개발의 시작이다.


{% highlight html linenos %}
<script>

!function($){
	
	$.sum = function(array) {

		var total = 0; // 초기화

		$.each(array, function( idx, value ) { // 배열을 인자로 받아온다
			value = $.trim( value ); // string의 공백 제거
			value = parseFloat( value ) || 0; // nember 인지 아닌지 판단, false 일 경우 0을 반환
			total += value; // value를 덧셈한다.
		});

		return total;
	}

	var result = $.sum( [20, 30, 15, 45, 'abc'] );
	console.log( result ); // 110


}(jQuery);

</script>
{% endhighlight %}

- 위 예제는 `$.sum` 유틸리티 메소드로 배열을 전달 받아 그 배열의 합을 반환하는 코드이다.  
유틸리티 메소드가 어떤 녀석인지 이해 되었다면, 좀 더 유연하게 옵션 값을 재정의 하여 사용할 수 있는 플러그인 제작을 시작해 보자. 옵션 값을 지정 하기 위해 `$.extend` 유틸리티 메소드를 많이 사용한다.


#$.extend()
둘 이상의 객체(Object)가 존재 할때, 첫번째 객체에 나머지 객체를 병합(Merge) 하는데 사용한다.
*Merge the contents of two or more objects together into the first object.*
`$.extend`는 객체를 인자로 넘긴다. 가장 마지막에 있는 객체 부터 차례로 앞으로 병합, 확장 하여 첫번째 객체에 그 결과 값을 반환한다. 병합되는 방식을 주의 깊게 보자.

{% highlight html linenos %}
{% endhighlight %}



http://e-rooms.tistory.com/entry/jQuery%EB%A5%BC-%EC%9D%B4%EC%9A%A9%ED%95%9C-%ED%94%8C%EB%9F%AC%EA%B7%B8%EC%9D%B8-%EA%B0%9C%EB%B0%9C-%EB%B0%8F-extend

