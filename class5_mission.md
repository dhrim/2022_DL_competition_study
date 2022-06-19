# 5회차 - 대회 출품


# 미션


## 1단계 - 결과물 예측

- test.csv를 pandas로 읽음
- 읽은 것에 train.csv에 사용된 것과 동일한 전처리 적용
- 학습된 모델에 적용하여 예측값 구하기
- 구한 예측값을 0.5를 기준으로 0과 1로 만들기


<br>

## 2단계 - 결과물 만들기

- sample_submission.csv를 읽기
- sample_submission data_frame의 state 컬럼의 값을 1단계에서 예측한 값으로 변경
- submission.csv 파일 이름으로 저장.
- 라인수는 sample_submission과 동일한 12,219 이어야 함.


<br>

## 3단계 - 결과물 출품

- 2단계에서 생성한 submission.csv를 로칼 컴퓨터로 다운로드
- https://www.kaggle.com/competitions/tabular-playground-series-apr-2022 페이지를 열고
- 'Late Submission' 클릭
- submission.csv를 업로드
- 'Make Submission' 클릭
- 스코어 확인.


<br>

## 4단계 - 성능 개선

- 참고 자료 : 
    - 오버피팅 처리 : material/deep_learning/dnn_in_keras_overfitting.ipynb
    - Early Stopping : material/deep_learning/dnn_in_keras_callback.ipynb

- 이상치 처리
    - 이상치 처리 안된경우 이상치 처리
    - 1~3단계를 반복

- Batch Normalization
    - 코드에 Batch Normalization을 적용.
    - 1~3단계를 반복

- Drop Out
    - 코드에 Drop Out을 추가 적용
    - 1~3단계를 반복

- Regularization
    - 코드에 Regularization을 추가 적용
    - 1~3단계를 반복

- Early Stopping
    - 코드에 Early Stopping을 추가 적용
    - 1~3단계를 반복

- (optional) 기타
    - 모델 사이즈 조정
    - 다른 모델 사용