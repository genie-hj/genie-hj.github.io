---
layout: post
title: "Prologue"
summary: Front-end development
tagline: "Supporting tagline"
tags : [front-end]
---
{% include JB/setup %}
<!--
#과거의 이야기
웹퍼블리셔 *(좋아하는 이름은 아니지만..)* 라고 불리며 해왔던 것들.

- 단지 PSD->browser 변환과 개발을 붙일 뼈대에 불과 했었던 굴욕의 **Table layout coding**
*조금만 잘 못 건들여도 와르르 무너지기 쉽상이었고 숙련되면 영혼없이 기계적인 코딩이 가능. 그 와중에 HTML4.0 Reference 책을 너덜거리도록 봤던 듯. 어느 누구도 중요하게 생각지 않아서 슬펐던 시절.*
- 브라우저 시장의 폭풍 전쟁 속에 등장한 **웹 표준**
- 장애인 차별금지법 으로 급물살을 탄 **웹 접근성**
- UI 동작을 위한 Javascript, JQuery...
-

>포토샵 파일, 이미지, 와이어프레임 등을 가지고 웹 페이지를 만드는 일
>때로는 앞서 나온 포토샵 파일, 이미지, 와이어프레임을 그리는 일
>웹 페이지에 애니메이션을 만들고 트랜지션 효과를 주기 위해 자바스크립트를 작성하는 것
>콘텐츠를 정의하고 이를 꾸미는 HTML과 CSS를 작성하는 것
 -->

