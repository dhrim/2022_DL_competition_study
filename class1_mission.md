# 1회차 - 기반 환경과 데이터 준비, 로딩

- colab or kaggle vm
- linux command
- 다양한 소스(kaggle, http, github, db, google drive, AWS S3)
- 다양한 포멧(zip, tar, npy, csv, xlx)

<br>

# 미션

## 1단계 - colab과 kaggle VM 접속
- colab에 접속하여 설치된 tensorflow, numpy, pandas, matplotlib 버전 출력해 보기.
- kaggle에서 VM을 생성하고 tensorflow, numpy, pandas, matplotlib 버전 출력해 보기.
- (optional) AWS SageMaker 서비스 신청하고 설치된 VM에서 tensorflow, numpy, pandas, matplotlib 버전 출력해 보기.
- (optional) 사용자 컴에 환경 설정하고 tensorflow, numpy, pandas, matplotlib 버전 출력해 보기.

<br>

## 2단계 - 데이터 가져오기
- colab
    - direct upolad
        - from normal web : https://forge.scilab.org/index.php/p/rdataset/source/file/master/csv/datasets/iris.csv 를 사용자 컴으로 다운받고 colab에 직접 업로드하여 pandas로 로딩하기.
        - kaggle data : https://www.kaggle.com/datasets/uciml/iris 의 iris.csv 파일을 사용자 컴으로 다운받고 colab에 직접 업로드하여 pandas로 로딩하기.
    - google drive : https://forge.scilab.org/index.php/p/rdataset/source/file/master/csv/datasets/iris.csv 를 사용자 컴으로 다운받아 google drive에 올리고 colab에서 drive를 마운트해서 colab에서 pandas로 로딩하기.
    - http by wget
        - from normal web : https://forge.scilab.org/index.php/p/rdataset/source/file/master/csv/datasets/iris.csv 를 colab에서 wget으로 직접 다운받고 pandas로 로딩하기.
        - from github : https://github.com/dhrim/2022_DL_competition_study/blob/master/material/deep_learning/iris.csv 를 colab에서 wget으로 직접 다운받고 pandas로 로딩하기.
        - image data : http://beltlineorg-wpengine.netdna-ssl.com/wp-content/uploads/2012/12/IMG_5669-flickr-websized.jpg 를 colab에서 wget으로 직접 다운받고 matplot으로 이미지 보기
    - google drive :
    https://drive.google.com/file/d/1_l-0FUDU1EovwlhnILnrrC0labjWtgCJ/view?usp=sharing 를 gdown(따로 설치한)으로 colab에서 직접 다운받고 matplot으로 이미지 보기

- kaggle VM
    - kaggle data : kaggle VM을 만들고 https://www.kaggle.com/competitions/titanic/data 의 train.csv 데이터를 kaggle VM에서 pandas로 로딩하기.
    - http by wget
        - from normal web : https://forge.scilab.org/index.php/p/rdataset/source/file/master/csv/datasets/iris.csv 를 kaggle VM에서 wget으로 직접 다운받고 pandas로 로딩하기.
        - from github : https://github.com/dhrim/2022_DL_competition_study/blob/master/material/deep_learning/iris.csv 를 kaggle VM에서 wget으로 직접 다운받고 pandas로 로딩하기.
        - image data : http://beltlineorg-wpengine.netdna-ssl.com/wp-content/uploads/2012/12/IMG_5669-flickr-websized.jpg 를 kaggle VM에서 wget으로 직접 다운받고 matplot으로 이미지 보기

<br>        

## 3단계 - 다양한 포멧
- https://github.com/dhrim/2022_DL_competition_study/raw/master/material/deep_learning/dogs_prepared.tar.gz 를 가져와서 압축풀고 matplotlib로 이미지 보기
- xxx의 xxx.tar를 가져와서 압축 풀고 pandas로 로딩하기.
- xxx의 xxx.zip을 가져와서 압축 풀고 pandas로 로딩하기.
- xxx의 xxx.npy를 가져와서 numpy로 로딩하기.
- xxx의 xxx.xlsx를 가져와서 pandas로 로딩하기.
- xxx의 xxx.csv를 가져와서 pandas로 로딩하기.
- xxx의 xxx.pickle을 가져와서 pickle로 로딩하기.

<br>

## 4단계 - linux 커멘드
- 현재 폴더의 위치를 출력
- 현재 폴더안의 파일과 폴더 리스트를 출력
- 현재 폴더에 sub1이라는 하위 폴더 생성, sub2라는 하위 폴더 생성.
- 현재 폴더 안의 파일 이름 변경
- 현재 폴더안의 파일을 sub1이라는 하위 폴더아래로 이동
- sub1아래의 파일을 현재 폴더로 이동
- sub1 아래의 파일을 sub2 아래로 이동
- tree 명령어 설치

<br>

# 참고 자료
- linux and library
    - linux command : https://github.com/dhrim/2022_DL_competition_study/blob/master/material/linux.md
    - numpy : https://github.com/dhrim/2022_DL_competition_study/blob/master/material/library/numpy_for_deep_learning.ipynb
    - pandas : https://github.com/dhrim/2022_DL_competition_study/blob/master/material/library/pandas_for_deep_learning.ipynb
    - matplotlib : https://github.com/dhrim/2022_DL_competition_study/blob/master/material/library/matplot_for_deep_learning.ipynb
- data download and loading example
    - google drive, csv, zip, pandas : https://github.com/dhrim/2022_DL_competition_study/blob/master/material/deep_learning/face_emotion_classification.ipynb
    - http by wget : https://github.com/dhrim/2022_DL_competition_study/blob/master/material/library/pandas_for_deep_learning.ipynb
- image dataload and view by matplotlib : https://github.com/dhrim/2022_DL_competition_study/blob/master/material/deep_learning/object_detection_yolo_keras.old.ipynb
- install gdown, download with gdown : https://github.com/dhrim/2022_DL_competition_study/blob/master/material/deep_learning/cat_with_glasses.ipynb