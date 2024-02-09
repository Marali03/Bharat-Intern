# Bharat-Intern
internship program 2024

Introduction:
The objective of this project is to develop a text classification model to distinguish between spam and non-spam (ham) SMS messages. We explored two Naive Bayes models for this task: Gaussian Naive Bayes and Multinomial Naive Bayes.

Data Loading and Preprocessing:
The SMS dataset was loaded and preprocessed to extract relevant features. The dataset initially contained multiple columns, including the target variable ('spam' or 'ham') and the SMS message text. The data was cleaned by removing duplicate entries and unnecessary columns.

Feature Engineering:
Three features were engineered from the text data: the number of characters, the number of words, and the number of sentences in each SMS message. These features provide insights into the length and structure of the messages, which can be crucial for distinguishing between spam and ham.

Exploratory Data Analysis (EDA):
Descriptive statistics and visualizations were used to analyze the distribution of features in both spam and ham messages. The analysis revealed differences in the length and structure of spam and ham messages, motivating the need for a robust classification model.

Model Selection:
Two Naive Bayes models were considered: Gaussian Naive Bayes and Multinomial Naive Bayes. Gaussian Naive Bayes assumes that numerical features follow a Gaussian distribution, while Multinomial Naive Bayes is designed for discrete features, such as word counts.

Model Training and Evaluation:
Both models were trained on the text data, and their performances were evaluated using a test set. The accuracy metric was used to assess the models' overall effectiveness in classifying SMS messages.

Gaussian Naive Bayes:
Achieved an accuracy of approximately 90.72% on the test set.
Assumes a Gaussian distribution for numerical features.
Suitable for continuous features but may not be optimal for discrete word counts.

Multinomial Naive Bayes:
Achieved a comparable accuracy of approximately 90.72% on the test set.
Specifically designed for discrete features like word counts.
Better suited for text classification tasks involving word frequency.

Conclusion:
Both Gaussian Naive Bayes and Multinomial Naive Bayes demonstrated similar performance in classifying SMS messages. The choice between the two depends on the nature of the features. Since our features involve word counts (a discrete, non-negative value), Multinomial Naive Bayes appears to be a more appropriate choice for this SMS spam classification task.

Recommendation:
For this specific SMS spam classification project, we recommend using Multinomial Naive Bayes due to its alignment with the nature of the features. It is well-suited for tasks involving discrete data such as word counts, making it a more robust choice for text classification.


