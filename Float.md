<h1 align="center">Float 예제</h1>
  
>+2019.09.30 Float 예제 등록
<p align="center">
:full_moon_with_face: :blush: :seedling: :bell: :koala: :octocat:  
</p>

Today should learn
- CSS의 float속성은 화면의 요소가 어떻게 떠야하는지를 정해준다.  
- CSS의 clear속성은 화면의 요소가 제거된요소옆에 떠야하는지를 정해준다.  
- 다음편에 CSS의 clear속성을 알아보도록 하자
[Link:]

>:exclamation:Note  
>float을 사용하게 되면 inline으로 바뀌게 됩니다.  
>:boom:div,p,h1..h6,selection 등 float속성 사용시 block->inline으로 변경:boom:
## **float:none**

<p>
<img src="https://placeimg.com/320/320/2" alt="" style="float:none"/>
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
    </p>

float 를 사용을 하지않으면 none가 기본 설정값이다.
사진의 마지막 오른쪽 끝부분에 글귀가 붙는다.  
## **float:left**
```css
<style>
    img{
            float:left;
        }
</style>
```
![float-left](https://user-images.githubusercontent.com/32647144/65856938-c8d0ab80-e39d-11e9-8884-f6e12fd57fce.png)