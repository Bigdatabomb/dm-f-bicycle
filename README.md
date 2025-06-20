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

데이터 파일은 Google Drive에 업로드되어 있습니다. 다운로드 후 프로젝트 루트에 data/ 폴더를 만들어 넣어주세요. 이후 파일 경로에 대한 설정 또한 필요합니다.
- [2024년 1월 따릉이](https://drive.google.com/uc?export=download&id=1WltLqTxbn-VHw8ki3tn-yQn1B-mpHn2R)
- [2024년 4월 따릉이](https://drive.google.com/uc?export=download&id=1bPJAzrorcrNFqMMahGvEAvIJAbzgO_u5)
- [2024년 따릉이 하반기](https://drive.google.com/uc?export=download&id=1Jx9UudV0TC2Syg1Aiy4g1LXuGfR1MHb-)

---

## 📝 노트북 설명

-**data preprocessing.ipynb**
여러 출처(예:열린데이터광장)에서 수집한 데이터를 통합, 분석 및 예측을 위한 맞춤형 변수 생성, 결측치 처리 및 형식 정리하여 전처리한 데이터 셋.

-**data_visualization.ipynb**
전처리한 데이터셋을 사용하여 월별 사용량 추이, 총_사용인원 기준 변수 상관관계 파악, 랜덤포레스트 기반 변수 중요도 파악, 변수 중요도 기반 입지 평가하여 folium함. 이를 통해 인사이트를 추출함.

-**model_training.ipynb**
Linear Regression, RandomForest Regressgion, XGBoost Regression, Lasso Regresssion, Ridge Regression, ElasticNet, KNN Regression 모델 간 학습 비교를 통해 최적의 모델 선정함.

---

## ⚙️ 실행 환경 및 주요 라이브러리

---
