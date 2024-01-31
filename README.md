## RFM을 활용한 실버세대 타겟 마케팅
|기간|Tags|역할|
|:---:|:---:|:---:|
|2021.05. ~ 2021.06.| DataAnalysis, Clustering |팀장, 인사이트 발굴, 군집화 및 마케팅 전략 제시|

#### 요구사항: 실버세대의 라이프스타일을 이해할 수 있는 특징을 분석 및 추정하고 이와 관련된 마케팅 전략 제시
#### 1. 문제 정의 및 목표 설정
- RFM 기법으로 고객을 세분화한 뒤 군집별 고객의 라이프스타일을 도출해 마케팅 전략을 마련한다.
- 마케팅을 통해 매출액 증가를 목표로 한다.

#### 2. 데이터 설명
외부 데이터를 사용할 수 없어 제공되는 롯데계열사 데이터만 사용한다.
![CRM](https://github.com/HASEOKYUNG/CRM_for_SilverGeneration/assets/104245855/963ad5a9-2411-45d6-b9df-5c622feb80c6)


#### 3. 데이터 전처리
- 구매가격의 이상치의 발생 과정을 확인하며 증정 행사임을 밝혀냈다.
- 구매지역별 상품 종류의 차이로 매장 유형을 백화점과 하이마트로 구분한다.
- 구매일자, 시간을 고려해 고객 여정 ID를 생성한다.
- 발생할 수 없는 환불 데이터는 제거한다.

#### 4. 피쳐 엔지니어링 & 모델링
- Recency, Frequency, Monetary를 구한 뒤 Z-score로 이상치를 제거한다.
- Kmeans를 사용하며 Elbow를 근거로 충성고객, 일반고객, 이탈고객, 3개의 군집으로 나눈다.

#### 5. 결론 도출
- 고객 군집별 관심 상품, 구매액이 컸던 시기, 행사를 도출하고 관련 마케팅 방안을 제시한다.

#### 배운 점
- 고객이 원할 서비스를 제공하는데 고객을 이해하는 것이 선수됨을 체감했다.
- 고객에 대한 이해를 높이기 위해 노력하며 다양한 접근을 통해 특징을 찾고 전처리를 수행했다.
- 마케팅에 대한 지식이 부족해 현실적인 방안 마련을 하지 못했다. 마케팅에 관해 공부해야 한다.
