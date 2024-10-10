# machine_learning
- 범주형 데이터 분류에서 어떤 모델이 적합한지를 테스트
- Anaconda 가상환경을 이용하여 jupyter notebook으로 학습 및 테스트 진행
- 의사결정나무(Decision Tree), 랜덤포레스트(Random Forest), XGBoost를 이용하여 학습/결과값 예측 비교
- 타이타닉 생존자 분류에서 어떤 알고리즘이 가장 효율적인지를 비교
- numpy, pandas, matplot, seaborn, 라이브러리 사용
- 데이터 전처리
  - 생존과 관련 있는 컬럼만 탐색하고 상관관계를 파악
  - 생존과 관련 있는 컬럼을 새로 생성(예: 가족수, 성별+나이)
  - 생존과 관련이 없거나 결측치가 대부분인 컬럼, 한가지 값이 대부분인 컬럼을 삭제
  - 결측값을 컬럼의 평균값으로 치환
  - 범주형 데이터 처리를 위해 문자가 저장된 컬럼을 숫자로 변환 

## 의사결정나무(Decision Tree)
- 지니 지수 계산식을 이용하여 어떤 속성으로 분류했을 때 지니지수가 가장 낮은지를 계산
- 의사결정나무를 시각화하는 Graphviz 사용
- sklearn, numpy, pandas, pydotplus 라이브러리 사용

## 랜덤포레스트(Random Forest)
- 여러 개의 의사결정나무를 결합한 형태로 Over-fitting 문제가 적고 구현이 간단하며 병렬 계산이 간편
- Dataset에서 샘플 데이터를 random으로 선택하여 decision tree를 생성
- Iris 데이터를 이용하여 간단한 Random Forest 구현
- numpy, pandas, sklearn 라이브러리 사용

## XGBoost
- learning rate를 적용하여 기존 예측값 업데이트
- 위스콘신 유방암 데이터를 이용하여 간단한 XGBoost 구현
- pandas, numpy, sklearn 라이브러리 사용
