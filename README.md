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




