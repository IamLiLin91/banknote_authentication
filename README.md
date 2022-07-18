# banknote_authentication
![image](https://user-images.githubusercontent.com/109471364/179455009-c92aad6d-8eec-483c-a0f0-50110ab3091e.png)
## Background
This project is about distinguishing genuine and forged banknotes. Data were originally extracted from images that were taken from genuine and forged banknote-like specimens. For digitization, an industrial camera usually used for print inspection was used. The final images have 400 x 400 pixels. Due to the object lens and distance to the investigated object, gray-scale pictures with a resolution of about 660 dpi were gained. A Wavelet Transform tool was used to extract 4 features from these images. The input and the output attributes are as follows:
1. Variance of Wavelet Transformed image (continuous)
2. Skewness of Wavelet Transformed image (continuous)
3. Kurtosis of Wavelet Transformed image (continuous)
4. Entropy of image (continuous)
5. Class (target): Presumably 0 for genuine and 1 for forged

Note: The dataset need to be randomly shuffled before you split the data.

## Tasks
1. State whether you need to perform any data preprocessing on this dataset and do those
preprocessing steps if needed.
2. Perform feature normalization.
3. Construct the logistic regression equation to classify whether the bank note is genuine or forged. Write down your equation in your report. Explain this equation briefly and the number of parameters that need to be estimated.
4. Split the dataset into train (70%) and test (30%).
5. Import SGDClassifier from scikit-learn API using log as the loss function (the ‘log’ loss gives logistic regression) and optimize these hyperparameters (namely, alpha, max_iter, tol,learning_rate) to achieve a model with the best accuracy. Explain your optimal hyperparameters in the report.
6. Use the classification_report() function provided by the scikit-learn library to construct a classification report for step 5. 
7. Use and/or regularization/penalty hyperparameter along with other optimal hyperparameters you have identified from step 5 for model training, and discuss in detail
about its working and its impact on your model accuracy. 
8. Use the classification_report() function provided by the scikit-learn library to construct a classification report for step 7 after regularization.
9. Import k-nearest neighbors (KNN) from scikit-learn API, build a KNN model with default hyperparameters, compare KNN's accuracy with Step 5 and briefly explain in the report.

