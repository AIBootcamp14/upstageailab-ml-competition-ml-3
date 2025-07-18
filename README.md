# 🏡 채린이네 | 부동산 가격 예측 경진대회

> 최대한 많이 넘어져 보자

---

## 🧑‍💻 Team Members

| <img src="https://avatars.githubusercontent.com/u/213385368?v=4" width="150" style="border-radius:50%;"> | <img src="https://avatars.githubusercontent.com/u/66048976?v=4" width="150" style="border-radius:50%;">  | <img src="https://avatars.githubusercontent.com/u/162023876?v=4" width="150" style="border-radius:50%;"> | <img src="https://avatars.githubusercontent.com/u/213417897?v=4" width="150" style="border-radius:50%;"> | <img src="https://avatars.githubusercontent.com/u/213385147?v=4" width="150" style="border-radius:50%;"> |
| :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: |
|            [문채린](https://github.com/CHAERINMOON)             |            [박재홍](https://github.com/woghd8503)             |            [김상윤](https://github.com/94KSY)             |            [김동준](https://github.com/rafiki3816)             |            [정서우](https://github.com/Seowoo-C)             |
|                            팀장, 데이터 전처리 및 모델링                             |                            개발 환경 세팅                             |                            데이터 전처리 및 모델링                             |                            데이터 전처리 및 모델링                             |                            데이터 전처리 및 모델링                             |
> **협업 철학:**  
> “배워서 남주자”, “모든 질문은 가치가 있다”, “모든 새로운 시도는 가치가 있다”  
> 매일 오전 10시 미팅, 오후 2시 집중 회의 진행.

## 📅 Competition Info

- **주제:** 서울시 아파트 실거래가 예측 (House Price Prediction)
- **기간:**  
  - 07.07 ~ 07.09: Git/서버 세팅  
  - 07.10 ~ 07.11: 데이터 전처리  
  - 07.14 ~ 07.17: 모델 학습 및 실험
- **목표:**  
  - 모델 성능보다는 다양한 시도와 인사이트 확보  
  - 개인별 리더보드 2회 업로드 필수
- **평가지표:** RMSE (Root Mean Squared Error)

---

## 🗂️ Directory Structure
```
project/
├── notebooks/ # 주피터 노트북 작업 공간
│ ├── user1/ # 개인 작업 공간
│ ├── user2/
│ ├── user3/
│ ├── user4/
│ └── user5/
│
├── data/ # 공유 데이터
│ ├── raw/ # 원본 데이터
│ ├── processed/ # 전처리된 데이터
│ └── external/ # 외부 데이터
│
├── src/ # 소스 코드
│ ├── data/ # 데이터 처리
│ ├── features/ # 피처 엔지니어링
│ ├── models/ # 모델 정의
│ └── utils/ # 유틸리티 함수
│
├── experiments/ # 실험 결과 저장
├── models/ # 학습된 모델 저장
├── .gitignore
├── environment.yml
└── requirements.txt
```



---

## ⚙️ Environment Setup

### Conda
```bash
conda env create -f environment.yml
conda activate real_estate_pred
```
### pip
```bash
python -m venv venv
# Windows
.\venv\Scripts\activate
# Linux/Mac
source venv/bin/activate

pip install -r requirements.txt
```
## 📊 Data Description

### Overview
서울시 아파트 실거래 데이터를 기반으로 한 매매가격 예측 문제

### EDA
- 결측치 100만개 이상 제거
- 연속형/범주형 변수 분리 및 보간
- 좌표 기반 외부데이터 활용
- 이상치 제거: IQR 방식

---

## 🛠️ Feature Engineering

- 지하철 역 수 (800m 반경)
- 버스 정류장 수
- 교통 인프라 총합 (버스+지하철)
- 프리미엄 지역 여부 (강남3구+용산구)
- 거래연도 구간화 (코로나/금리 영향 구간)
- 한강 뷰 거리 + 층수 조합 점수
- `target` log 변환

---

## 🤖 Modeling

### 사용 모델 및 RMSE

| Model             | RMSE       |
|------------------|------------|
| RandomForest      | **4672.44** |
| XGBoost           | 8620.20    |
| LinearRegression  | 23694.44   |
| Ridge             | 23694.45   |

- 주요 실험 결과: `RandomForest` 기반이 가장 안정적
- Trial 1~3 순차적 개선, 구간별 모델링 수행

---

## 📈 Result

- **최종 리더보드 RMSE:** `77060`

### 목표성취률 (Self Check)
| 이름     | 목표성취률 |
|--------|--------|
| 문채린 | 60%    |
| 박재홍 | 60%    |
| 김상윤 | 70%    |
| 김동준 | 60%    |
| 정서우 | 80%    |

---

## 🗣️ Retrospective

### 잘한 점
- 꾸준한 회의 및 정보 공유 → 공통 성장

### 아쉬운 점
- 개별 코드 공유는 어려움
- 협업 툴/구조 체계화 필요

### 향후 개선
- 베이스라인 코드 통일 → 분기 실험
- 크롤링 등 다양한 데이터 수집 시도
- 데이터 분석에 더 많은 시간 투자

---

## 📎 Attachments

- 📊 [Presentation Slides (Google Slides)](https://docs.google.com/presentation/d/1goCK9XeZ8y0_F8VlcFVUV3L5twD3pttG/edit?slide=id.p35#slide=id.p35)
- 📒 [Meeting Log (Notion)](https://www.notion.so/21d40cb3731d819e8f6acab053dfcf3c?v=21d40cb3731d81508fdb000ca3e68674)

---

## 🔗 Reference

- 서울시 열린데이터 광장  
- Kaggle Housing Price 예측 레퍼런스  
- scikit-learn / XGBoost / RandomForest 공식 문서  

---

## 🙏 Special Thanks

> “모든 질문은 가치가 있다.”  
> 팀원 여러분의 선의와 공유 정신에 감사드립니다.
