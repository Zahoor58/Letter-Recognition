# Letter Recognition Using SVM 

## Overview
This case study focuses on building a machine-learning model to recognize letters based on various attributes. The dataset used in this study contains information about different characteristics of letters, and the goal is to predict which letter corresponds to a given set of attributes.

## Files
- `letter-recognition.csv`: This is the dataset file containing the letter recognition data.
- `letter_recognition_svm.ipynb`: This is the Jupyter notebook file that contains the entire code for data exploration, preprocessing, model building, and evaluation.

## Dependencies
Make sure you have the following libraries installed before running the code:
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

You can install them using `pip`:

## Steps

1. **Data Understanding**
   - The dataset's shape, attributes, and data types are explored.
   - Some visualizations are used to understand how various attributes vary with the letters.

2. **Data Preparation**
   - The dataset is preprocessed, including scaling the features.
   - The data is split into training and testing sets.

3. **Model Building**
   - Two initial models are built: a linear SVM and a non-linear SVM with default hyperparameters.
   - Model accuracies and confusion matrices are evaluated.

4. **Hyperparameter Tuning**
   - Grid Search is used to find the optimal values of hyperparameters (`C` and `gamma`) for the non-linear RBF kernel.
   - Cross-validation is performed with 5 folds to ensure robustness.

5. **Choosing the Best Model**
   - The best hyperparameters are determined based on the highest test accuracy.

6. **Building and Evaluating the Final Model**
   - The final SVM model is built with the optimal hyperparameters.
   - The model's accuracy and confusion matrix are reported.

## Conclusion
The study demonstrates that the problem of letter recognition is inherently non-linear, as evidenced by the superior performance of non-linear models compared to linear ones. The final model achieves an accuracy of approximately 95%, indicating that it is well-suited for this task.


