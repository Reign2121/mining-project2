# Mining-project2

프로젝트 개요

목표: 모교인 서울과학기술대가 소재한 공릉동의 상권을 분석하여 해당 상권의 소비자군의 특성, 소비패턴을 도출하여 적절한 시사점과 전략을 제안한다.

데이터: 공공데이터 포털의 서울시 상권 데이터에서 공릉동 지역을 발췌했습니다. (실제 데이터)

- 데이터의 상권 코드를 도메인에 맞게 새로운 카테고리로 분류하였습니다. 

  ex) (한식, 일식, 중식 -> 음식점) / (철물점, 잡화점, 시계, 안경, 고시원 등) -> 생활
  
__

이 프로젝트에서 제가 가장 신경 쓴 부분은 마케팅 개념을 분석흐름에 잘 녹여내는 것이었습니다.

저는 효과적인 상권분석을 위해 분석흐름을 고민하던 중 "STP 전략"에서 아이디어를 얻었습니다.

*STP 전략 (Segmentation, Targeting, Positioning)

STP 전략은 마케팅에서 전략적 활동을 결정하는 주요 전략으로 쓰입니다.

특히 이는 비즈니스 도메인에서 시장을 세분화하고, 타겟을 설정하여, 그 타겟에 맞는 전략을 제시하는 기본적인 분석 방향으로 제안되곤 합니다.

__

가장 먼저 

1. S, segementation을 통해 소비자군을 나누어 각 segment에 속한 소비자들의 특성과 소비패턴을 도출합니다.

2. 이후, 앞서 도출한 segment별 특성을 바탕으로 T, target을 도출하여 전략적인 방향을 설정합니다.

3. 마지막으로 P, Positioning은 자사의 제품이나 서비스가 소비자들의 인지 속에 어떻게 자리잡을 지, 그것을 고안하여 구체적인 전략을 제시하는 단계입니다.

*그런데 이 분석의 목표는 어떠한 특정 제품, 서비스에 대한 것이 아니므로 타겟을 더 많은 구매로 이끄는 전략들을 모두 positioning이라고 보았습니다.

__

위와 같은 흐름을 고려하여 다음과 같은 분석기법을 선택, 적용하였습니다.

1. S: Segmentation, 군집분석
2. T: Targeting, 회귀분석
3. P: Positioning, 마케팅 전략 제시

여기서 2. Targeting에서 회귀분석의 종속변수로 "분기별_매출_건수"를 선택하였습니다.

왜냐하면, 각 서비스 업종의 분야와 그에 따른 가격이 상이할 뿐만 아니라 매출 건수와 매출 금액 간의 매우 강한 양의 상관관계가 관찰되었기 때문입니다.

*즉, 매출 건수가 높을 수록 매출 금액이 올라가며, 소비자들이 많이 이용하도록 하는 것(매출 건수를 높이는 것이)이 상권의 활성화에 있어서 더 유효한 시사점이라고 보았습니다.

__________

![image](https://user-images.githubusercontent.com/121419113/218407619-bf0a1e00-722f-47bc-bbb0-fab9e4648f7a.png)

서비스 업종 분포 

![image](https://user-images.githubusercontent.com/121419113/218407699-985d0ff3-d26c-4194-b3a0-706d367fad18.png)

성별에 따른 매출 비율

![image](https://user-images.githubusercontent.com/121419113/218407779-d633c09d-9ef1-4420-9dc2-7deb5871f66b.png)

연령에 따른 매출 비율

_____

<img width="830" alt="image" src="https://user-images.githubusercontent.com/121419113/218412310-a572f964-823b-4967-9f14-e0eb0bd10061.png">



