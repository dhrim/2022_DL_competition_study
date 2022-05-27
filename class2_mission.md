# 2회차 - 데이터 전처리, 시각화

- 데이터 전처리 : 결측치, 이상치, 코드성 데이터 인코딩, 정규화
- pandas로 데이터 전처리
- numpy로 데이터 전처리
- 데이터 시각화 : histogram, image 그리기, 선 그래프 그리기

<br>

# 미션
## 1단계 - pandas로 데이터 전처리 : 결측치 처리, 이상치 처리, 코드성 데이터 인코딩, 정규화

- https://github.com/dhrim/2022_DL_competition_study/blob/master/material/data/iris.csv 데이터를
    - pandas로 로딩
    - 정규화
- https://github.com/dhrim/2022_DL_competition_study/blob/master/material/data/flawed_iris.csv 데이터를 
    - pandas로 로딩
    - 이상치 처리
    - 결측치 처리
    - 코드성 데이터를 인코딩
    - 정규화

<br>

## 2단계 - 데이터 시각화 : histogram, image 그리기, 선 그래프 그리기

- https://github.com/dhrim/2022_DL_competition_study/blob/master/material/data/iris.csv 데이터를
    - pandas로 로딩
    - numpy로 데이터 받고
    - septal_width, septal_height, petal_width, petal_height 컬럼의 histogram 그리기
    - septal_width를 가로축으로 septal_height를 세로축으로 2차원 공간에 점 찍기.
- https://github.com/dhrim/2022_DL_competition_study/blob/master/material/data/flowers.zip 데이터를
    - 다운받아 
    - google drive에 올리고
    - colab에서 google drive를 마운트해서 카피해 오고
    - 압축풀고
    - 영상 파일 전체에 대하여 matplotlib의 imread()로 로딩하고
    - 이미지 1개 출력
    - 이미지 8개를 4x2로 격자로 출력

<br>

## 3단계 - 실 데이터 EDA

- https://www.kaggle.com/competitions/tabular-playground-series-apr-2022 데이터를
    - 다운 받고
    - google drive에 올리고
    - colab에서 google drive를 마운트해서 카피해 오고
    - train.csv를 pandas로 로딩
    - 컬럼 subject, step, sensor_00, sensor_01, ..., sensor_07의 histogram을 그리고
    - sensor_xx의 이상치를 처리
