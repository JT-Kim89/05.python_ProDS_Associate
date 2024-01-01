## part 1 데이터 전처리
01차시 프로그램 소개 및 설치  
 - Anaconda 설치  
 - Jupyter Notebook 실행  

02차시 기본 문법1: 연산자, 숫자/문자, 리스트, 튜플, 딕셔너리  
 - Python basic(list, tuple, dictionary)  

03차시 기본 문법2: 제어문, 라이브러리
 - Python basic(if, for, def)  

04차시 EDA: 수치형, 범주형 기술통계  
 - Numpy basic(array, ones, zeros, empty, eye, identity)  
 - Pandas basic(Series, DataFrame)
 - df.groupby

05차시 데이터 전처리: 결측치, 이상치  
 - 결측치: df.isna, isnull  
 - 결측치 채우기: df.fillna  
 - 결측치 제거: df.dropna  
 - 분위수: df.quantile

06차시 데이터 전처리: 파생변수 생성  
 - 조건출력: np.where  
 - 변수명 변경: pd.rename  
 - 행 또는 열 function 계산: pd.apply  
 - 속성 변경: pd.astype  
 - 가변수 생성: pd.get_dummies  

07차시 데이터 전처리: 데이터 병합  
 - 인덱스 초기화: dt.reset_index  
 - 특정 변수를 인덱스로 지정: df.set_index  
 - 데이터 단순병합: pd.concat  
 - 데이터 키(key) 병합: pd.merge

08차시 데이터 전처리: 정렬 및 변환  
 - 빈도 확인: pd.crosstab  
 - 정렬: df.sort_values  
 - 자료 구조변환(long form): df.melt  
 - 자료 구조변환(wide form): df.pivot  


## part 2 통계

09차시 모평균 비교에 관한 가설검정: t-test  
 - 단일 표본 t-검정: scipy.stats ttest_1samp 
 - 대응 표본 t-검정: scipy.stats ttest_rel
 - 독립 2 표본 t-검정: scipy.stats ttest_ind  

※ 아래 사이트에서 p-value, 검정통계량 이해하기  
 - https://huidea.tistory.com/233
 - https://www.youtube.com/watch?v=tpow70KGTYY  (~32분까지)

 - 가설검정: 모집단을 알 수 없을 때, 표본집단을 이용하여 모집단을 추정하는 것 (표본으로 보아 전체는 이럴 것이다.)  
 - 귀무가설: 모집단의 평균은 10 일 것이다. 
 - p-value: probability, 0 ~ 1 사이 값, 귀무가설이 맞으면 1에 가까워 짐 (통상 0.1 보다 커야 맞다고 볼 수 있음)  
 - 검정통계량: 샘플값(샘플의 평균값) - 귀무가설값(평균10), 귀무가설값에 가까워지면 검정통계량은 0에 가까워 짐

10차시 모평균 비교에 관한 가설검정: One way ANOVA(분산 분석, analysis of variance)  
 - 일원 분산 분석: scipy.stats f_oneway
 - 일원 분산 분석: statsmodels ols
 - 일원 분산 분석: statsmodels anova_lm
 - 사후검정: statsmodels pairwise_tukeyhsd

11차시 모분산 비교에 관한 가설검정: 등분산 검정(F-test of equality of variances)  
 - F-검정: scipy.stats f.cdf
 - Bartlett 검정: scipy.stats bartlett
 - Leneve 검정: scipy.stats levene

12차시 범주형 변수 간의 독립성 검정(Chi-squared test)  
 - 카이제곱 검정: scipy.stats chi2_contingency

13차시 상관분석  
 - 상관분석: pandas corr
 - Pearsono 상관분석: scipy.stats pearsonr
 - Spearman 상관분석: scipy.stats spearmanr
 - Kendall 상관분석: scipy.stats kendalltau

## part 3 분석

14차시 단순 회귀분석(Simple Linear Regression)  
 - 선형회귀분석: statsmodels.formula.api ols
 - 선형회귀분석: sklearn.linear_model LinearRegression
 - MAE(Mean Absolute Error): sklearn.metrics mean_absolute_error
 - RMSE(Root Mean Squared Error): sklearn.metrics mean_squared_error

15차시 다중 회귀분석(Multiple Linear Regression)  
 - 전처리: pasty dmatrices
 - 분산 팽창 계수(VIF): statsmodels.stats.outliers_influence variance_inflation_factor

16차시 분류: 로지스틱 회귀분석(Logistic Regression)  
 - 로지스틱 회귀분석: statsmodels.api Logit
 - 로지스틱 회귀분석: sklearn.linear_model LogisticRegression
 - AUC(Area Under Curve): sklearn.metrics roc_auc_score
 - 정확도: sklearn.metrics accuracy_score
 - f1: sklearn.metrics f1_score
 - 정밀도: sklearn.metrics precision_score
 - 재현율: sklearn.metrics recall_score

17차시 의사결정나무 모델: 분류 및 회귀나무  
 - 분류 나무(명목형 종속변수): sklearn.tree DecisionTreeClassifier
 - 회귀 나무(연속형 종속변수): sklearn.tree DecisionTreeRegressor


