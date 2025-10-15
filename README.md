# 심장질환 예측 프로젝트
이 저장소는 심장질환(Framingham Heart Study) 데이터를 활용해 다양한 지도 학습 기법을 적용하고, 데이터 전처리, 모델링 및 성능 평가 과정을 다룹니다.

## 파일 구성
- 심장병_예측_SupervisedClassification.ipynb
심장질환 데이터셋에 대해 지도 분류(Classification) 분석을 진행하는 노트북입니다. 로지스틱 회귀, 랜덤 포레스트, XGBoost 등 다양한 모델을 적용하며, 성능 평가, 변수 중요도 분석, 각종 전처리(결측값 처리, 이상치 처리, 스케일링 등)를 포함합니다

- 심장병_예측_디벨롭.ipynb
지도 분류 이외에도 군집화(K-means), 차원 축소(PCA), 메타 모델(스태킹 등)과 같은 고급 기법들을 분석합니다. 다양한 머신러닝 라이브러리와 예측 설명(Feature Importance, Odds Ratio 등) 내용을 포함한 종합 데이터 분석 노트북입니다.

- Classification_HeartDisease.csv
Framingham 심장질환 예측용 원본 데이터셋(CSV). 주요 컬럼은 다음과 같습니다:

  male: 성별(1=남, 0=여)
  
  age: 연령
  
  education: 교육 수준(1~4)
  
  currentSmoker: 현재 흡연 여부
  
  cigsPerDay: 하루 평균 흡연 개수
  
  BPMeds: 혈압약 복용 여부
  
  prevalentStroke, prevalentHyp, diabetes: 기저질환 유무
  
  totChol, sysBP, diaBP, BMI, heartRate, glucose: 주요 임상지표
  
  TenYearCHD: 10년 내 심장질환 발생 여부 타겟(0=No, 1=Yes)
