# Hespress_Classifier
Text Classification of Hespress News Stories

The purpose of this analysis is to classify a set of Hespress news stories into different topics using machine learning. The data consists of multiple CSV files that contain news stories in Arabic language, and each story is labeled with a topic, such as politics, sports, or entertainment.

Data Preparation
The first step in the analysis was to load the data from the CSV file into a Pandas dataframe. The code used the pd.read_csv function to read the file, and then encoded the topic labels using the preprocessing.LabelEncoder function. The resulting dataframe contained a total of N rows and M columns.

The code also performed some data preparation steps to split the data into training and testing sets. Specifically, it split the data by topic, and then randomly shuffled the data and split it into 80% training and 20% testing sets for each topic.

Text Classification
To classify the news stories into different topics, the code used the Linear Support Vector Classifier (LinearSVC) algorithm. The code vectorized the text data using the TfidfVectorizer function to convert the text into numerical features. It then trained the LinearSVC model on the training data, and used the model to predict the topic labels for the testing data.

The code evaluated the performance of the model using the classification_report function, which provided various metrics such as precision, recall, and F1-score for each topic.