[참고문서]
[Why can't we find Front End developers?](http://www.slant.co/topics/1488/~front-end-package-managers)
[[번역] 프론트엔드 개발자는 왜 구하기 어렵나요?](https://taegon.kim/archives/4810)


##대부분의 사람들이 생각하는 프론트엔드 엔지니어링

- 포토샵 파일, 이미지, 와이어프레임 등을 가지고 웹 페이지를 만드는 일
- 때로는 앞서 나온 포토샵 파일, 이미지, 와이어프레임을 그리는 일
- 웹 페이지에 애니메이션을 만들고 트랜지션 효과를 주기 위해 자바스크립트를 작성하는 것
- 콘텐츠를 정의하고 이를 꾸미는 HTML과 CSS를 작성하는 것

##프론트엔드 개발자가 실제로 하는 일

- 디자이너와 엔지니어 간의 시각적 언어 확립
- 시각 디자인으로부터 콘텐츠, 브랜드, 기능 등을 표현할 컴포넌트 세트 정의.
- 컨벤션, 프레임워크, 요구 사항, 시각적 언어, 스펙 면에서 웹 애플리케이션의 기준 확립
- 웹 애플리케이션의 범위를 기기, 브라우저, 화면, 애니메이션의 측면에서 정의
- 브랜드 충성도, 코드 품질, 관계자의 상품 리뷰를 위한 품질 보증 가이드라인 개발
- 적절한 간격, 타이포그래피, 헤딩, 글꼴, 아이콘, 여백, 그리드 등을 사용해 웹 애플리케이션 꾸미기
- 디자인 가이드라인을 따르며 다양한 해상도에 대응하는 이미지, 디바이스별 목업 등을 사용해 웹 애플리케이션 꾸미기
- 시맨틱, 접근성, 검색엔진 최적화, 스키마, 마이크로포맷 등을 고려하여 웹 애플리케이션 마크업하기
- API에 접근하여 사용하기 편하고 배터리 소모가 없는 디바이스 및 클라이언트가 인지하는 방식으로 정보를 가져오기
- 부드러운 애니메이션, 트랜지션, 게으른 로딩lazy loading, 인터랙션, 애플리케이션 워크플로우를 수행하는 클라이언트 사이드 코드 개발. 대부분 점진적 기능 향상 및 하위 표준 호환성까지 고려.
- CORS(Cross Origin Resource Sharing)을 고려하는 한편 XSS(Cross Site Scripting)와 CSRF(Cross Site Request Forgery) 공격을 막아낼 수 있도록 백엔드 접속에 대한 안전성 확보
- 엄격한 데드라인, 관계자들의 요구, 기기별 제한에도 불구하고 항상 사용자가 최우선이라는 점을 잊지 않는 것
- 이러한 목표를 달성하기 위해 프론트엔드 엔지니어들은 시각 디자인 도구(포토샵, Adobe, Macaw, Sketch)부터 프로그래밍 도구(IDE, Command Line, Source Version Control, Bash 스크립트, 빌드
태스크)까지 다양한 도구를 사용한다. 심지어 간혹 마케팅(뉴스레터, 캠페인, 분석, 검색엔진최적화, 소셜미디어), UX(애니메이션, 트랜지션, 피드백, 인터페이스, 시각적 언어)부터 콘텐츠 수정(구획점, 단어가 뚝 떨어지지 않게 하는 일, 가독성, 색상)까지 신경써야 한다.


##숙련된 프론트엔드 엔지니어가 알아야 하거나 작업시 해야할 일 (힌트: 바로 여러분이 고용하고 싶은 사람이다)

- DNS Resolution, CDNContent Delivery Networks 사용, 여러 호스트 이름을 통한 리소스 요청 성능 향상
- HTTP 헤더 (Expires, Cache-Control, If-Modified-Since)
- 스티브 사우더스의 규칙 전부 (고성능 웹사이트)
- PageSpeed, YSlow, 크롬 개발자 도구 Audit, 크롬 개발자 도구 Timeline에서 보여주는 문제를 해결하는 법
- 작업을 서버에서 해야할 때와 클라이언트에서 해야할 때 구분
- 캐시, 프리 페칭pre-fetching 및 지연 로드 기법
- 네이티브 자바스크립트. 직접 바닥부터 코드를 작성해야 할 때 혹은 다른 사람의 코드를 가져다 써야 할 때를 아는 것. 그리고 두 작업의 장점과 단점을 평가할 수 있는 능력
- 최신 MVC 자바스크립트 라이브러리(예. AngularJS, EmberJS, ReactJS), 그래픽 라이브러리(예. D3, SnapSVG), DOM 관련 라이브러리(예. jQuery, Zepto), 게으른 로딩 또는 패키지 관리 라이브러리(예. RequireJS, CommonJS), 태스크 관리자(예. Grunt, Gulp), 패키지 관리자(예. Bower, Componentjs), 테스팅(예. Protractor, Selenium)에 대한 지식과 사용.
- 이미지 포맷과 장점. 언제 무엇을 어떻게 써야 하는가에 대한 지식. 이미지 최적화 기법과 사용 계획 (스프라이트, 게으른 로딩 기법, 캐시 비움, 인터레이스드 PNG)
- CSS 표준, 최신 컨벤션과 기법(예. BEM, SMACSS, OOCSS)에 대한 지식과 사용
- 자바스크립트의 컴퓨터 과학(메모리 관리, 싱글 스레드 특성, 가비지 컬렉터 알고리듬, 타임아웃, 스코핑, 호이스팅, 패턴)

Package Managers
Preprocessors
Task Based Build Tools

RequireJS
BEM
Grunt.js
Gulp.js
React.js

----------------------

1. 버전관리시스템
- GIT
- mercurial
- subversion


2. 통합개발환경
- eclipse
- sublime
- wenstorm
- aptana


3. Scaffolding
- Grunt-init


4. 모듈 관리 도구 ( Package managers )
- npm (node package manager)
- Bower


5. CSS 전처리기
- less
- sass


6. 코드 품질 검증 도구
- JS Lint
- JS Hint
- ESLint


7. 테스트 프레임워크 & 테스트 더블
- QUnit
- Jasmine
- Sinon.JS


8. 테스트 러너
- Karma


9. 압축, 난독화
- UglifyJS


10. 문서화 & 애너테이션
- yui
- jsDoc3


11. Task runners & Build system
- Gulp
- Grunt

- JS 최적화 (Min & Uglify)
JS 코드 품질 검증 (JS Lint, flow)
JS 테스트 수행 (test code run with browser)
JS Code Templating
CSS 최적화 (Min)
CSS Image sprite 자동화
HTML, CSS 리소스를 js로 변환 (tmpl[‘index.html’] = ‘<html>n<body></body></html>’;)
ALL FILE CONCAT to THE_ONE.js
BUILD 태스크를 수행 하면 3초만에 우리가 원하는, result.min.js 산출물 파일 생성



12. 지속적인 통합
- Jenkins
- Travis


13. 웹사이트 측정
- YSlow
- PageSpeed


14. 브라우저 테스트
- Browser-Sync (무료)
	- Task runner (grunt/gulp)를 통해 쉽게 run
	- weinre 자동 세팅 (Remote Debugging)
	- Click & Scroll position & Form action 동기화
	- 자동 화면 갱신 (리소스/코드 변경시)
- VM 환경세팅 (무료)
	- modern.ie : IE test VM
	- Genymotion : Android VM
	- Xcode : ios VM (Simulator)

- Browser Stack (유료)
	- 웹 베이스 가상 머신 테스트 (설치x)
- SauceLabs (유료)


15. 성능 최적화
- 조금 그리고 (draw) , 조금 연산하기
- Repaint / Reflow 최소화
- 리소스 로컬 캐싱 활용 (Local Storage)
- UI 인터페이스 응답성 최대한 보장
- 빌드를 이용한 파일 크기 최적화



----------------------------------------

##TO-BE
- JS 파일 안에 있던 리소스 분리
- 유틸리티 함수 추출
- 기능 단위 파일 분리
- gulp를 이용한 빌드 환경 세팅

