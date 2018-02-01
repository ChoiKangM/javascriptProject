# javascriptProject
자바스크립트 프로젝트북

<details><summary>배경지식</summary>
<p>

* HTML을 먼저 불러온 후 자바스크립트를 실행한다.   

> 문서 하단 <body> 태그가 끝나기 전에 작성한다. 
> /basicSyntax/internalJS.html

* 성능 향상을 위해 CSS3와 자바스트립트 간의 역활 분담을 해야한다.

> CSS3의 그래픽 처리는 하드웨어 가속으로 작동해 자바스크립트의 그래픽 처리 보다 현저히 부드럽다. 
> /basicSyntax/css3&jQuery.html  

</p>
</details>


<details><summary>Basic Syntax</summary>
<p>

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
</p>
</details>

  

<details><summary>DOM</summary>
<p>
    
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

</p>
</details>

<details><summary>이벤트 제어</summary>
<p>
    
* 마우스와 키보드 이벤트  

```

<요소 이벤트 핸들러 속성 = 'javaScript 명령어'>  

<a href="http://www.google.com" onclick ="alert('구글로 이동합니다.')">
  구글  
</a>

```  

> onclick           : 마우스를 클릭할 때  
> onmouseover       : 요소안에 마우스가 들어갔을 때  
> onmouseout        : 요소에서 마우스가 벗어났을 때  
> onkeydown         : 키보드를 입력할 때  
> onkeyup           : 키를 눌렀다 놓을 때  
> onfocus, onblur   : 요소가 선택됐거나 해제됐을 때  
> onsubmit          : 폼 전송 이벤트가 발생했을 때  


* 이벤트 핸들러

```
(문서 객체).(이벤트 속성명) = function(){}
```
> 자바스크립트가 문서를 조작하려고 할 경우 문서보다 먼저 작성하면 안됩니다.  
> /eventControl/beforeEventHandler.html  
> /eventControl/afterEventHandler.html

* 이벤트 객체와 this

> this는 이벤트가 발생한 객체 자신을 의미합니다.  
> 사용자가 클릭한 요소의 위치를 반환해주기 때문에 상대적인 지정 방식으로 자주 사용합니다.  
> /eventControl/thisEventHandler.html

* 이벤트 리스너

> 이벤트 핸들러는 객체에 속성으로 이벤트를 지정하는 방식
>> 요소당 하나의 이벤트  
> /eventControl/eventHandler.html   

> 이벤트 리스너는 메서드 방식입니다.    
>> 요소당 여러 개의 순차적인 이벤트 처리 가능 
> /eventControl/eventListener.html 

```
(문서 객체).addEventListener(이벤트 타입, 리스너);
```

> 이벤트 타입: 이벤트 속성을 지정합니다. 앞에 on을 붙이지 않습니다.  
> 리스너: 이벤트가 발생할 때 호출할 함수 또는 메서드를 지정합니다.   

* hover 구현

> 자바스크립트에 hover 이벤트가 따로 있지 않아  
> mouseover와 mouseout 이벤트를 조합해 구현할 수 있다.  
> /eventControl/hoverForJS.html

* submit 이벤트와 기본 동작 방지

> 기본 이벤트를 차단할 수 있다. preventDefault() 사용  
>  /eventControl/submitWithPreventDefault.html  

* 터치 이벤트

> touchstart: 화면을 건드렸을 때  
> touchend: 화면에서 손을 떼었을 때  
> touchmove: 화면에서 터치로로 이동 중일때  
> /eventControl/touchEvent.html

* 이벤트 바인딩

> 바인딩이란 함수를 외부에 작성하고 내부에는 함수명만 작성하는 방식  
> 처리는 동일합니다  
> /eventControl/eventBinding.html  

* 드래그 앤 드롭 구현

> /eventControl/touchEvent.html 참조해 만들었습니다.  
> clientX: 브라우저 화면을 기준으로 한 X 좌표  
> clientY: 브라우저 화면을 기준으로 한 Y 좌표  
> touchmove: 화면에서 터치로 이동 중일 때
> /eventControl/drag&drop.html  


</p>
</details>

 


