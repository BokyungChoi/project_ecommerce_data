##### Meeting Log & Timeline
---

### 1st : 프로젝트 아웃라인 소개, 플젝장 정하기
#### Overview
- 일시: 9/19
- 작성자: 최보경  
- 참석자: 전원

#### Pre-shared (해온 것을 공유)
<details>
  <summary> Click to expand! </summary>
  1. 데이터셋 소개자료
  2. 지난 프로젝트에서의 방황 이야기
</details>

#### Contents and Decisions (결정 사항)
- 앞으로 기대하는 프로세스: 데이터 분석 A to Z 를 경험해보는 것이 우선순위 목표

#### Forward Plans (앞으로 할 것을 이야기)
1. 변수설명 한글 파일 + pdf 파일 
   => 각 6가지 파일을 pd.read_csv()
   주피터를 통해서 읽어보고, 변수에 대해 이해
2. EDA, 전처리, 모델링 다 무엇인지에 대한 구글링

---
### 2nd : 데이터 구조와 변수 파악

#### Overview
* 일시: 9/21 17:00 ~ 18:00
* 작성자: 최보경
* 참석자:

#### Pre-shared (해온 것을 공유)
<details>
  <summary> Click to expand! </summary>

- 데이터셋에 대한 생각, 모르는 것
 동민: session 데이터셋에서 sess_seq sess_id 가 헷갈린다. session이 어렵다.
 동진: 결과적으로 상품 구매를 유도하는데, hit을 어떻게 유도할 수 있을까? 선후관계를 어떻게 파악할 수 있을까? hit 상품 구매 최소 단위
 원지: 
 한 명의 방문자여도 여러개의 adid. 세션 단위를 한 사람으로 카운트해도 괜찮을까?
 검색어 관련 데이터셋은 EDA가 어렵지 않을까?
 
- EDA, 전처리 프로세스에 대한 구글링
 리서치 자료는 공유
 http://www.dodomira.com/2016/10/20/how_to_eda/
 https://towardsdatascience.com/a-gentle-introduction-to-exploratory-data-analysis-f11d843b8184
 https://eda-ai-lab.tistory.com/13
 https://wanzargen.tistory.com/1
  
</details>

#### Contents and Decisions (결정 사항)

1. 데이터셋 분담
동민 - Product
동진 - Search1
원지 - Search2
민섭 - Custom
상품 분류 left

2. 전처리는 차후로 미루고, 이번에는
> 1) EDA(통계량 분석, groupby 해서 묶어서 보기, 파이썬으로는 value_counts 함수, 눈으로 훑어 변수 이해, 변수들간 상관관계 파악)
> 2) 아웃라이어 제거
> 3) 각 데이터셋을 더 파고들어 보자. 더 깊은 고민을 해보자


#### Forward Plans (앞으로 할 것을 이야기)


### 3rd : 데이터 구조와 변수 파악

#### Overview
* 일시: 9/24 21:30 ~ 22:50
* 작성자: 최동민
* 참석자: 강동진, 김종찬, 김현우, 서원지, 소민섭, 최동민

#### Pre-shared (해온 것을 공유)
<details>
  <summary> Click to expand! </summary>

- 데이터셋에 대한 생각, 모르는 것 <br/> <br/>
 동진: value count를 해본 결과 의류의 count 수가 제일 많았다는 것이 좀 의미있었다. <br/>
 민섭: gender랑 age를 위주로 봄. age는 평균 33세. 30대에 비해 7,80대의 수는 너무 적어서 제외해도 될 것 같다. <br/>
 원지: 마찬가지로 의류의 count 수가 상위권. 검색어중에 오타나 의미없는 것이 많아서 처리를 해보고자 했다. <br/>
       검색어가 브랜드명, 품목, 혹은 둘이 섞인 것이 많이서 이들을 어떻게 구분해야 할지 고민이 된다.  <br/>
 동민: product 구매 가격과 양이 숫자형으로 되어있지 않아서 숫자형으로 처리. 데이터 분포가 특이해서 고민이 된다. <br/>
 
</details>

#### Contents and Decisions (결정 사항)

merge된 데이터프레임 가지고 y값 예측을 위한 변수로 어떤 것들을 사용할지 아이디어 생각해보기, 지표 만들어보기
코드로 구현해오기

ex)
이 client가 몇번째 방문인지
평균 몇일 이내에 방문하는 고객인지
client id는 feature로 넣지 않았다.
평균 얼마 썼는지
월말 월초 요일
검색 키워드-전체검색량 대비 개인 검색량-->높으면 검색에 대한 적극성이 높았구나...

#### Forward Plans (앞으로 할 것을 이야기)
==
#### Overview
* 일시: 9/24 21:30 ~ 22:50
* 작성자: 최보경
* 참석자: 강동진, 김종찬, 김현우, 서원지, 소민섭, 최동민

#### Pre-shared (해온 것을 공유)
<details>
  <summary> Click to expand! </summary>

- 데이터셋에 대한 생각, 모르는 것 <br/> <br/>
 동민<br/>
 - 30%의 고객이 77%의 매출을 차지한다. 최상위에게 가중치를 준다. vip 고객에 대한 차등.
 <br/>
 - 피드백 한 사람당 최근 20개 기록. (종찬) 가치 있는 구매를 하는가?
 <br/> 
 - 6개월 문제
 <br/>
 원지
 <br/>
 - 대략적으로 그 페이지당 사용한 시간. page_view한 시간, 제품 정보를 볼 때는 더 오래 머무르지 않을까의 가설. 
 - avg page view 변수 생성. (300
 - 재구매 없는 사람들은 제거한 상태의 플랏
 - 반복적으로 특정 제품을 구매하는 패턴 
 - 월급날 효과 (가장 구매를 많이 한 날이 월급날일까 싶어서 봤지만 특별하지 않았다)
<br/>
민섭
<br/>
- 의외로 무의미해보이는 컬럼을 넣으면 모델 성능이 좋을 수도 있다.
- tot_session hour v * 세션에서 많이 움직인 수 곱하여 컬럼 생성
- device 컬럼에 따라서 재구매 횟수가 다를까의 가설
<br/>
동진
<br/>
- 연령대별, 검색기기별, 평균구매건수 & 총 페이지 뷰 수 
- 연령대별과 검색기기별은 가설과 달랐다. 
 
</details>
#### Forward Plans (앞으로 할 것을 이야기)

동진 & 동민:동민 아이디어 좋다. 더 진행해보자. 가중치로 컬럼 만들어 넣으면 y와 다른 columns과 관계 보기 가능한 액션: 모델 성능 높이기
동진: 아웃라이어 제거 
원지: 프러덕트와 서치 연결해서 보고 싶었으나, 할 수 있을지 모르겠다. 연령대랑 구매액이랑 기기별로 차이를 보고 싶다. 
+ ( 동일한 product를 n번 이상구매한 단골고객?을 labeling해보자)
민섭: 오늘 전달한 부분을 시각 자료로 구현. 
 
