# Heart Disease Classification with KNN

A machine learning project focused on classifying heart disease using the K-Nearest Neighbors (KNN) algorithm. Developed using the tidymodels framework in R, this project demonstrates strong skills in data preprocessing, model tuning, and evaluation. The objective was to build a robust and interpretable model while navigating real-world challenges, such as performance trade-offs in healthcare applications.


## Tech Stack

- **Language**: R  
- **Framework**: tidymodels  
- **Model**: K-Nearest Neighbors
- **Evaluation**: Cross-validation, Accuracy, Precision, Recall, Confusion Matrix  
- **Visualization**: ggplot2  


## Project Highlights

- **Goal**: Predict heart disease presence using clinical features like age, max heart rate, and ST depression.
- **Approach**:
  - Preprocessed data using recipes (center/scale).
  - Split into training/testing (75/25) with stratification.
  - Trained initial KNN model (`k = 3`) and evaluated baseline performance.
  - Performed 5-fold cross-validation and hyperparameter tuning to find optimal `k`.
  - Re-trained the final model and evaluated performance on test data.


## Model Results

| Metric     | Before Tuning | After Tuning |
|------------|----------------|---------------|
| Accuracy   | 73.33%         | **78.67%**    |
| Precision  | 71.43%         | **88.00%**    |
| Recall     | 71.43%         | **62.86%**    |

- Final model used `k = 66` (optimal via tuning).
- High **precision** reduces false positives—important in clinical screening.
- Lower **recall** reveals a trade-off: missed cases, highlighting the challenge of medical ML.

## Skills Demonstrated

- Applied end-to-end ML workflow using `tidymodels`.
- Built reproducible pipelines with clear preprocessing steps.
- Conducted robust model validation with cross-validation.
- Performed metric-driven hyperparameter optimization.
- Interpreted model performance in a healthcare context.


## Notes

- Dataset derived from the [UCI Heart Disease dataset](https://archive.ics.uci.edu/ml/datasets/Heart+Disease).
- All analysis was done in R using a reproducible pipeline.




