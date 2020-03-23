# How Much Fish
2019년 4학년 1학기 TeamProject2 
Youtube: https://www.youtube.com/watch?v=-EsIAYE_Xiw

# WHY? 
우리나라는 세계수산물 소비 1위국가인데 농산물에 비하여 수산물은 뚜렷한 4차산업혁명과의 결합이 없었습니다. 이에 대한 관심은 적었고 폭등하는 수산물 가격에 정부의 많은 예산이 소비되는 것을 확인하였습니다.
이에 하나의 대시보드로서 가격을 예측하여 대비하고 안정화 한다면 새로운 플랫폼이 될 것이라 생각하였습니다.

# HOW?
데이터 수집에 있어서는 농수산물유통정보 기상청 합쳐서 데이터를 만듬 csv 파일로만들고
이를 텐서플로우에서 넘파이를 사용하여 플레이스 홀더를 각각 설정. 선형회귀를 사용했는데
경사하강법으로 이를 예측  hypothesis = tf.matmul(X,W) +b
Cost = tf.reduce_mean(tf.square(hypothesis - Y)
평균제곱 오차법 
optimizer = tf.train.GradientDescentOptimizer(learning_rate=0.000005)
* 선형 회귀란? 독립 변수 x를 사용해 종속 변수 y의 움직임을  예측 하는 방식
1. Initial Screen
- Flask Web + BootStrap Template을 활용하여 Video 클립을 활용한 빠른 웹 디자인 개발
<img width="1678" alt="스크린샷 2020-03-23 오후 4 36 30" src="https://user-images.githubusercontent.com/62536330/77292895-8d97af80-6d24-11ea-9e5f-7d53721744fc.png">


2. Prolouge
- 고령화 및 수질오염으로 인한 솟구치는 수산물 가격 변동에 따른 프로젝트의 필요성을 인지
- 아직 수산물 관련 데이터 활용 프로젝트 부족 (일본 및 미국에서는 도입 단계)
<img width="1680" alt="스크린샷 2020-03-23 오후 4 32 10" src="https://user-images.githubusercontent.com/62536330/77292632-077b6900-6d24-11ea-8049-e2efdc3f4ac9.png">

3. Analysis & Model
- Kibana를 활용한 시각화 , Tensorflow를 활용한 시각화를 통하여 데이터 분석
- 강수량은 수치화 하여 표현 선형회귀를 통한 예측모델 구성
<img width="823" alt="스크린샷 2020-03-23 오후 4 38 12" src="https://user-images.githubusercontent.com/62536330/77293094-fb43db80-6d24-11ea-8cf9-636ce44ff2f9.png">
<img width="1248" alt="스크린샷 2020-03-23 오후 4 37 31" src="https://user-images.githubusercontent.com/62536330/77293097-fd0d9f00-6d24-11ea-8d10-e372ea294805.png">
<img width="1205" alt="스크린샷 2020-03-23 오후 4 40 25" src="https://user-images.githubusercontent.com/62536330/77293116-05fe7080-6d25-11ea-92db-2f4c7faac6bc.png">

4. Article & Contact
- 네이버 뉴스 검색API를 사용하였습니다. '수산물'이라는 키워드로 얻은 결과를 JSON파일로 만들어서 다음과 같이 주요 뉴스를 선정 하였습니다.
- Gmail API를 활용하여 contact를 통해 불편사항 접수
<img width="1651" alt="스크린샷 2020-03-23 오후 4 41 54" src="https://user-images.githubusercontent.com/62536330/77293255-4bbb3900-6d25-11ea-8521-21ee2b0ac41c.png">
<img width="1664" alt="스크린샷 2020-03-23 오후 4 42 01" src="https://user-images.githubusercontent.com/62536330/77293266-537add80-6d25-11ea-9042-0a246e98a5dc.png">
