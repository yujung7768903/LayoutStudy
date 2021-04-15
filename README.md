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

