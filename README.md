# [채린이네] Team 

## 최대한 많이 넘어져 보자

| ![문채린](https://avatars.githubusercontent.com/u/156163982?v=4) | <img src="https://avatars.githubusercontent.com/u/66048976?v=4" width="150" style="border-radius:50%;">  | ![김상윤](https://avatars.githubusercontent.com/u/156163982?v=4) | ![김동준](https://avatars.githubusercontent.com/u/156163982?v=4) | ![정서우](https://avatars.githubusercontent.com/u/156163982?v=4) |
| :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: |
|            [문채린](https://github.com/UpstageAILab)             |            [박재홍](https://github.com/woghd8503)             |            [김상윤](https://github.com/UpstageAILab)             |            [김동준](https://github.com/UpstageAILab)             |            [정서우](https://github.com/UpstageAILab)             |
|                            팀장, 데이터 전처리 및 모델링                             |                            개발 환경 세팅                             |                            데이터 전처리 및 모델링                             |                            데이터 전처리 및 모델링                             |                            데이터 전처리 및 모델링                             |

## 1. Competiton Info

### Overview

- _Write competition information_

### Timeline

- ex) January 10, 2024 - Start Date
- ex) February 10, 2024 - Final submission deadline

### Evaluation

- _Write how to evaluate model_

## 2. Components

### Directory
```
project/
├── notebooks/                 # 주피터 노트북 작업 공간
│   ├── user1/                # 개인 작업 공간
│   ├── user2/
│   ├── user3/
│   ├── user4/
│   └── user5/
│
├── data/                     # 공유 데이터
│   ├── raw/                  # 원본 데이터
│   ├── processed/            # 전처리된 데이터
│   └── external/             # 외부 데이터
│
├── src/                      # 소스 코드
│   ├── data/                 # 데이터 처리
│   ├── features/             # 피처 엔지니어링
│   ├── models/               # 모델 정의
│   └── utils/                # 유틸리티 함수
│
├── experiments/              # 실험 결과 저장
│   ├── user1/
│   ├── user2/
│   ├── user3/
│   ├── user4/
│   └── user5/
│
├── models/                   # 학습된 모델 저장
│   ├── user1/
│   ├── user2/
│   ├── user3/
│   ├── user4/
│   └── user5/
│
├── .gitignore               # Git 제외 파일 설정
├── environment.yml          # Conda 환경 설정
└── requirements.txt         # pip 패키지 목록
```

### Environment Setup

#### Conda 환경 설정
```bash
# Conda 환경 생성 및 활성화
conda env create -f environment.yml
conda activate real_estate_pred
```

#### pip 환경 설정
```bash
# 가상환경 생성
python -m venv venv

# 가상환경 활성화
# Windows
.\venv\Scripts\activate
# Linux/Mac
source venv/bin/activate

# 패키지 설치
pip install -r requirements.txt
```

## 3. Data descrption

### Dataset overview

- _Explain using data_

### EDA

- _Describe your EDA process and step-by-step conclusion_

### Feature engineering

- _Describe feature engineering process_

## 4. Modeling

### Model descrition

- _Write model information and why your select this model_

### Modeling Process

- _Write model train and test process with capture_

## 5. Result

### Leader Board

- _Insert Leader Board Capture_
- _Write rank and score_

### Presentation

- _Insert your presentaion file(pdf) link_

## etc

### Meeting Log

- _Insert your meeting log link like Notion or Google Docs_

### Reference

- _Insert related reference_
