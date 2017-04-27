Predict insurance fraud(팀프로젝트)

team project in data science school (방승환, 오학, 이승수, 정준모)

-목표

보험금 지급 정보를 바탕으로 보험급 지급 전에 사기확률을 예측한다.

-데이터 수집

OO생명의 10년간의 분석대회용 데이터

-분석

도메인지식을 바탕으로 관련있을 것 같은 category값 20개와 numeric값 17개를 선정

target값을 '보험 사기자 여부'로 놓고 시행

heatmap과 pairplot을 그려 분포를 알아보고 변수들이 독립인지 구분

category값은 다변량, numeric값은 가우시안나이브베이지안으로 시행

의사결정나무를 통해 변수결정

roc커브를 통하여 모형비교

-한계점

데이터자체에 결측값이 너무 많아서 임의로 mean값 등을 넣어주다보니 데이터가 좋지 않았다


Medical Appointment No Shows(개인 프로젝트)

-목표

환자들의 정보를 바탕으로 다음 내원 때 오지 않을 환자를 예측

-데이터

Kaggle Data

-분석

필요없는 column을 제거해주고 문자를 숫자로 음수값을 양수값으로 바꿔주는 전처리 시행

heatmap과 pairplot을 이용해 분포와 변수들의 상관관계를 알아보았다

변수들의 중요도를 알아보기 위해 랜덤포레스트를 이용하여 모든 노드에 IG를 비교하여 변수의 중요도를 알아보았다

역시나 나이와 시간이 압도적으로 관계가 있는 것을 알 수 있었다

그리고 LogisticRegression 과 RandomForest 모형을 돌려보았다

LogisticRegression 을 실행한 결과 
Train Score : 0.696736318408 Test Score : 0.698141414141 auc : 0.56207855268257911 
RandomForest 를 실행한 결과 
Train Score : 0.811084577114 Test Score : 0.639262626263 auc : 0.69673631840796024

RandomForest가 조금 높게 나왔지만 만족할만한 수치는 나오지 않았다

조금 더 스케일링이 필요한 것 
