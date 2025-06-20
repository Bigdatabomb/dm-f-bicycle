# 프로젝트: 서울시 따릉이 이용 패턴 및 예측 모델을 통한 입지 평가
이 저장소에는 따릉이 수요 예측 및 입지 분석에 필요한 변수들의 전처리 데이터셋, 시각화, 모델 학습 및 최적화를 위한 Jupyter 노트북이 포함되어 있습니다. 사용한 데이터(에: 열린데이터광장) 파일은 용량이 크므로 아래 Google Drive 링크에서 다운로드하여 사용하세요.

---

## 📁 디렉토리 구조

```
/                # 프로젝트 루트
├─ notebooks/    # Jupyter 노트북
│   ├─ data preprocessing.ipynb                           # 데이터 전처리
|   ├─ data_visualization.ipynb                           # 데이터 시각화
|   ├─ model_training.ipynb                               # 모델 학습 및 최적화
|   └─ bicycle_rental_n_return
|      └─month_merge.ipynb                                # 일일 사용량을 월별로 합산 및 전처리
|      └─data_conversion_for_month_merge.ipynb            # month_merge에 사용할 main 파일 생성
└─ README.md     # 이 파일
```
---

## 📁 사용 데이터셋

24년도 1월부터 12월까지의 따릉이 대여소 이용 기록에 관한 데이터는 구글 드라이브에 zip파일로 업로드 하였습니다.
- [2024년 따릉이 데이터](https://drive.google.com/uc?export=download&id=1WltLqTxbn-VHw8ki3tn-yQn1B-mpHn2R)
해당 zip 파일은 bicycle_rental_n_return 안에서 압축해제 하여야 합니다.
- zip 파일 속 csv 파일들은 정확히 bicycle_rental_n_return 폴더 안에 있어야 하며, 다른 폴더 안에 있으면 오류가 생깁니다.
- 24년 11월 27일 데이터의 경우 누락되어 삭제하였습니다.

-**bike_accident_data.csv**
자전거 사고 현황에 관한 데이터

-**bike_lane_data.csv**
자전거 도로 정보에 관한 데이터

-**bike_rental_master.csv**
따릉이 대여소에 대한 마스터 데이터

-**bike_shed_location.csv**
자전거 보관소 위치에 관한 데이터

-**bus_stop_location.csv**
버스 정류장 위치에 관한 데이터

-**college_data.csv**
대학교 위치에 관한 데이터

-**crossroad_data.csv**
교차로 위치에 관한 데이터

-**dong_data.csv**
대여소id별로 해당하는 주소지의 '동'을 합산한 데이터

-**diner_location_data.csv**
휴계음식점 위치에 관한 데이터

-**high_school_data.csv**
고등학교 위치에 관한 데이터

-**subway_station_location.csv**
지하철역 위치에 관한 데이터

-**tourist_attraction_location.csv**
관광지 위치에 관한 데이터

-**2024 Rain Data.csv**
24년도 강수량 데이터

---

## 📝 노트북 설명

-**data preprocessing.ipynb**
여러 출처(예:열린데이터광장)에서 수집한 데이터를 통합, 분석 및 예측을 위한 맞춤형 변수 생성, 결측치 처리 및 형식 정리하여 전처리한 데이터 셋.

-**data_visualization.ipynb**
전처리한 데이터셋을 사용하여 월별 사용량 추이, 총_사용인원 기준 변수 상관관계 파악, 랜덤포레스트 기반 변수 중요도 파악, 변수 중요도 기반 입지 평가하여 folium함. 이를 통해 인사이트를 추출함.

-**model_training.ipynb**
Linear Regression, RandomForest Regressgion, XGBoost Regression, Lasso Regresssion, Ridge Regression, ElasticNet, KNN Regression 모델 간 학습 비교를 통해 최적의 모델 선정함.


- 참고사항
kakao api를 사용한 코드의 경우, 학생 개인의 api 키가 노출되어 보안상의 문제로 포함하지 않았습니다.
또한, geopy를 사용한 코드의 경우, 오류나 블록되는 경우가 너무 많이 발생하여 kakao api를 사용하는 코드로 모두 변경하였습니다.

---

## ⚙️ 실행 환경 및 주요 라이브러리
tfenv(Python 3.10.16)


---
