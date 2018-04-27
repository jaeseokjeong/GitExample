# article-about-data

## [<신한은행 이동경로 분석>](http://www.fntimes.com/html/view.php?ud=201803190023486486dd55077bc2_18)

신한은행은 고객의 금융 검색 여정을 추적해 이탈 가능성이 높은 고객을 붙잡는 이동경로분석 솔루션 구축

변수- 은행 앱에 로그인해서 투자상품을 검색한 횟수 같은 데이터. 고객이 투자상품을 3회 검색하는 순간 모바일 상담쪽지를 보내고 펀드가입 유도.

이동경로 분석을 통해 주요 현안에 대한 통찰을 얻을 수 있다.

## [<예측에서 피해야할 8가지 함정들>](https://www.kdnuggets.com/2018/03/8-common-pitfalls-ruin-prediction.html)

Keep in mind

#### 1.	Model Selection
Linear regression – 이해하기 쉽지만 복잡한 관계 설명 어려움

Decision Tree – 이해와 시각화 쉽지만 파리미터 신중하게 선택해야함

Random Forest- 높은 예측률 그러나 시각화하기 어렵고 느릴 수 있음

Neural Networks – 복잡한 경우 가장 높은 예측파워 하지만 extraordinarily compute-intensive 이것의 진행과정 이해하기 불가능

#### 2.	Overfitting

매우 협소하고 우연에 의해 일어날 법한 사건에 기반하여 결론을 내리는 경우를 의미. 동시에 조건들이 발생하는 경우가 매우 드물경우.

방지하기 위해 cross-validating 사용

예를들어, 좋은 예측은 하늘에 구름이 끼고 습도가 높으면 비올가능성이 높다. 오버피팅된 예측은 요일은 금요일이고 6월이고 지금 시간은 10시에서 11시사이에, 나의 차는 다른곳에 있을 때, 비가 올 가능성이 높다.

#### 3.	변수들간 시점을 동일하게. 과거와 미래를 섞으면 안된다.
몇개의 다른 변수들로 예측을 할 때, 변수들은 타겟보다 과거의 데이터여야 한다.
예를들어 인터넷 쇼핑 구매력 측정시, 웹에 있는 시간이라는 변수는 구매가 이루어진 후에도 지속적으로 측정되고 있따.

#### 4.	Outliers

#### 5.	Measuring the Efficiency
예측시 지속적으로 예측효율성을 체크해야한다.

그 이유는

1.	너무 좋거나 나쁜 예측결과는 나의 모델이나 예측에 문제가 있는 것을 의미

2.	시간에 따라 나의 예측이 어느 시점에 outdate되기 떄문에 그것을 탐지하기 위해

#### 6.	Not enough predictiors
주제와 관련된 한정된 도메인 지식만 이용하는 것은 문제. 

예를들어 아이스크림 매출을 예측할 때 아이스크림 관련된 변수를 사용하는 것 뿐만 아니라, 에어컨,비키니 매출 또는 정치적뉴스도 이용할 수 있다.

이러한 요인들이 아이스크림매출에 correlated 되어 있다. 

correlated된 변수를 추가하는 것은 큰 문제가 되지 않다. 

왜냐하면 예측알고리즘이 자동적으로 그것을 제거해줄 것이기 떄문이다.


## [<Difference of Data Science, Machine Learning and Data Mining>](https://www.datasciencecentral.com/profiles/blogs/difference-of-data-science-machine-learning-and-data-mining?utm_content=buffer724b0&utm_medium=social&utm_source=plus.google.com&utm_campaign=buffer)

data science: 모든 종류의 데이터를 다루는 것. Data cleansing, preparation 그리고 데이터 분석까지 모든 것을 포함한다. 여러가지 테크닉을 사용해 데이터에서 새로운 정보나 인사이트를 뽑아내는 전 과정을 의미. 

Data handling에 초점. 기존의 시스템에서는 사용하지 않았던 것에 데이터를 접목할 수 있도록.

data mining:이전에 몰랏던 것을 큰 데이터로 더미로부터 얻고 비즈니스 결정에 그 정보를 이용하는 과정. 알고리즘은 데이터로부터 지식을 얻는 하나의 수단일뿐.

Machine learning: 컴퓨터가 새로운 데이터에 대해 스스로 학습할 능력을 만드는 것. 알고리즘 짜는 것에 포커스가 되어있음



