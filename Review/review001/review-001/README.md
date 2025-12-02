# ESTbootcamp-Review

> text-align은 블록요소 내부에서 텍스트+inline요소(span,img,a등) 가 어떻게 정렬 될지를 결정하는 속성

> **padding** 은 요소의 내용(content)과 테두리(border) 사이의 내부여백을 의미한다.

> ┌───────────────────────────┐ ← border(테두리)
> │ `padding 영역
> │ ┌───────────────────┐ 　 　 　
> │ │ content 　　　　　　　　　
> │ └───────────────────┘
> └───────────────────────────┘

# Padding 값 설정 방식

> 1. 모든 방향 같은 값 padding: 20px;
> 2. 상하/좌우 padding: 10px 20px;
> 3. 4방향 각각 따로 padding : 10px 20px 30px 40px;
>    /_ 순서 :top right bottom left 12시 3시 6시 9시_/
> 4. 개별 속성가능 padding-top , padding-right: 10px; 형식

### Padding이 요소 크기에 미치는 영향

기본적으로 요소의 실제 크기는 다름

> width + padding + border
> height + padding +border

` .box {width:200px padding:20px }`

> 실제 보여지는 폭은 200+20+20 = 240px

## **bacground** 정의

`background`는 **요소의 배경 전체를 설정하는 '배경 속성들의 묶음(단축 속성, shorthand)'**이다.

즉,
단 하나의 속성으로 배경색 + 배경이미지 + 반복 + 위치 + 크기 등을 한 번에 설정할 수 있다.

## **background-color** 정의

`background-color` 는 요소의 배경색을 지정하는 css속성

## **border-radius** 정의

`border-radius` 는 요소의 모소리를 둥글게 만드는 css속성

## **box-shadow** 정의

`box-shadow` 는 요소(박스)에 그림자를 넣는 속성이다.

## **font-size** 정의

`font-size` 는 텍스트의 글자크기(폰트크기) 를 지정하는 css속성

> font-size가 적용되는 대상 (텍스트전체,inline요소(span,a등) block 요소 내부 텍스트,버튼 안 글자,input/textarea 안 글자 )
> rem 반응형 웹에서 가장 좋은 단위 1rem = 16px (HTML 기본 글자크기 기준)

## **color** 정의

`color` 는 텍스트의 색상을 지정하는 css속성

## **line-height** 정의

`line-height` 는 텍스트 줄과 줄 사이의 간격(줄 높이)를 결정하는 css속성

## **display** 정의

`display`는 요소가 화면에서 어떻게 보이고 ,배치되고,공간을 차지할지 결정하는 css 속성이다

> `display: block`
> 가로 전체 너비(100%) 차지
> 줄바꿈 발생
> width/height/padding/margin 적용 O
> 예:
> `display: block;`
> 대표 태그: div, p, h1~h6, section, header

> `display: inline`
> 자신의 내용(content)만큼만 차지
> 줄바꿈 X (옆에 다른 요소 올 수 있음)
> width/height 설정 불가능
> padding, margin 중 좌우만 적용됨
> `예: display: inline;`
> 대표 태그: span, a, strong

> `display: inline-block`
> inline처럼 옆에 배치 가능
> block처럼 width/height 지정 가능
> `예:display: inline-block;`
> 버튼 레이아웃에 자주 사용됨.

> `display: none`
> 화면에서 완전히 사라짐
> 영역(공간)도 없음
> `display: none;`
> (visibility: hidden과 다름 → 공간은 남고 보이지만 않음)
> 레이아웃 시스템

> `display: flex`
> 부모 요소를 “플렉스 레이아웃 방식”으로 바꿈
> → 가로·세로 정렬, 센터 정렬, 비율 배치 등 매우 강력
> `display: flex;`
> 대표적으로 반응형 레이아웃에서 필수.

> `display: grid`
> 격자(grid) 형태의 레이아웃
> 2D(가로+세로) 설계에 최강
> display: grid;

## **gap** 정의

`gap` 은 flex 또는 grid 컨테이너 내부에서 **아이템 사이의 간격을** 설정하는 css 속성

## **flex** 정의

`flex`란 유연한 1차원(한줄) 레이아웃을 만들기 위한 css배치 방식

### flex를 구성하는 속성들

![로고](./image/flex.png)

## **hover** 란?

> `:hover` 마우스 커서를 요소 위에 올렸을때 실행되는 상태
