Github 저장소의 Readme.md  
:heart_eyes: :grin: :open_mouth: :muscle: :pig:
# *Display 예제*  
> +2019.09.25 Display 예제

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
-HTML code 
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
-CSS code ...설명설명

### Ther Reuslt

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
-CSS code ...설명설명

### Ther Reuslt

### Source code : ↓
