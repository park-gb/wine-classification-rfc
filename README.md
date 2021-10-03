# RandomForest 알고리즘 기반 와인 분류
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## 목표
- Random Forest 알고리즘 기반 와인 분류를 위한 Classifier 모델링(Binary Classification)

## 데이터셋
- Source: [Wine Quality Data Set](https://archive.ics.uci.edu/ml/datasets/Wine+Quality)
- Description
  - 목표변수
    - 클래스 개수: 2개(Red wine: 0, White wine: 1)
    - 목표변수명: target
  - 설명변수(Feature) 13개
    - fixed acidity: 산도
    - volatile acidity: 휘발성산
    - citric acid: 시트르산
    - residual sugar: 잔당(발효 후 남은 당분)
    - chlorides: 염화물
    - free sulfur dioxide: 독립 이산화황
    - total sulfur dioxide: 총 이산화황
    - density: 밀도
    - pH: 수소이온농도
    - sulphates: 황산염
    - alcohol: 알코올
    - quality: 품질

  - 전체 인스턴스 개수: 6,497개
    - 레드 와인 instance: 1,599개
    - 화이트 와인 instance: 4,898개

## 파일구조
``` bash
├─wine-classification-rfc
│ README.md
│  ├─src
│  │      wine_classification_rfc.ipynb
│  └─model
│  │      wine_classification_rfc.pkl
│  └─figure
│  │      RFC_n_estimator.png
│  │      RFC_n_depth.png
│  │      RFC_min_samples_split.png
│  │      RFC_min_samples_leaf.png
│  │      RFC_confusion_matrix.png
│  │      RFC_feature_importance.png
│  └─dataset
│         red_raw.csv
│         white_raw.csv
│         wine_combined_raw.csv
│         wine_combined_prep.csv
```

## 모델 성능
- Accuracy: 99.8%
- Precision: 0.999
- Recall: 0.998
- F1-score: 0.999
- Confusion Matrix

![RFC_confusion_matrix](https://user-images.githubusercontent.com/80144296/135718352-266fdeaf-8577-48b0-82df-7921993130f3.png)

## 변수 중요도
![RFC_feature_importance](https://user-images.githubusercontent.com/80144296/135718375-0f310008-7b47-4b2c-93c2-512e0d99e63a.png)

## 상세설명
- [티스토리 블로그](https://heytech.tistory.com/118)
