alovena의 CSS 저장소 Overflow편(Overflow.md)
:blush: :collision: :musical_note: :hand: :droplet:
# *Overflow의 모든것*
> 2019.09.25 

CSS의 overflow 속성은 페이지의 크기를 벗어날때 제어를 한다.

overflow 속성은 크게 4가지가 있다.
-visible : 크기를 벗어나도 크기를 벗어난채 보여준다.
-hidden : 크기를 벗어나면 보이지 않는다.
-scroll : 크기를 벗어나면 content에 스크롤이 생성된다.
-auto : scroll 과 비슷하지만 필요할때만 스크롤을 보여준다.
<blockquote style="background:#30A9DE">
    :exclamation:Note:exclamation: : overflow 속성은 오직 block 요소에만 적용됩니다.
    즉, div p h1..h6 section 등에만 적용되고 
    inline 요소에는 적용되지 않습니다.
    :boom: a,img,span tag :boom:
    하지만 inline->block 요소로 바꿔주면 가능합니다
</blockquote>
```css
    a,img,span{
        display:block
    }
```

예제를 살펴보겠습니다.
## *overflow:visible*
```html
    <div></div>
```
```css
```
## The Result : ↓

## *overflow:hidden*
```html
    <div></div>
```
```css
```
## The Result : ↓

## *overflow:scroll*
```html
    <div></div>
```
```css
```
## The Result : ↓

## *overflow:auto*
```html
    <div></div>
```
```css
```
## The Result : ↓
