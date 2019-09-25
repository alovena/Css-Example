Github 저장소의 Readme.md  
:heart_eyes: :grin: :open_mouth: :muscle: :pig:
# *Display 예제*  
> +2019.09.25 우리는 왜 Display 속성을 사용하는가?

Display 속성은 CSS의 레이아웃을 잡아주는데 중요한 역활을 한다.  
display 속성은 크게 2가지로 나눌수 있다.  
### **Block과 Inline**  
**Block**는 화면을 한줄로 다차지한다.즉 width가 full로 사용을 하여 화면을 한줄로 다차지한다.  
Block를 사용하는 태그에는  
div h1..h6 p from header section 가 있다.  
반면 **Inline** 요소에는  
한 문장안의 요소가 들어가게 된다. 즉 한줄이아니라 한칸한칸을 차지하는 방식이다.  
Inline를 사용하는 태그에는
span a img 가 있다.  
코드를 보자  
다음 코드는 한줄을 차지하는 div,h1,p 태그를 한칸한칸으로 바꿔주는 코드이다.  
## *Block->Inline*
```html
    <div>
        <div class="div_display">div1</div>
        <div class="div_display">div2</div>
        <div class="div_display">div3</div>
    </div>
    <div style="margin-top: 10px;">
        <h1 class="h_display">h1</h1>
        <h1 class="h_display">h2</h1>
        <h1 class="h_display">h3</h1>
    </div>
    <div style="margin-top: 10px;">
            <p class="p_display">p1</p>
            <p class="p_display">p2</p>
            <p class="p_display">p3</p>
    </div>
```

```css
    .div_display{
        display:inline;
        border:1px solid red;
    }
    .h_display{
        display:inline;
        border:1px solid black;
    }
    .p_display{
        display:inline;
        border:1px solid green;
    }
```
위의 코드는 한줄한줄을 차지하는 태그들을 한칸한칸 차지하도록 바꿔주는 코드가
```css
div,p,h1{
    display:inline
}
```
이다  
네비게이션을 만들때, 태그를 일렬로 배치하고 싶을때 주로 사용한다.  
### **단점 : inline요소는 margin요소나 padding 요소를 적용 할 수 없다.line-height도 적용불가**
### Ther Reuslt : ↓
![inline](https://user-images.githubusercontent.com/32647144/65559378-6c245980-df75-11e9-9255-1acb6228987f.png)

Block 요소는 한칸한칸이아니라 한줄을 차지하는 방식이다.
코드를 보자  
다음 코드는 한칸한칸을 차지하는 a,img,span 태그를 한줄로 바꿔주는 코드이다. 
## *Inline->Block*
```html
    <div>
            <a class="a_display" href="#">link1</a>
            <a class="a_display" href="#">link2</a>
    </div>
```
-HTML code 
```css
    .a_display{
        display: block;
        border:1px solid pink;
    }
```
-CSS code  

위의 코드는 한칸한칸을 차지하는 태그들을 한줄로 차지하도록 바꿔주는 요소가
```css
div,p,span{
    display:block
}
```
이다  
## The Reuslt : ↓
![block](https://user-images.githubusercontent.com/32647144/65559377-6c245980-df75-11e9-9ab0-b35c91519642.png)

inline요소에는 입맛대로 커스텀을 하지못하여 나온게 inline-block라는 요소다  
가장 중요한것은 성질 자체는 inline을 따라가되 커스틈을 할 수 있도록 나온것이
```css
div,p,h1{
    display:inline-block;
}
```
이다.

## 결론 
-> 디테일한 보정이 필요하다면 inline-block, 특정부분 스타일등 간단한것들은 inline,block를 사용하도록 하자!
### Source code : ↓
