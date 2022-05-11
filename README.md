# ML-ComparingFeatureExtractionApproaches

SEP 786 – ARTIFICIAL INTELLIGENCE AND MACHINE LEARNING FUNDAMENTALS COURSE PROJECT REPORT
COMPARING FEATURE EXTRACTION APPROACHES
DATE: November 28th, 2021

Project Objective:
Application of two Feature Extraction approaches i.e., PCA & Feature Selection, and classification of the dataset using the Linear Discriminant Analysis and Support Vector Machine.

Dataset Used:
The data used for the project was taken from the UCI Machine Learning Repository. It is named as “Electrical Grid Stability Simulated Data Data Set” and has 10,000 instances. The dataset consists of 13 attributes and 2 classes of data. It is a multivariate data set having real values. https://archive.ics.uci.edu/ml/datasets/Electrical+Grid+Stability+Simulated+Data+

Methodology:
1. A dataset of 10,000 samples was taken and split into training and testing sets in the ration 3:1.
2. Initially LDA was applied to the original dataset with all the features followed by the calculation of classification error and runtime.
3. Similarly, SVC was applied to the original dataset with all the features followed by the calculation of classification error and runtime.
4. Four Experiments were carried out based on the two Dimensionality reduction techniques PCA and Backward Search and then the dataset was classified using LDA and SVC. Confusion matrices were determined for each step of the dimensionality reduction in all 4 experiments. Later their classification errors and training & testing runtimes were calculated and plotted, and the results compared.
• Experiment 1: Dimensionality reduction using PCA and classification using LDA
• Experiment 2: Dimensionality reduction using PCA and classification using SVC
• Experiment 3: Dimensionality reduction using Backward Search and classification using LDA
• Experiment 4: Dimensionality reduction using Backward Search and classification using SVC

Observations:
The different observations and comparison of results are demonstrated by the two graphs below followed by an explanation:
1. Upon calculation of percentage of classification error with all features and total runtime of both LDA and SVC models, it was observed that the percentage of classification error through SVC (0.4%) was much less than that obtained using LDA (2%). However, the total runtime of LDA model was significantly less than that of the SVC model as demonstrated in the Graph (2)
2. Experiment 1: Dimensionality reduction using PCA and classification using LDA
• As the number of dimensions reduced, the classification error increased as seen in the Graph (1). Classification error with 13 features was 61 and that with 1 feature increased to 908
3. Experiment 2: Dimensionality reduction using PCA and classification using SVC
• As the number of dimensions reduced, the classification error increased as seen in the Graph (1). Classification error with 13 features was 10 and that with 1 feature increased to 900
4. Experiment 3: Dimensionality reduction using Backward Search and classification using LDA
• As the number of dimensions reduced, the classification error remained almost constant.
5. Experiment 4: Dimensionality reduction using Backward Search and classification using SVC
6. As the number of dimensions reduced, the classification error remained almost constant.
7. Overall, we noticed that when it comes to efficiency in terms of classification error, the Feature selection methodology outperforms the PCA methodology by a significant margin. Since PCA uses the variance to determine the most important feature, it is not always suitable for classification problems.
8. Within the backward search, we observed lesser classification error when support vector machine classifier used compared to LDA.
9. Coming to computational runtime, it is apparent from the plots that LDA classifier takes relatively lesser time to train and test the data set compared to support vector machine classifier.
10. In general, we noticed that the computational time reduces as and when more and more features are removed. This is because the size of the data being worked on reduces.
11. Confusion matrices were determined for each step of the dimensionality reduction for all 4 experiments in the below format:
Class 0 misclassified as Class 1
(False positive or Type 1 error)
Class 1 correctly classified
(True positive)
Class 0 correctly classified
(True negative)
Class 1 misclassified as Class o
(False negative or Type 2 error)
