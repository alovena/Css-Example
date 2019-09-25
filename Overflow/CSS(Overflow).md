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
    하지만 inline->block 요소로 바꿔주면 가능합니다.
</blockquote>

```css
    a,img,span{
        display:block;
    }
```

예제를 살펴보겠습니다.
```html
    <div class="overflow_Test">
                Think like a man of action and act like man of thought.
                Courage is very important. Like a muscle, it is strengthened by use.
                Life is the art of drawing sufficient conclusions from insufficient premises.
                By doubting we come at the truth.
                A man that hath no virtue in himself, ever envieth virtue in others.
                When money speaks, the truth keeps silent.
                We give advice, but we cannot give conduct.
                Nature never deceives us; it is always we who deceive ourselves.
                Forgiveness is better than revenge.
                We never know the worth of water till the well is dry.
                Pain past is pleasure.
                Books are ships which pass through the vast seas of time.
                Who begins too much accomplishes little.
                Better the last smile than the first laughter.
                Faith is a higher faculty than reason.
                Until the day of his death, no man can be sure of his courage.
                Great art is an instant arrested in eternity.
    </div>
```
## *overflow:visible*
```css
    .overflow_Test{
        width:50%;
        height: 200px;
        overflow:visible;
        background: #30A9DE;
        border:1px solid #ccc;
    }
```
## The Result : ↓
![visible](https://user-images.githubusercontent.com/32647144/65564997-a7c91e80-df89-11e9-8c35-ca66c3bc2db2.png)
  
## *overflow:hidden*
```css
    .overflow_Test{
        width:50%;
        height: 200px;
        overflow:hidden;
        background: #30A9DE;
        border:1px solid #ccc;
    }
```
## The Result : ↓
![hidden](https://user-images.githubusercontent.com/32647144/65564995-a7308800-df89-11e9-8e46-271a7bb6bf3f.png)  
## *overflow:scroll*
```css
    .overflow_Test{
        width:50%;
        height: 200px;
        overflow:scroll;
        background: #30A9DE;
        border:1px solid #ccc;
    }
```
## The Result : ↓
![scroll](https://user-images.githubusercontent.com/32647144/65564996-a7308800-df89-11e9-83a6-a622eedcc20d.png)  
## *overflow:auto*
```css
    .overflow_Test{
        width:50%;
        height: 200px;
        overflow:auto;
        background: #30A9DE;
        border:1px solid #ccc;
    }
```
## The Result : ↓
![auto](https://user-images.githubusercontent.com/32647144/65564993-a7308800-df89-11e9-8714-9375ef0fc3cb.png)  