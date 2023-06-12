# Predicting Chronic Kidney Disease
For this project, a random forest classifier was used to predict the presence of chronic kidney disease. The dataset underwent preprocessing steps, such as converting categorical variables like "rbc" (Red Blood Cell count) to binary values (1 or 0) for normal or abnormal, respectively. Additionally, missing values represented as "\t?" were replaced with NaN, which were then filled with the mean value of the respective columns. Duplicate columns were not present.

A pipeline was created using Scikit-learn's MinMaxScaler and RandomForestClassifier after splitting the dataset into training and testing sets. The accuracy score achieved by this algorithm was 92%, indicating a good performance.

A confusion matrix was plotted to evaluate the accuracy of the model. The classification report based on the confusion matrix demonstrated that the model performed well, with high precision, recall, and F1-score for both the "with CKD" and "without CKD" classes. This suggests that the model effectively distinguished between the two classes. The high accuracy and consistent performance across metrics indicate the reliability of the model for this classification task.

![cm_ckd](https://github.com/temmyfioye/predictingchronickidneydisease/assets/26744249/a7bd19e5-b7cb-474b-add2-90595a99b1cc)

Furthermore, the top 5 features, namely Hemoglobin (hemo), Packed Cell Volume (pcv), Specific Gravity (sg), rbc, and Albumin (al), were identified as the most important features. These features play a significant role in the random forest classifier's decision-making process. They reflect the importance of blood and urine parameters related to kidney function in determining the presence of chronic kidney disease. By considering these features, the model can make accurate predictions and provide insights into the factors that contribute most to the classification task.

![features_ckd](https://github.com/temmyfioye/predictingchronickidneydisease/assets/26744249/78d7b117-1dd4-46fc-83ef-4c7321736764)
