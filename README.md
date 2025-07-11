# Title (Please modify the title)

## Team

| ![박패캠](https://avatars.githubusercontent.com/u/156163982?v=4) | ![이패캠](https://avatars.githubusercontent.com/u/156163982?v=4) | ![최패캠](https://avatars.githubusercontent.com/u/156163982?v=4) | ![김패캠](https://avatars.githubusercontent.com/u/156163982?v=4) | ![오패캠](https://avatars.githubusercontent.com/u/156163982?v=4) |
| :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: |
|            [박패캠](https://github.com/UpstageAILab)             |            [이패캠](https://github.com/UpstageAILab)             |            [최패캠](https://github.com/UpstageAILab)             |            [김패캠](https://github.com/UpstageAILab)             |            [오패캠](https://github.com/UpstageAILab)             |
|                            팀장, 담당 역할                             |                            담당 역할                             |                            담당 역할                             |                            담당 역할                             |                            담당 역할                             |

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
