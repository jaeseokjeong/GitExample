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


## [<8 ways of Boosting Performance of Machine Learning Models>](http://houseofbots.com/news-detail/2520-4-8-ways-of-boosting-performance-of-machine-learning-models)

1.	Data 추가
상황에 따라 추가해야 될 시기는 다르다. 시계열의경우 적어도 1년치 필요. Neural network도 많이 필요

2.	Feature engineering (변수추가)
새로운 변수추가는 모델의 variance를 증가시키는 대가로 bias를 줄임.
존재하는 데이터로부터 변수를 뽑아내야 한다. 예를들어 ATM에서 현금인출을 예측하고 싶을 때 월초에 더 많이 인출될 것이다. 사기탐지 모델 만들 때는 소득대비 대출비율들을 만들 수 있음

3.	변수선택 (Feature selection)
Make everything as simple as possible, but no simpler – Albert Einstein
Select best features, add new features
각각의 변수가 모델에 기여하는 정도를 살펴봐야 한다.
100개의 변수가 있을 때, 단순히 p-value기준으로 변수를 선택하면 여전히 많은 변수가 선택된다. 하지만 만약 15의 개의 변수로 모델의 90%가 설명된다면 15개 변수모델을 선택하는 것이 옳다.

4.	Missing value and Outlier treatment

5.	Ensemble Models
어떤모델은 데이터의 variance를 포착하는데 좋고, 어떤 모델은 트렌드만 포착하는데 좋기 떄문에 결국 합친 것이 더 잘 작동한다.

6.	Using the suitable machine learning algorithm
여러가지 모델을 해보고 가장 효율적인 것 찾아야 한다. 데이터에 따라 효율적인 모델이 다르기 때문

7.	Auto-feature generation
이것이 딥러닝의 가장 큰 장점. 머신러닝 알고리즘에서 변수의 quality는 정확성에 있어서 매우 중요하다. 그러나 딥러닝 알고리즘은 feature engineering을 필요로하지 않음. 스스로 학습한다. Ex 이미지분류

8.	Data distribution and parameter tuning
예를 들어, 랜덤포레스트 사용시 나무의 개수, 몇 개의 변수를 선택할지 등 파라미터 튜닝 필요. 또는 딥러닝 알고리즘 구현시 얼마나 많은 층을 필요로 할지 등.

## [<철학으로서의 통계학>](https://www.facebook.com/jaekwang.kim.125/posts/2128149037200925)


중세에서는 권위와 전통에 기대어 지식을 알려했다. 하지만 근대에서는 권위와 전통을 부정하고 오로지 경험과 이성을 통해서 새롭게 지식 체계를 세우고자 한다. 

종교의 영향력에서 벗어나 기존의 지식을 의심하고 참된 지식을 세우려는 노력에서 필요한 도구는 결국 경험(데이터)와 이성(논리)라는 것.
경험주의의 단점은 자칫하면 회의주의에 빠진다는 것. 

왜냐하면 지식이 데이터로부터 얻어지는 것은 인정하지만 우리는 모든 데이터를 다 관측할 수 없기 때문에 그 지식을 결코 신뢰할 수 없다는 난관에 부딪힘.

이러한 문제를 수리적인 방법으로 해결한 것이 통계학. 

통계학은 제한된 관측으로 얻어지는 결론에 대한 확실성의 정도를 확률이라는 개념으로 설명한다. 

확률을 계산하는 과정에서 수리적 논리를 부여하여 보편성을 획득한다. 통계학은 경험주의의 한계를 극복하고자 하는 인간 지성사의 커다란 선물.

통계학이 과학적인 방법론이지만 통계학을 사용한 모든 결론이 다 타당하거나 과학적인 것은 아니다. 데이터에 대한 전제를 만족하는지 확인해야하 하는데, 전제를 만족하는지 확인하는 것이 통계학 실력에 의해 좌우된다.

첫번째 전제는 데이터의 적절성이다. 적절성이란 데이터의 질적 지표인 대표성, 타당성, 신뢰성을 포함하는 개념이다.

두번째 전제는 모델의 적절성이다. 모형의 적절성은 모형이 데이테의 현실을 얼마나 잘 반영하느냐에 따라 판단된다.자료가 범주형인지 연속형인지, 시계열인지, 공간자료인지 ,계층적 구조를 가지는지… 자료의 구조에 대한 이해가 있어야 모형의 적절성이 충족됨.

