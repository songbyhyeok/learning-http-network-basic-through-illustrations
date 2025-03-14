# 10장 HTML
## 10.1 HTML 
웹페이지는 대부분 HTML로 되어있다.

hyper text는 서로 링크되어있는 문서임.

팀 버너스리가 모자이크 브라우저를 개발해서, 해당 브라우저가 해석할 수 있는 HTML 사양을 정리한 것이 HTML 1.0이 되었다.

```http request
HTML 1.0 (1993년)
최초의 HTML 버전
기본적인 텍스트 구조와 링크만 지원

HTML 2.0 (1995년)
HTML 표준화의 시작
폼(form)과 이미지(img) 태그 추가

HTML 3.2 (1997년)
CSS 지원 시작
<table>, <iframe>, <script> 태그 추가
플러그인(예: Java Applet) 지원

HTML 4.01 (1999년)
HTML 문서 유형(Strict, Transitional, Frameset) 도입
접근성과 국제화 개선
<div>, <span>, <abbr>, <acronym> 같은 태그 추가
JavaScript와 DOM의 활용 증가

XHTML 1.0 (2000년)
HTML을 XML 형식으로 변환한 버전
더 엄격한 문법 요구(태그 소문자 사용, 태그 닫기 필수 등)

XHTML 1.1 (2001년)
더욱 엄격한 문법 적용 (프레임셋 제거)

HTML5 (2014년 - 현재)
가장 큰 변화 중 하나
<video>, <audio>, <canvas> 등 멀티미디어 태그 추가
<article>, <section>, <nav>, <header>, <footer> 등 시맨틱 태그 추가
JavaScript API 확장 (예: WebRTC, WebSocket, LocalStorage)
플래시(Flash) 사용 감소, 모바일 웹 지원 강화
```

## 10.1.2 CSS
HTML 디자인 관련 요소

## 10.2.1 다이나믹 HTML
정적 HTML을 클라이언트 사이드 스크립트를 사용해서 동적으로 변경하는 기술임.

동적으로 바꾸고 싶은 HTML요소를 지정하기 위해서 DOM이라는 구조를 사용함.

## 10.2.2 DOM
HTML, XML 문서를 위한 API임.

```http request
DOM API는 브라우저가 자체적으로 구현한 엔진 덕분에 우리가 사용할 수 있는 거야. 🚀
브라우저마다 DOM API를 직접 구현하고, 이걸 통해 JavaScript 코드에서 HTML 요소를 조작할 수 있어.

각 브라우저가 자체적으로 DOM API를 구현

크롬(Chrome) → V8 엔진 + Blink 렌더링 엔진
파이어폭스(Firefox) → SpiderMonkey 엔진 + Gecko 렌더링 엔진
사파리(Safari) → JavaScriptCore 엔진 + WebKit 렌더링 엔진
엣지(Edge) → V8 엔진 + Blink 렌더링 엔진 (크로미움 기반)
👉 같은 DOM API(document.querySelector, element.innerHTML)라도 브라우저마다 내부 구현 방식이 다를 수 있어.
```
dom tree(바이트 -> 문자 -> 토큰 -> 노드 -> dom)
cssom tree
render tree
레이아웃 리플로우(요소의 크기, 좌표정보 설정) - 렌더트리 계산하기, 배치
페인트 리페인트 - 렌더트리 그리기
composite(레이어들을 합성해서 pixel로 표현함.)

## 10.3 웹 애플리케이션
xml, rss, atom... 
json
