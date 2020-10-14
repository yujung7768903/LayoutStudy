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

![image](https://user-images.githubusercontent.com/68562176/95116298-c6a7e680-0781-11eb-8856-7a65d9f36624.png)

#### gravity - 정렬

