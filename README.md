# HeartWise — Smart Prediction of Heart Disease Using Machine Learning in R

HeartWise is an educational machine-learning project that explores how patient health attributes can be used to classify heart-disease outcomes. The project uses R for data preparation, exploratory analysis, visualization, model training, and evaluation.

> **Important:** This project is for educational and research purposes only. It is not a medical device and must not be used to diagnose, treat, or guide clinical decisions. Predictions from this project are not a substitute for advice from a qualified healthcare professional.

## Project workflow

1. Load and inspect the heart-disease dataset.
2. Check for missing values and remove duplicate rows.
3. Encode selected categorical variables.
4. Explore feature distributions and relationships through visualizations.
5. Split the data into training and test sets.
6. Train logistic regression and random forest classifiers.
7. Evaluate predictions using confusion matrices and accuracy.
8. Review random-forest feature importance.

## Models and reported results

| Model | Reported test accuracy |
|---|---:|
| Logistic regression | 85.33% |
| Random forest | 82.67% |

These figures are the results reported by the project for its test split. They are not a guarantee of performance on other data or in clinical settings.

## Technology stack

- **R** for data analysis and model development
- **tidyverse** and **ggplot2** for data handling and visualization
- **caret** for data partitioning and evaluation utilities
- **randomForest** for random forest classification
- **ROCR** for ROC analysis
- **corrplot** for feature-correlation visualization

## Dataset

The notebook expects a file named `heart.csv` in the working directory. The dataset used in the analysis contains 14 columns, including patient attributes and a binary `target` field. Make sure you have the right to use and share your copy of the dataset; the dataset is not included here unless added separately.

## Running the project

1. Install R and an R-compatible notebook environment, such as Jupyter with an R kernel or Google Colab with R support.
2. Place `heart.csv` in the notebook's working directory.
3. Open and run the notebook cells in order. The notebook installs and loads its R package dependencies.

The notebook also writes `heart_tableau.csv` as an output for further exploration.

## Notes and limitations

- The reported metrics come from a single train-test split and should be treated as illustrative, not as a robust estimate of real-world generalization.
- The notebook uses a classification threshold that differs between some logistic-regression evaluation steps; results may therefore vary depending on the step and threshold used.
- The dataset's variable definitions, collection context, and suitability for a particular use should be reviewed before interpreting results.

## Learning outcomes

- Practice a complete supervised-learning workflow in R.
- Explore data cleaning, categorical encoding, and visualization.
- Compare interpretable logistic regression with a tree-based model.
- Evaluate classifiers and inspect feature importance.

## License

No license has been specified yet. Unless a license is added, standard copyright applies and reuse should not be assumed.
