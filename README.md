# Lab 2: Classification Using KNN and RNN Algorithms

## Course
Advanced Big Data and Data Mining  
Spring 2026  

## Student
Mounisha Yarava  

## Overview
This lab focuses on implementing and analyzing two instance-based classification algorithms:
- K-Nearest Neighbors (KNN)
- Radius Neighbors (RNN)

The goal is to understand how different parameter values impact classification performance using the Wine dataset.


## Dataset
- Source: Scikit-learn built-in dataset
- Name: Wine Dataset
- Features: 13 numerical attributes (e.g., alcohol, color intensity)
- Classes: 3 wine categories


## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn


## Implementation Details

### 1. Data Preparation
- Loaded dataset using sklearn
- Split into training and testing sets (80/20)

### 2. K-Nearest Neighbors (KNN)
- Tested values of K: 1, 5, 11, 15, 21
- Evaluated using accuracy score

**Observations:**
- Small K → Overfitting
- Moderate K → Best performance
- Large K → Slight underfitting


### 3. Radius Neighbors (RNN)
- Tested radius values: 350–600

**Observations:**
- Small radius → Fewer neighbors, lower accuracy
- Medium radius → Best results
- Large radius → Reduced performance


## Results

| Model | Best Performance |
|------|----------------|
| KNN  | More stable and consistent |
| RNN  | Sensitive to radius selection |


## Visualizations
- Accuracy vs K (KNN)
- Accuracy vs Radius (RNN)


## Challenges
- Selecting optimal radius values for RNN
- Understanding overfitting vs underfitting
- Interpreting model performance


## Conclusion
KNN performed more consistently and was easier to tune.  
RNN offered flexibility but required careful parameter selection.

## How to Run

```bash
pip install numpy pandas matplotlib scikit-learn
