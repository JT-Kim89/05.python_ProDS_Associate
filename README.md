## 05.python_ProDS_Associate

### 01차시 프로그램 소개 및 설치  
Anaconda  
Jupyter Notebook  

### 02차시 기본 문법 1  
Python basic

### 03차시 기본 문법 2
Python basic

### 04차시 EDA: 수치형, 범주형 기술통계  
Numpy basic  
Pandas basic

### 05차시 데이터 전처리: 결측치, 이상치  
<pandas>
- df.isna  
- df.fillna  
- df.dropna  
- df.quantile

### 06차시 데이터 전처리: 파생변수 생성  
<numpy>
- np.where  
<pandas>
- pd.rename  
- pd.apply  
- pd.astype  
- pd.get_dummies

### 07차시 데이터 전처리: 데이터 병합  
<pandas>
- dt.reset_index  
- df.set_index  
- pd.concat  
- pd.merge

### 08차시 데이터 전처리: 정렬 및 변환  
<pandas>
- pd.crosstab  
- df.sort_values  
- df.melt  
- df.pivot  

### 09차시 모평균 비교에 관한 가설검정: t-test  
<scipy.stats>
- ttest_1samp 
- ttest_rel
- ttest_ind  

아래 사이트에서 p-value, 검정통계량 이해하기  
https://huidea.tistory.com/233
https://www.youtube.com/watch?v=tpow70KGTYY  (~32분까지)

- 가설검정: 모집단을 알 수 없을 때, 표본집단을 이용하여 모집단을 추정하는 것 (표본으로 보아 전체는 이럴 것이다.)  
- 귀무가설: 모집단의 평균은 10 일 것이다. 
- p-value: probability, 0 ~ 1 사이 값, 귀무가설이 맞으면 1에 가까워 짐 (통상 0.1 보다 커야 맞다고 볼 수 있음)
- 검정통계량: 샘플값(샘플의 평균값) - 귀무가설값(평균10), 귀무가설값에 가까워지면 검정통계량은 0에 가까워 짐

### 10차시 모평균 비교에 관한 가설검정: One way ANOVA  
<scipy.stats>
- f_oneway
<statsmodels>
- ols
- anova_lm
- pairwise_tukeyhsd


### 11차시 모분산 비교에 관한 가설검정: 등분산 검정(F-test of equality of variances)  

### 12차시 범주형 변수 간의 독립성 검정(Chi-squared test)  

### 13차시 상관분석  

### 14차시 단순 회귀분석(Simple Linear Regression)  

### 15차시 다중 회귀분석(Multiple Linear Regression)  

### 16차시 분류: 로지스틱 회귀분석(Logistic Regression)  

### 17차시 의사결정나무 모델: 분류 및 회귀나무  

