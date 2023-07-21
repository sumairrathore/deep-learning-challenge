# deep-learning-challenge
Analysis of Charitable Funding Prediction
Analysis Overview: In this study, I aimed to predict the success of charitable donations for a charitable organization called Alphabet Soup, using a deep learning approach. The dataset used for analysis was "charity_data.csv," which contained information about different organizations' funding applications. The primary goal was to create a model with predictive accuracy exceeding 75%, allowing Alphabet Soup to identify organizations likely to utilize their funding effectively.
Results Summary: 
  Data Preprocessing: 
-	Target Variable: I used the "IS_SUCCESSFUL" column as my  target variable, indicating whether an organization's funding application was successful (1) or not (0). 
-	 Features: Initially, I considered all columns, excluding "IS_SUCCESSFUL," "EIN," and "NAME," as features for my  model. However, during model optimization, I found that including the "NAME" column as a feature improved the accuracy to over 78%. 
-	Removed Variables: After optimization, I observed that the "EIN" column didn't contribute significantly to the model's predictive power, so I removed it from the input data.
Model Compilation, Training, and Evaluation: 
-	Neural Network Model: I designed a deep neural network with multiple hidden layers to achieve high performance. The model comprises 80 neurons in the first hidden layer with 'relu' activation, 30 neurons in the second hidden layer with 'relu' activation, and 1 neuron in the output layer with 'sigmoid' activation. 
-	Target Model Performance: My  objective was to achieve an accuracy greater than 75% on the testing dataset. 
-	Steps to Increase Model Performance: I enhanced the model's performance by including the "NAME" column as a feature during training.
Summary: My  deep learning model surpassed the target accuracy of 75% on the testing dataset, meeting my  expectations. However, the inclusion of the "NAME" column likely introduced noise and overfitting to the analysis, which may impact generalization to new data.
Recommendation: For this classification problem, my  deep learning model achieved a predictive accuracy of 73% on the testing dataset. The inclusion of the "NAME" column as a feature significantly increased accuracy to over 78%, but it might have introduced overfitting concerns.
To build a more robust model, I recommend exploring alternative methods, such as the Random Forest Classifier. This approach can offer insights into feature importance, allowing identification of the most influential factors in funding application success.
In conclusion, while the deep learning model met the target accuracy, it's crucial to investigate various models and optimization techniques for a more effective solution. Combining deep learning and traditional machine learning approaches can provide valuable insights without compromising generalization on new data and mitigating overfitting issues.
