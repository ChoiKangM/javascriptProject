# javascriptProject
자바스크립트 프로젝트북

## 배경지식
* HTML을 먼저 불러온 후 자바스크립트를 실행한다.   

> 문서 하단 <body> 태그가 끝나기 전에 작성한다. 
> /basicSyntax/internalJS.html

* 성능 향상을 위해 CSS3와 자바스트립트 간의 역활 분담을 해야한다.

> CSS3의 그래픽 처리는 하드웨어 가속으로 작동해 자바스크립트의 그래픽 처리 보다 현저히 부드럽다. 
> /basicSyntax/css3&jQuery.html

## Basic Syntax
* 동적 타입의 변수 선언    

> 특정 값을 입력하는 순간 타입이 자동으로 선언된다. 
> /basicSyntax/jsDynamicTypes.html


* UX/Ui 기본

> document.write 함수 사용  
> /basicSyntax/multipleTable.html  

> document.getElementById 함수 사용  
> /basicSyntax/nickBackground.html

> eventhandler 응용
> /basicSyntax/NightorDay.html

* for

> /basicSyntax/forloop.html


* function

> /basicSyntax/functionJS.html

* callback

> 많이 사용되는 콜백 함수다 익숙해지자
> /basicSyntax/callbackJS.html

* array

> /basicSyntax/arrayJS.html

* object

> /basicSyntax/objectJS.html 


## DOM  
* single Selector  

> document.getElementById(id명): 아이디 사용해 문서 객체(요소) 선택
> document.querySelector(CSS 선택자): CSS 선택자를 사용하는 방식(IE 8 이상)  
> /DOM/singleSelector.html

* multiple Selector

> document.getElementsByTagName(요소명): 태크명으로 여러 문서 객체 선택
> document.getElementsByClassName(클래스명): 클래스명으로 여러 문서 객체 선택(IE 9 이상)
> document.querySelectorAll(CSS 선택자): CSS 선택자로 여러 문서 객체 전달(IE 9 이상)
> /DOM/multipleSelector.html

* 텍스트 조작

> DOM.innerText: 요소 내부의 텍스트를 읽거나 변경
> DOM.innerHTML: 요소 내부의 HTML 형식을 읽거나 변경
> /DOM/innerText&innerHTML.html
 
* Style 객체

> 요소.style.backgroundImage: background-image 
> 요소.style.backgroundColor: background-color 
> 요소.style.listStyle: list-style 
> /DOM/styleObject.html

* 속성 조작

> setAttribute(속성명, 값): 속성값 설정
> getAttribute(속성명): 속성값 읽기
> removeAttribute(속성명): 속성 제거
> /DOM/setAttribute.html
> /DOM/getAttribute.html
> /DOM/removeAttribute.html

* 응용

> make div Red or Blue
> /DOM/red&blueButton.html 


