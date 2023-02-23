### Confusion matrix

The data came from [Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset?select=heart.csv)

A logistic regression model is used to predict whether a participant in a study has heart disease or not, based on a set of features that is related to the presence of heart disease. 

Features:
- age
- sex
- cp: chest pain type (4 values)
- trestbps: resting blood pressure
- col: serum cholestoral in mg/dl
- fbs: fasting blood sugar > 120 mg/dl
- restecg: resting electrocardiographic results (values 0,1,2)
- thalach: maximum heart rate achieved
- exang: exercise induced angina
- oldpeak: ST depression induced by exercise relative to rest
- slope: the slope of the peak exercise ST segment
- ca: number of major vessels (0-3) colored by flourosopy
- thal: 0 = normal; 1 = fixed defect; 2 = reversable defect

We can train the logistic regression model on a labeled dataset, where each participant is labeled with either 0 (no heart disease) or 1 (heart disease) as the target outcome.

Once the model is trained, we can use it to make predictions on new, unseen data. For each new example, the logistic regression model will output a predicted probability of having heart disease, based on the values of the input features. If the predicted probability is greater than a certain threshold, we can classify the example as having heart disease, otherwise we can classify it as not having heart disease.

To evaluate the performance of the logistic regression model, we can use a confusion matrix. A confusion matrix is a table that summarizes the number of true positives, true negatives, false positives, and false negatives produced by the model on a given set of examples. True positives (TP) are the number of examples that were correctly classified as having heart disease, true negatives (TN) are the number of examples that were correctly classified as not having heart disease, false positives (FP) are the number of examples that were incorrectly classified as having heart disease (false alarms), and false negatives (FN) are the number of examples that were incorrectly classified as not having heart disease (missed detections).

By analyzing the confusion matrix, we can calculate metrics such as accuracy, precision, recall, and F1-score, which provide a more detailed assessment of the model's performance. For example, accuracy measures the proportion of examples that were classified correctly, while precision measures the proportion of positive predictions that were correct, and recall measures the proportion of actual positives that were correctly predicted. F1-score is the harmonic mean of precision and recall and is often used as a summary metric that balances the trade-off between precision and recall.
