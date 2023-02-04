# Machine Learning- Comparing Classification & Feature Extraction Approaches

Project Objective:
1. Application of two Feature Extraction approaches i.e., PCA & Feature Selection, and classification of the dataset using the Linear Discriminant Analysis and Support Vector Machine.
2. Classification using different Machine Learning Algorithms and analyzing which algorithm is the most suitable.
    The project was completed using 3 different approaches namely:
    1. K Nearest Neighbors
    2. Naïve Bayes
    3. AdaBoost
Dataset Used:
The data used for the project was taken from the UCI Machine Learning Repository. It is named “Electrical Grid Stability Simulated Dataset” and has 10,000 instances. It is a multivariate dataset consisting of 13 attributes and two classes. It is a numerical dataset with real values. The data is classified based on the stability label of the system. 0 refers to unstable state and 1 refers to stable state (which is preferred) of the electrical grid.
https://archive.ics.uci.edu/ml/datasets/Electrical+Grid+Stability+Simulated+Data+

Methodology:
1. A dataset of 10,000 samples was taken and split into training and testing sets in the ratio 3:1.
2. Initially LDA was applied to the original dataset with all the features followed by the calculation of classification error and runtime.
3. Similarly, SVC was applied to the original dataset with all the features followed by the calculation of classification error and runtime.
4. Four Experiments were carried out based on the two Dimensionality reduction techniques PCA and Backward Search and then the dataset was classified using LDA and SVC. Confusion matrices were determined for each step of the dimensionality reduction in all 4 experiments. Later their classification errors and training & testing runtimes were calculated and plotted, and the results compared.
• Experiment 1: Dimensionality reduction using PCA and classification using LDA
• Experiment 2: Dimensionality reduction using PCA and classification using SVC
• Experiment 3: Dimensionality reduction using Backward Search and classification using LDA
• Experiment 4: Dimensionality reduction using Backward Search and classification using SVC
5. We used 3 approaches to classify the data which were KNN, Naïve Bayes, and AdaBoost.
6. After organizing the data, the parameters with respect to each algorithm were calculated followed by computational time, confusion matrix, cross-validation and finally plotting the ROC curve.

Observations:
The different observations and comparison of results are demonstrated by the two graphs below followed by an explanation:
1. Upon calculation of percentage of classification error with all features and total runtime of both LDA and SVC models, it was observed that the percentage of classification error through SVC (0.4%) was much less than that obtained using LDA (2%). However, the total runtime of LDA model was significantly less than that of the SVC model as demonstrated in the Graph (2)
2. The least computational time was observed in the Naïve Bayes approach, followed by AdaBoost and KNN. The testing time for KNN is fairly larger than the training time because most of the computational process takes places during the testing process itself. Once Naïve Bayes and AdaBoost classifiers are trained, it takes very less computational time for testing.

FOR DETAILED OBSERVATIONS REFER files in the Results folder
