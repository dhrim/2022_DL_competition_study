# 3회차 - ML(머신러닝)으로


# 미션
## 1단계 - 데이터 로딩

- https://www.kaggle.com/competitions/tabular-playground-series-apr-2022 데이터를
    - colab으로 가져와 train.csv, train_labels.csv, test.csv를 pandas로 로딩하고
    - 각 파일을 pandas로 로딩

<br>

## 2단계 - x, y 데이터 준비

- 데이터는 다음과 같이 구성됨.
    - 13개의 센서가 있고, 투수의 공을 연속으로 60번 센싱함
    - sequence 컬럼이 데이터 id에 해당함. step이 60번 촬영중에 몇번째인지에 해당함
- 데이터를 다음과 같이 변환하여 x데이터 생성
    - pandas로 읽은 train.csv 데이터를 numpy로 변환
    - 원 데이터 60(60 스텝)x16(sequence, subject, step 하고 센서 13개)의 데이터를 1x780 데이터로 변환
    - 780은 60x13에 해당하고, sequence, subject, step은 포함하지 않음.
    - 위의 변환을 총 25,968개의 train 데이터에 대하여 전부 실행. train_x
    - 그리고 같은 수의 train_labels.csv를 state값을 train_y에 numpy로 담음.

<br>

## 3단계 - ML 실행

- 다음 자료를 참고로 ML 방법들을 적용
    - [material/deep_learning/ML_classifiers.ipynb](material/deep_learning/ML_classifiers.ipynb)


# ML에 대하여
n개의 속성으로 이루어진 x 데이터를 m개의 값으로 출력하는 작업을 분류(classification)이라함.

지금 다루는 문제는 780개 속성의 입력 데이터를 2개의 값으로 출력하는 전형적인 분류 문제임.


이외에 다양한 실수값을 출력하는 회귀(regression)과 군집화(clustering)작업이 있음.



