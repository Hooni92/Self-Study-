# 서론 
- Project를 진행하면서 부족했던점을 공부하거나 배우고싶었던 것을 공부한걸 기록하기 위해 만들었다.
# 본론
## display : gird and flex
web page를 디자인하기 위하여 그림판에 원하는 webpage layout을 그려보았다.<br>
그림판의 layout처럼 div(block)영역의 넓이나 높이, 위치들이 생각처럼 되지않아 Webpage Layout 을 구성하는데 어려움을 겪었다.<br>
이같은 문제를 해결하기 위하여 flex와 grid를 알게되었고 학습 후 각각의 방법으로 같은 Web page layout을 만들어 보고 각각의 장점이 무엇인지 알아보려한다.<br>
- flex
- grid
  1.TEST page는 아래와 같이 준비하였다.
    1. test body<br>
![image](https://user-images.githubusercontent.com/108508922/180649136-572813ab-1293-47bc-bed4-083ecab366ba.png)
    2. test style<br>
![image](https://user-images.githubusercontent.com/108508922/180649391-fd3ce101-4561-4ad9-83c5-d582521fe5b4.png)
    3. test page<br>
![image](https://user-images.githubusercontent.com/108508922/180649380-a0b7534f-183b-47b9-8e1e-aae3729ba8ed.png)
  2. display: grid 
    1. 설정은 페이지 변화를 주지않는다.<br>
![image](https://user-images.githubusercontent.com/108508922/180649475-4280108c-22e8-4d10-9e52-73a7bd79d5ee.png)
  3. grid-template-columns
    1. 30% 70% 설정된 비율에 맞게 페이지가 구성되며 페이지 폭에 맞춰 반응형으로 작동된다.<br>
![image](https://user-images.githubusercontent.com/108508922/180649576-46c453bc-adce-4ebf-bad8-ce4d31559cc9.png)
    2. 30% 70% 와 똑같이 비율에 맞게 페이지가 구성되는 다른 표현 fr.<br>
![image](https://user-images.githubusercontent.com/108508922/180649837-882cfb70-41a8-469d-9baf-c64f4f09fdd9.png)
    3. repeat(나눌 컬럼수, 비율)을 활용하여 반복되는 컬럼 나눔을 표현가능하다. <br>
![image](https://user-images.githubusercontent.com/108508922/180650248-6912c1bb-bc93-4984-97c2-ade2aec02f7e.png)
    4. px로 넓이를 고정시키면 웹페이즈 크기에 따라 반응하지않고 고정된 넓이를 가진다.<br>
![image](https://user-images.githubusercontent.com/108508922/180650354-c20113eb-e062-4145-af42-6b4da3353844.png)
  4. grid-gap
    1. grid-gap을 이용하면 모든 컬럼에 일정한 gap을 쉽게 줄수 있는 장점이 있다 
    2. gap을 주면 grid-template-columns 의 %비율은 가로스크롤을 주므로 fr로 비율 설정을 하는게 더 좋다.<br>
![image](https://user-images.githubusercontent.com/108508922/180650038-8bc3c38c-fbd9-442b-8074-e5f74b03d173.png)
  5. grid-auto-rows:
    1. grid-auto-rows: minmax(최소높이, 최고높이)
    2. 아래의 설정값은 컬럼은 최소 150px의 높이를 가지고 최고높이는 최고 컨텐츠에 맞춰 정렬된다.<br>
![image](https://user-images.githubusercontent.com/108508922/180650751-b8940e04-755b-4e06-8fc5-f79a4dc863ab.png)
  6. justify-items: start, center, end
    1. 각 컬럼이 수평축을 놓고 움직인다.<br>  
![image](https://user-images.githubusercontent.com/108508922/180651065-26b651cc-b325-4415-be1f-2225b95db2f8.png)
  7. align-items: start, center, end
    1. 각 컬럼이 수직축을 놓고 움직인다.<br>
![image](https://user-images.githubusercontent.com/108508922/180651185-7718b18e-ec32-42b8-80fb-c3e1fb07ab7a.png)
  8. justify-selft:
    1. container안의 컬럼을 각각 정렬할 수 있다.<br>
![image](https://user-images.githubusercontent.com/108508922/180651344-b41a1fa0-7fad-44ed-813a-40f33c3e8c59.png)
  9. grid-column, grid-row
    1. 각 셀이 차지하는 공간을 지정할 수 있다. 
    2. 각 컬럼이 나누어지는 공간을 축으로 생각하고 제일 왼쪽 혹은 위가 1번으로 시작한다.<br>
![image](https://user-images.githubusercontent.com/108508922/180651557-6b5d4bc8-8e32-4fc9-9866-d8817fb4fb73.png)
    4. 각 컬럼의 시작지점을 지정하여 위치를 변환시킬수 있다.
![image](https://user-images.githubusercontent.com/108508922/180651733-5e96044d-3605-498b-a855-b018baf6e363.png)



-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
- grid layout code<br>
![image](https://user-images.githubusercontent.com/108508922/178519821-45151722-233f-4cfc-924c-1723ce80f4af.png)
- grid output<br>
![image](https://user-images.githubusercontent.com/108508922/178518837-7af58885-a3f6-450c-873c-36fdeb9b6356.png)

------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## position
-absolute
-relative
-fix
------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-좌 우측 광고베너 추가 + 로그인 nav 추가
![image](https://user-images.githubusercontent.com/108508922/179122412-947e9a58-73fd-4587-98e1-f0162a122957.png)

