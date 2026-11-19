# Customer Churn Prediction — Results

- Dataset: 1200 synthetic customer records
- Target: Churn (0 = stayed, 1 = churned)
- Overall churn rate: 32.7%
- Train/test split: 80% / 20%, stratified
- Best model by test ROC-AUC: Logistic Regression

## Test-set metrics

| Model               |   Accuracy |   Precision |   Recall |     F1 |   ROC_AUC |
|:--------------------|-----------:|------------:|---------:|-------:|----------:|
| Logistic Regression |     0.6417 |      0.4608 |   0.6026 | 0.5222 |    0.7433 |
| Random Forest       |     0.6958 |      0.5281 |   0.6026 | 0.5629 |    0.7339 |

## Classification report

```text
              precision    recall  f1-score   support

      Stayed       0.78      0.66      0.71       162
     Churned       0.46      0.60      0.52        78

    accuracy                           0.64       240
   macro avg       0.62      0.63      0.62       240
weighted avg       0.67      0.64      0.65       240
```

## Confusion matrix

```text
[[107  55]
 [ 31  47]]```

## Important limitation

The dataset is synthetic and intended for education and portfolio demonstration. These scores do not represent real-world company performance.
