
# CatBoost Classifier Implementation

This project showcases the implementation of the CatBoost classification model on a dataset to predict a binary outcome. The notebook walks through the process of data preprocessing, model training, and robust evaluation using k-Fold Cross Validation.

## About the Model

[CatBoost](https://catboost.ai/) is a high-performance, open-source gradient boosting on decision trees library. It is particularly well-suited for datasets with categorical features and often provides excellent results with minimal parameter tuning.

This implementation achieves an accuracy of **97.26%** with a standard deviation of **2.03%** across 10 folds, demonstrating the model's high performance and stability on this dataset.

## Dataset

The project uses a `Data.csv` file. The features (`X`) are all columns except the last one, and the target variable (`y`) is the last column, which represents the class to be predicted.

* **Features (X):** Independent variables used for training.
* **Target (y):** The binary outcome (0 or 1) that the model predicts.

## Requirements

The project requires Python and the following libraries:
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* CatBoost

You can install CatBoost using pip:
```bash
pip install catboost
````

## How to Use

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/your-username/catboost-classifier-project.git](https://github.com/your-username/catboost-classifier-project.git)
    cd catboost-classifier-project
    ```

2.  **Ensure you have the dataset:**
    Place your `Data.csv` file in the root directory of the project.

3.  **Run the Jupyter Notebook:**
    Open and execute the `catboost.ipynb` notebook in a Jupyter environment (like Jupyter Lab or Google Colab) to see the full workflow, from data loading to model evaluation.

## Results

The CatBoost classifier was evaluated using 10-fold cross-validation, yielding the following results:

  * **Average Accuracy:** 97.26%
  * **Standard Deviation:** 2.03%

The confusion matrix on a single test split also showed excellent performance with very few misclassifications.
