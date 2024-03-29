---
title: "[Etc] Javascript"

categories:
  - Etc
tags:
  - [Etc, 자바스크립트]

permalink: /etc/Javascript/


date: 2023-09-16
#last_modified_at: 2022-07-24
---
<br><br>
리팩토링에 관심이 생기며, 리팩토링(마틴 파울러) 1판 / 2판을 읽어보려 한다.<br><br>
리팩토링(마틴 파울러) 1판 / 2판은 출간한지 좀 되었지만 리팩토링의 기본서라 불릴만큼 유명한 책이다.<br><br>
1판의 경우 예제를 Java로 작성하였고, 2판의 경우 JavaScript로 작성했다는 점이 가장 큰 차이점이다.<br><br>
2판이 JavaScript로 작성된 이유는 대세 언어이기 때문이며, 이 대세 언어에 대해 자세히 공부해보려고 한다.

<br><br><br><br>
## <span class="color">Javascript 란?</span>
Javascript는 <code>웹 브라우저에서 동작하는 유일한 프로그래밍 언어</code>로, 현재는 서버 사이드, 모바일 앱 개발 등 다양한 분야에서 활용되고 있다.<br><br>
- <code>초보자 친화적</code> : 자바스크립트는 배우기 쉬운 언어 중 하나이며, 개발자 커뮤니티도 매우 활성화되어 있어, 새로운 개발자들이 접근하기 좋은 언어다.
- <code>빠른 반복과 테스트</code> : 빠르게 프로토타이핑과 테스트를 할 수 있게 해주는 동적 언어의 특징을 가지고 있다.
- <code>동적 타이핑</code> : 변수의 타입을 미리 선언할 필요가 없으며, 런타임에 타입이 결정된다.
- <code>객체 지향 및 함수형 프로그래밍 지원</code> : 자바스크립트는 프로토타입 기반의 객체 지향 프로그래밍을 지원하며, 일급 함수의 개념을 지원함으로써 함수형 프로그래밍 패러다임도 지원한다.
- <code>비동기 프로그래밍 지원</code> : I/O 작업이나 네트워크 요청 등을 비동기로 처리할 수 있으며, Promise나 async/await와 같은 모던 기능들도 지원한다.
<br><br><br><br>

## <span class="color">Javascript의 프레임워크</span>
<br>

### 1. Vue.js
: Vue.js는 구글의 엔지니어 Evan You에 의해 개발되었으며, 2014년 2월에 공식적으로 배포되었다. <br>
  대표적인 사용기업은 나사, 어도비, 깃랩, 페이스북, 넷플릭스, 샤오미, 알리바바 등이 있다.<br><br>

- Vue.js는 다른 프레임워크와는 달리 선택적으로 채택하여 사용할 수 있다. 따라서 다른 라이브러리나 기존 프로젝트에 적용하는 것이 비교적 수월하다.
- 개발한 프론트엔드 파일을 사용자가 볼 수 있도록 브라우저 화면에 렌더링하는 과정에 템플릿이란 문법을 사용하는데, 이때 이 템플릿을 구성하는 문법이 HTML 기반으로 이루어져 있어 초보 개발자도 빠른 시간 안에 기본적인 사용이 가능할 정도로 쉽다.
- Angular에서 핵심적인 요소들이 가진 장점을 기반으로 가볍게 제작한 프레임워크로, 작은 규모의 어플리케이션의 개발시 용이하며 속도 측면에서 큰 장점을 보인다. 
- 단일 파일 컴포넌트 기반를 기반으로 하여, HTML, CSS, JavaScript 코드를 .vue 확장자를 가진 하나의 파일에 모두 정의한다. 이러한 관리 방식은 적당한 규모의 프로젝트에서 관리의 생산성을 높이고, 협업을 수월하게 한다는 장점이 있다.

<br><br><br><br>

### 2. React
:  React는 페이스북의 엔지니어 Jordan Walke에 의해 개발 되었으며, 2011년에 페이스북 뉴스피드에 처음으로 적용되었다. 대표적인 사용 기업은 페이스북, 넷플릭스, 우버, 페이팔, 에어비앤비, 마이크로 소프트 등이 있다. 싱글페이지 어플리케이션, 모바일 어플리케이션 개발시 많이 활용되며 데이터 변경에 따라 특정 컴포넌트만 효율적으로 갱신하고 렌더링한다는 특징이 있다.<br><br>

- 거대한 사용자 커뮤니티가 있다. 페이스북의 지원을 받는 만큼 지속적인 버전 관리 및 오류 수정이 이루어지고, 사용자가 많아 다양한 레퍼런스, 확장 라이브러리가 많다.
- 템플릿 방식으로 프레임워크를 관리하는 Vue와는 달리, React는 <code>JSX 코드</code>로 컴포넌트를 작성하고 컴포넌트의 상태를 변화시키지 않고 관리한다. 따라서 템플릿은 재구조화가 어렵고, 에러에 취약한 반면, React는 상태를 고유 속성대로 유지하기 때문에 대규모 프로젝트에서도 관리가 수월하고 테스트에도 적합하다.
- 코어 기능 외의 편의 기능을 제공하지 않기 때문에, 타 프레임워크에 비해 독립적으로 사용이 가능하다. 더불어 이미 서비스 배포 중인 어플리케이션에도 점진적으로 채택할 수 있다.
<br><br><br><br>

### 3. Node.js
: 일반적으로 자바스크립트는 브라우저에서 실행되어 웹 페이지의 스크립트 언어로 주로 사용된다. 그러나 <u>노드.js를 통해 자바스크립트를 서버 측 언어로도 사용</u>할 수 있게 되었다.<br><br>

- <code>비동기 I/O 처리</code> : 비동기 I/O 처리를 제공하여, I/O 작업이 수행되는 동안 다른 작업을 동시에 진행할 수 있다.
- <code>이벤트 드리븐</code> : 이벤트 루프를 통한 이벤트 드리븐 프로그래밍 모델을 사용한다. 이러한 방식은 높은 성능과 확장성을 제공한다.
- <code>NPM(Node Package Manager)</code> : 노드.js에는 npm이라는 강력한 패키지 관리 시스템이 내장되어 있어, 다양한 라이브러리와 도구를 쉽게 설치하고 관리할 수 있다.
- <code>크로스 플랫폼</code> : 다양한 플랫폼(Windows, Linux, macOS 등)에서 작동하며, 코드의 이식성이 좋다.
- <code>모듈러 프로그래밍</code> : 모듈러 프로그래밍을 지원하여 코드의 재사용성과 유지 보수성을 향상시킨다. 
<br><br><br><br>

---
참고링크 | <br>
- [[도서 리뷰] 리팩터링 2판](https://blog.soobinpark.com/202)
- [[IT 기본 지식] JS 프레임워크란?](https://www.icia.co.kr/community/board/view/2/1/84)
<br><br><br>
