<h1 align="center">Float 예제</h1>
  
>+2019.09.30 Float 예제 등록
<p align="center">
:full_moon_with_face: :blush: :seedling: :bell: :koala: :octocat:  
</p>

-CSS를 float로 작업을 하다보면 요소가 의도와는 크기가 벗어나거나 뭉개지는 현상이 발생하는데 원하는곳에 포지셔닝을 하기위해 clearfix라고 하는 오류를 해결하기위해 만들어낸 방법이 있다.
>1. clear 속성 적용 
>2. overflow 속성 적용
>3. 가상요소 ::after를 사용(권장)

1. clear 속성을 사용
```css
    .divstyle{
        width:200px;
        height: 250px;
        border:1px solid black;
        float:left;
    }
    .divstyle2{
        clear:left;
    }
```
```html
    <div class="divstyle">
        Think like a man of action and act like man of thought.
            Courage is very important. Like a muscle, it is strengthened by use.
            Life is the art of drawing sufficient conclusions from insufficient premises.
            By doubting we come at the truth.
    </div>
    <div class="divstyle2">
        We give advice, but we cannot give conduct.
        Nature never deceives us; it is always we who deceive ourselves.
        Forgiveness is better than revenge.
        We never know the worth of water till the well is dry.
        Pain past is pleasure.
    </div>
```
# **The Result**
result1

2. overflow 적용 하여 의도와는 크기가 벗어나는것을 해결
```css
    div{
        border:1px solid yellow;
    }
    img{
        float:right;
    }
    .clearfix{
        overflow: auto;
    }
```

```html
    <div>
        <img src="https://placeimg.com/128/128/2">
        Think like a man of action and act like man of thought.
            Courage is very important. Like a muscle, it is strengthened by use.
            Life is the art of drawing sufficient conclusions from insufficient premises.
            By doubting we come at the truth.
    </div>
    <p style="clear:right">Add a clearfix class with overflow: auto; to the containing element, to fix this problem:</p>

    <div class="clearfix">
        <div >
                <img src="https://placeimg.com/128/128/2">
                Think like a man of action and act like man of thought.
                Courage is very important. Like a muscle, it is strengthened by use.
                        Life is the art of drawing sufficient conclusions from insufficient premises.
                        By doubting we come at the truth.
        </div>
    </div>
```
# **The Result**
result2
3. 가상요소 ::after을 사용
```css
.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
```
```html
<div class="divstyle">
        <h1>Without clearfix</h1>
        <img src="https://placeimg.com/128/128/2"/>
        Think like a man of action and act like man of thought.
            Courage is very important. Like a muscle, it is strengthened by use.
            Life is the art of drawing sufficient conclusions from insufficient premises.
            By doubting we come at the truth.
    </div>
    <p style="clear:right">to solve clearfix</p>
    
    <div class="clearfix">
            <h1>With clearfix</h1>
            <img src="https://placeimg.com/128/128/2"/>
        We give advice, but we cannot give conduct.
        Nature never deceives us; it is always we who deceive ourselves.
        Forgiveness is better than revenge.
        We never know the worth of water till the well is dry.
        Pain past is pleasure.
    </div>
```