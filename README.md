# Ensemble Learning Algorithms: AdaBoost, K-Fold Cross Validation, and Bagging

This project provides a comprehensive analysis and comparison of three popular ensemble learning algorithms: **AdaBoost**, **K-Fold Cross Validation**, and **Bagging**. The main focus is on evaluating their performance, accuracy, bias-variance tradeoff, and computational efficiency on employee attrition prediction and other datasets.

## Project Overview
The aim of this project is to predict employee attrition and compare the effectiveness of different ensemble methods. Employee attrition is a key issue for many companies, and predicting the likelihood of employees leaving can provide valuable insights for improving retention. The project involves:

- Implementing and comparing **AdaBoost**, **Bagging**, and **K-Fold Cross Validation** techniques.
- Evaluating accuracy, performance, and execution time across multiple datasets, including employee attrition data.
- Visualizing the results to assess the bias-variance tradeoff, model stability, and computational efficiency.

## Key Algorithms

### 1. **AdaBoost (Adaptive Boosting)**
   - **Description**: AdaBoost is a boosting algorithm that combines multiple weak classifiers to create a strong classifier, focusing on misclassified instances in each iteration.
   - **Use Case**: Applied to employee attrition prediction using decision trees as weak learners.
   - **Key Results**:
     - **Accuracy**: ~85% on employee attrition dataset.
     - **Advantages**: High accuracy and robustness to overfitting.
     - **Limitations**: Sensitive to noisy data and outliers.

### 2. **Bagging (Bootstrap Aggregating)**
   - **Description**: Bagging improves the stability and accuracy of machine learning algorithms by training multiple models on different subsets of the data (bootstrapping).
   - **Use Case**: Used to reduce variance in the employee attrition dataset.
   - **Key Results**:
     - **Accuracy**: ~83% on employee attrition dataset.
     - **Advantages**: Reduces variance, mitigates overfitting.
     - **Limitations**: Higher computational cost due to training multiple models.

### 3. **K-Fold Cross Validation**
   - **Description**: K-Fold Cross Validation divides the dataset into K subsets (folds), training the model on K-1 subsets and testing it on the remaining subset, iterating for each fold. This provides a robust evaluation of the model’s performance.
   - **Use Case**: Evaluated models using 5-fold cross-validation on the employee attrition dataset to ensure unbiased model performance.
   - **Key Results**:
     - **Advantages**: Prevents overfitting by evaluating models on different data partitions.
     - **Limitations**: Computationally expensive for large datasets.

## Dataset Overview
The dataset used in this project includes employee records with 23 features such as:
- **Age**, **Monthly Income**, **Job Role**, **Years at Company**, **Overtime Hours**, **Work-Life Balance**, etc.
- **Target**: Whether the employee left the company or not.

This dataset is crucial for understanding the impact of different features on employee attrition and how ensemble learning algorithms perform in predicting turnover.

## Features
1. **Comparison of Ensemble Methods**: Implementation and in-depth comparison of AdaBoost, Bagging, and K-Fold Cross Validation.
2. **Bias-Variance Tradeoff**: Visualized using K-Fold Cross Validation to highlight the stability of each algorithm.
3. **Performance Metrics**: Evaluation of accuracy, precision, recall, F1-score, and computational time for each algorithm.
4. **Visualizations**: Plots showcasing algorithm performance, including accuracy comparison, execution time, and bias-variance evaluation.

## Visualizations

- **Accuracy Plots**: Visual representations of the accuracy of AdaBoost, Bagging, and K-Fold Cross Validation across different datasets.
- **Execution Time**: A comparison of the execution time for the three algorithms, particularly when handling large datasets.
- **Bias-Variance Evaluation**: Graphs illustrating the bias-variance tradeoff using K-Fold Cross Validation.

## Setup and Usage

### Prerequisites
- Python 3.x
- Required libraries: `scikit-learn`, `NumPy`, `pandas`, `matplotlib`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Emelloul98/Ensemble-Learning-Algorithms.git
   cd Ensemble-Learning-Algorithms
   ```
   
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Comparisons
1. Open the provided Jupyter Notebooks.
2. Run the analysis for AdaBoost, K-Fold, and Bagging using the dataset of your choice.
3. Modify the dataset or K-Fold parameters for customized experiments.
4. View and analyze the generated visualizations to compare performance, bias-variance tradeoff, and execution time.

## Example Visualizations

![AdaBoost Accuracy Plot](https://github.com/Emelloul98/Ensemble-Learning-Algorithms-AdaBoost-K-Fold-Cross-Validation-and-Bagging/blob/main/adaboost.png)

![Bagging Performance Plot](https://github.com/Emelloul98/Ensemble-Learning-Algorithms-AdaBoost-K-Fold-Cross-Validation-and-Bagging/blob/main/feature%20selection.png)


## Results
- **AdaBoost**: Achieved the highest accuracy (85%) but was sensitive to noise.
- **Bagging**: Balanced accuracy (83%) with strong robustness against overfitting.
- **K-Fold Cross Validation**: Ensured stable evaluation with a clear understanding of bias-variance tradeoff, though computationally heavier.

## Conclusion
This project offers a detailed exploration of ensemble learning techniques applied to employee attrition prediction. Through AdaBoost, Bagging, and K-Fold Cross Validation, we gain insight into the strengths and weaknesses of each method in terms of accuracy, bias-variance tradeoff, and execution time. The analysis provides valuable guidance for selecting appropriate ensemble techniques for different datasets and problems.
