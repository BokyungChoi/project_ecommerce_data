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


---
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


---
### 3rd : 데이터 구조와 변수 파악

#### Overview
* 일시: 9/24 21:30 ~ 22:50
* 작성자: 최동민
* 참석자:

#### Pre-shared (해온 것을 공유)
<details>
  <summary> Click to expand! </summary>

- 데이터셋에 대한 생각, 모르는 것
 동진: value count를 해본 결과 의류의 count 수가 제일 많았다는 것이 좀 의미있었다.
 민섭: gender랑 age를 위주로 봄. age는 평균 33세. 30대에 비해 7,80대의 수는 너무 적어서 제외해도 될 것 같다.
 원지: 마찬가지로 의류의 count 수가 상위권. 검색어중에 오타나 의미없는 것이 많아서 처리를 해보고자 했다.
       검색어가 브랜드명, 품목, 혹은 둘이 섞인 것이 많이서 이들을 어떻게 구분해야 할지 고민이 된다. 
  
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







