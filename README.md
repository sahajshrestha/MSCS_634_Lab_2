# Lab 2: KNN vs RNN Classifiers

## Purpose
This lab compares the performance of K-Nearest Neighbors (KNN) and Radius Neighbors (RNN) classifiers on the Wine dataset using the Scikit-learn library. The goal was to see how different parameter values affect classification accuracy.

## Accuracy Results

### K-Nearest Neighbors (KNN)
- K=1 → 77.78%
- K=5 → 72.22%
- K=11 → 75.00%
- K=15 → 75.00%
- K=21 → 77.78%

### Radius Neighbors (RNN)
- Radius=350 → 75.00%
- Radius=400 → 72.22%
- Radius=450 → 72.22%
- Radius=500 → 72.22%
- Radius=550 → 72.22%
- Radius=600 → 72.22%

## Insights
- **KNN had higher peak accuracy** and performed best at K=1 and K=21.
- **RNN was more stable** but did not outperform KNN at any point.
- The choice of parameters (k or radius) has a direct impact on accuracy.
- KNN is more flexible for tuning and may generalize better with the right `k`.

## Challenges
- RNN returned slightly lower accuracy overall and required handling cases where no neighbors were found.
- KNN was more straightforward and consistent to implement.

## Tools Used
- Python 3
- Jupyter Notebook
- Scikit-learn
- Matplotlib