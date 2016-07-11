
# 제목 <!--<h1>제목</h1>과 같음 6개까지만 사용가능-->
## 제목2
### 제목3
#### 제목4
##### 제목5
###### 제목6

> 내용을 열심히 작성하면.
인용문으로 처리<br>
br도 줄바꿈

강조처리 *기울기* **굵게** ***기울고 굵게*** <br />
강조처리 _기울기_ __굵게__ ___기울고 굵게___

___

```
  <h1>markdown logo</h1>
  <p></p>
```
  <p>간단하게 처리</p>

`<br>` &lt;br&gt; 내용을 보이고 설명

[네이버](http://naver.com)
<http://naver.com>

</http://naver.com>

![네이버](http://naver.com) <!-- 이미지삽입할때-->

`<!--  -->` 주석처리

# css 기본이해하기
> css란 html문서의 구조형태를 디자인으로 변화시키는것(꾸며주는것)

1. 선택자
  - type 선택자 : `p{}`, `div{}`
  - id 선택자 : `#box{}`, `#test`
  - class 선택자 : `.box{}, `.test` 
  - 자손 선택자 : `div p{}`, `container ul a{}`
  - 자식 선택자 : `div>ul>li{}`, `.container>ul>li>a{}`
  - 속성 선택자 : `a[href="#"]{}`, `a[taget="blank"]{}, `a[gerf^="http"]{}`
2. 공간의 이해
  -margin : 자신의 주변의 공간을 주는것
  -padding : 자신이 커지는것(커지는 크기에는 어떠한 요소를 담을 수 없다.)
  -border : 외곽선을 주는것(부피 o, 크기o)
  -outline : 외곽선을 주는것(크기만 존재, 부분을 바꿀 수 없다. -접근성 사용시 포커스 처리될때 사용)
3. RGBA ,webRGB ,HSLA
  - RGB: red, green, blue 컬러를 이용한 빛의 3원색(3색이 모두 모이면, 흰색)
    +red: 0~255(256단계) 0은 색이 없다, 255는 색이 꽉찼다.
    +rgba: red,green, blud, alpha(투명도 0~1)
    +rgba(red, green, blud, alpha)
  - wedRGB: #으로 시작해서 총 6자리의 숫자로 표기(압축시에는 3자리로 표현 가능)
    + 숫자: 0~9, a~f(숫자의 개념) f=16
    + 기본 2자리씩 끊어서 사용: #ff(red)ff(green)ff(blue)
    + f(16)f(16) = ff(256)
    + #000(#000000), #00ff44(#0f4), #fff677(3자리 변경 불가)
    + #000(검정), #fff(흰색), #aaa(회색), #777(회색), #555(회색)
    + 빨간색, 붉으스름한색, 벌건색, 밝가므리한색
    + #faa(밝은 빨강), #afc(녹색이 들어있는 밝은색 계통-민트색)
  - HSLA: hue(색상), asturation(채도), light(명도), alpha(투명도)
    + 먼셀 색입체
    + hue(360deg)deg=도 를 표현 : 360 = 0
    + saturation(0~100%): 0%(무채색), 100%(유채색, 순색)
    + light(0~100%) : 0(검정), 100%(흰색)
    + hsla(hue, saturation, light, alpha)  ==> hsla(30 50%, 50%, 1)
    + 색상 읽는 순서: a-l-s-h  순으로 읽는다
      - a : 1 투명도 먼저
      - l : 밝기 0:검정, 100%:흰색 50%
      - s : 채도 100:
      - h : 색의각도
4. float기능 이해 
  -float:left | right;
  -clear
      