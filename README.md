# fake_or_real_news
                 ML-Truth_Serum
 Overview
The idea behind “Fake or Real News Predictor” project was to apply Machine Learning techniques to predict whether a particular news story is real or fake. We wanted to test if leveraging various ML techniques and applications could provide a good assessment of the veracity of an article or a news report. We also wanted to understand how and which ML model we can train to accomplish the task above in the best possible way. Our main hypothesis was that using a Generative Pre-Trained Transformer (neuro networks) will yield a better accuracy then a logistic model (baseline machine learning).


Model Summary
The input data was pulled from Kaggle.  It contained 6200+ record.  Each record contained 3 elements: a title of the article, text of the article and a classifier (real/false)
The data was used to train and test models using:
a. Simple models that parsed the title and text of the articles into individual words and used Random Forrest and Logistic Regression to classify each article.  The results were checked against the actual classifiers
b. OpenAI Pre Trained (neuro network) model using embeddings translates text into a numerical format (embeddings) that represents the meaning of words and their relationships. It then analyzes these numerical representations to categorize the text into specific classes or categories based on its content.


Data Clean-Up 
a. Reading in and merging the data 
b. Dropping rows with NaN from the combined data frame
 Removing outliers
c. Removing special character while keeping apostrophes to preserve the meaning.
d. Columns updated from Object  data types to string.
e. Making text not case sensitive. 
f. Standardizing the classification types.

Model Training
a. Creating training and testing datasets with the following break down (2/3 training data vs. 1/3 Testing data) for ML models.
b. Creating training and testing datasets with the following break down (20% training data vs. 80% Testing data) for OpenAI  model.

Model Evaluation - Simple ML Model 
a. Simple models – based on the encoded text values:
We created 3 “simple” models to test the results:
Simple Logistic Regression Model 1 – Classifying Articles based only on the text in the Title.  The accuracy rate was 75%
b. Random Forest Model - Classifying Articles based the text in the Title and the Body of the article.  The accuracy rate was 68%
c. Simple Logistic Regression Model 2 – Classifying Articles based on the text in the Title and the Body of the articles.  The accuracy rate was 72%

Conclusion 
a. OpenAI Based model showed significantly higher accuracy rate of 91% vs 75% (for best performing simple model), which supported our initial hypothesis
b. OpenAI model used only 20% of the data available to train, yet still delivered superior results
c. The high accuracy classification rate of the OpenAI model proves viability of using this ML based model to determine the validity of news articles in a very time efficient way
d. This could make a powerful research tool which allows quickly discard invalid/fake news from a particular analysis on various economic, financial, scientific and political topics

Next Steps
a. We’ve discussed possibility of doing additional testing of articles and user inputs  that were not part of our original data set
b. We’ve also considered leveraging OpenAI Model to do different type of assessment/classification of news articles to identify hate speech, political leanings, or to determine overall subject of the publication (economy, politics, travel, science, etc.)
c. Determining which words were more likely associated with fake or real classifications

