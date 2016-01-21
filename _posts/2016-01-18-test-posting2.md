---
layout: post
title: "MARKDOWN Exercise"
description: ""
tags: [MARKDOWN]
published: false
---
{% include JB/setup %}

이것은 문장입니다. **엔터는 엔터**입니다. 강조 부분을 눈에 띄게 만들려면, 구문 강조용 스타일시트를 추가해야 합니다. 참고해볼만한 스타일시트로는 `syntax.css` 가 있습니다. 이 스타일은 GitHub 에서 사용하는 것과 동일하며 당신의 사이트에도 자유롭게 사용할 수 있습니다. linenos 를 사용하는 경우에는, syntax.css 에 .lineno 라는 CSS 클래스 선언을 추가해서 줄 번호와 구문 강조된 코드를 구분할 수 있습니다

> 굉장히 쉽고 직관적입니다. 좋군요. `_config.yml` `aaa.html`
>
> 이것은 인용이라고 합니다.

- list1
- list2
- list3

1. Item 1
  1. A corollary to the above item.
  2. Yet another point to consider.
2. Item 2
  * A corollary that does not need to be ordered.
    * This is indented four spaces, because it's two spaces further than the item above.
    * You might want to consider making a new list.
3. Item 3

![테스트 이미지](http://placehold.it/350x150)

# title1

## title2


**title3**

[LINK](https://github.com/mojombo/jekyll/wiki/YAML-Front-Matter)

{% highlight html linenos %}
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Document</title>
<style>
	.a { margin: 0; }
</style>
<script>
	var aaa = function(){
		if(){

		}
	}
</script>
</head>
<body>

</body>
</html>
{% endhighlight %}

