# Decision Tree Classifier: Custom Implementation vs Scikit-Learn
# Project Overview
This project investigates the creation and application of a Decision Tree Classifier using the ID3 algorithm, and compares it with the Scikit-Learn DecisionTreeClassifier. The main objective is to explore the performance of a custom-built decision tree and its comparison with a well-established machine learning library. The study utilizes three datasets: Mushroom, Car Evaluation, and Congressional Voting Records, each providing unique challenges in terms of categorical and numerical data handling.

# Features
## Custom ID3 Decision Tree Implementation
A recursive, entropy-based approach for building decision trees from scratch.
## Comparison with Scikit-Learn Classifier
Performance metrics such as accuracy, precision, recall, F1-score, and training time are used to evaluate both classifiers.
## Evaluation across Multiple Datasets
Mushroom, Car Evaluation, and Congressional Voting datasets were used to test the robustness and versatility of the classifiers.
Performance Metrics: Detailed evaluation of models using accuracy, precision, recall, F1-score, and training time.
# Datasets
## Mushroom Dataset
Classification Task
Predict whether a mushroom is edible or poisonous.
Data Type
Categorical features with a binary classification output.
## Car Evaluation Dataset:
Classification Task
Predict the acceptability of a car based on features like price, safety, and maintenance.
Data Type
Categorical features with a multi-class output.
## Congressional Voting Records:
Classification Task: Predict the party affiliation of a congressperson based on their voting record.
Data Type: Categorical features with binary outputs.


# Methodology
## Custom Decision Tree Implementation:
Node Class: This class defines each node in the decision tree, which can either be a decision node or a leaf node (final prediction).
Entropy & Information Gain: Key components of the ID3 algorithm that determine the best feature splits.
Recursive Tree Building: The custom classifier recursively builds the tree by choosing the feature with the highest information gain at each node.
Handling Categorical and Numerical Data: The classifier can handle both types of data, making it versatile for various datasets.
## Scikit-Learn Decision Tree:
Built-in Classifier: The standard DecisionTreeClassifier from Scikit-Learn was used to compare performance with the custom implementation.
Hyperparameter Tuning: The max depth of the tree was varied, and performance was compared across different depths and training sizes.
## Model Evaluation:
Accuracy: The proportion of correct predictions made by the classifier.
Precision & Recall: Metrics that evaluate the classifier’s ability to handle class imbalances.
F1 Score: The harmonic mean of precision and recall, offering a balanced evaluation metric.
Training Time: A critical comparison factor for assessing computational efficiency between classifiers.
# Results
## Performance Comparisons
### Mushroom Dataset:

Custom Classifier: Accuracy of 95%, with slightly longer training times than Scikit-Learn.
Scikit-Learn Classifier: Accuracy of 96.5%, with faster training times.

### Car Evaluation Dataset:

Custom Classifier: Accuracy of 90%, with relatively consistent performance.
Scikit-Learn Classifier: Accuracy of 91.5%, outperforming in both accuracy and efficiency.
### Congressional Voting Records Dataset:

Custom Classifier: Accuracy of 85%, performing well on a politically complex dataset.
Scikit-Learn Classifier: Accuracy of 87.5%, with more stable performance across depths.
## Visualizations
Accuracy vs. Max Depth: Both classifiers achieve high accuracy at various tree depths, though Sklearn tends to slightly outperform theClassifier at deeper tree levels.
Training Time Comparison: Sklearn consistently outperforms theClassifier in terms of training time across all datasets and tree depths.
Accuracy Distribution: The accuracy variability is more significant in theClassifier, whereas Sklearn exhibits more consistent performance.
## Statistical Analysis
t-Test: A Welch Two-Sample t-test comparing the accuracy of both classifiers shows no statistically significant difference in performance (p-value > 0.05).
Linear Regression: A regression analysis reveals that max depth has a significant positive effect on accuracy, but training size and classifier type had little impact.

# Future Work
Hyperparameter Tuning: Future work will focus on optimizing hyperparameters like max_depth and min_samples_split for improved performance.
Handling Imbalanced Data: Investigating techniques like SMOTE or class weighting to improve handling of imbalanced datasets.
Ensemble Methods: Implementing ensemble models like Random Forest to improve both accuracy and computational efficiency.

# Acknowledgements
Special thanks to:

Nabi Nabiyev, M.Sc. Data Science 2024 student at Lancaster University, for assistance with debugging.
Prof. Dr. Plamen Angelov for guidance throughout the project.
Various online resources, including Stack Overflow, Scikit-Learn documentation, Machine Learning Mastery, and others for troubleshooting and conceptual insights.

