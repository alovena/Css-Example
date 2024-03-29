<h1 align="center">Align Example</h1>

> ### 2019.10.04 Align 예제 등록
<div align="center">:bulb: :couple: :boy: :cop: :angel:</div>

<div align="center"><h1> margin:auto & padding :10px 방법<h1></div>

```css
.center{
    margin:auto;
    width:50%;
    border:3px solid green;
    padding : 10px;
}
```
```html
<div class="center">
<strong>Using margin:auto</strong>will make center align elements;
</div> 
```
![margin-auto](https://user-images.githubusercontent.com/32647144/66220563-35cea300-e708-11e9-92a7-e183d0d087ee.png)

<div align="center"><h1>text-align:cetner 방법<h1></div>

```css
.center{
    text-align:center;
    border:3px solid green;
    padding : 10px;
}
```
```html
<div class="center">
<strong>Using text-align</strong> will make center align elements;
</div> 
```
![text-align](https://user-images.githubusercontent.com/32647144/66220564-35cea300-e708-11e9-8850-da6dea47e261.png)

<div align="center"><h1>Using position&transform 방법<h1></div> 

```css
html, body, .container {
    height: 100%;
}
.container {
    position: relative;
    text-align: center;
}
.container > p {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
}
```

<div align="center"><h1>img align center<h1></div> 

```css
img{
    display:block;
    margin-left:auto;
    margin-right:auto;
    width:40%;
}
```