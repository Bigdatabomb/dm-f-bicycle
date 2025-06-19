# 프로젝트: 서울시 따릉이 수요 예측 및 입지 분석
이 저장소에는 따릉이 수요 예측 및 입지 분석에 필요한 변수들의 데이터셋(열린광장데이터, 프로젝트 맞춤형 변환 데이터), 시각화 및 분석, 모델 학습을 위한 Jupyter 노트북이 포함되어 있습니다. 데이터 파일은 용량이 크므로 아래 Goolge Drive 링크에서 다운로드하여 사용하세요.

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

## 📝 노트북 설명

-**data preprocessing.ipynb**

-**data_visualization.ipynb**
전처리한 데이터셋을 사용하여 월별 사용량 추이, 총_사용인원 기준 변수 상관관계 파악, 랜덤포레스트 기반 변수 중요도 파악, 변수 중요도 기반 입지 평가하여 folium함. 이를 통해 인사이트를 추출함.

-**model_traingin.ipynb**

---

## ⚙️ 실행 환경 및 주요 라이브러리

---
