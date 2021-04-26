# LayoutStudy
## 1. Linearlayout
#### 특징
- weight을 이용해 가중치를 둘 수 있다.
- 수직 또는 수평 방향으로 정렬할 때 유용하다.
- 하지만 수직 또는 수평 중 한 가지의 방향만 가능하다. 따라서 복잡한 구조를 표현하려면 계층이 여러 개 필요하다.

#### orientation - 중심 축
- 중심 축을 기준으로 요소들이 위치하게 된다.
- horizontal : 수평
- vertical : 수직

#### weight - 가중치
- 고정값이 아닌 비율에 맞춰 레이아웃이 표현된다.
- ex) 아래의 예는 weightSum="3"이고 layout_weight="1"일 때 이다. 이 때 view는 전체 너비의 1/3만큼 차지하게 된다.

#### weightSum - 가중치의 합
- orientation이 horizontal일 때는 전체 가로의 비율을, vertical일 때는 세로의 비율을 정할 수 있다.    
- weightsum이 설정되지 않은 경우에서 a, b, c 가 각각 weight가 1, 2, 3일 때 a는 1/6만큼 b는 2/6만큼 c는 3/6만큼 차지하게 될 것이다.
- 하지만 weightsum이 10으로 설정이 된 경우 a는 1/10만클, b는 2/10만큼, c는 3/10만큼 차지하게 될 것이다.       
ex)          
아래의 예는 weightSum="3"이고 layout_weight="1"일 때 이다. 이 때 view는 전체 너비의 1/3만큼 차지하게 된다.               
만약 아래의 예시 그림에서 weightSum을 설정하지 않았다면, view는 전체를 차지 할 것이다.            

![image](https://user-images.githubusercontent.com/68562176/95116298-c6a7e680-0781-11eb-8856-7a65d9f36624.png)

#### gravity - 정렬
           
2. Constraintlayout
#### 특징
- 복잡한 뷰를 그릴 때 한 층으로 간단하게 그릴 수 있음.
- 화면 전환이 이루어졌을 때 그 비율을 유지한다.
*주의할 점 : 제약을 3개 이상 걸어야함(=어딘가에 고정을 시켜야한다는 뜻)

* constraint~~~

|constraint~|설명|
|------|---|
|constraintStart|constraint를 주고 싶은 요소의 왼쪽 점|
|constraintTop|constraint를 주고 싶은 요소의 위쪽 점|
|constraintEnd|constraint를 주고 싶은 요소의 오른쪽 점|
|constraintBottom|constraint를 주고 싶은 요소의 아래쪽 점|
* to~Of

|to~Of|설명|
|------|---|
|toStartOf="기준이 될 요소(ex:parent, id)"|기준이 되는 요소의 왼쪽 점|
|toTopOf="기준이 될 요소"|기준이 되는 요소의 위쪽 점|
|toEndOf="기준이 될 요소"|기준이 되는 요소의 오른쪽 점|
|toBottomOf="기준이 될 요소"|기준이 되는 요소의 아래쪽 점|

▼예시▼
```
app:layout_constraintStart_toStartOf="parent" 
```
-> 부모의 왼쪽 점과 요소의 왼쪽 점을 연결해라
