# fake_or_real_news
                 ML-Truth_Serum
 Overview
The idea behind “ML-truth-Serum” project was to analyze the summary/title of the articles to predict if the news is real or fake.
The key hypothesis that we wanted to use the Generative Pre Trained Transformer (neuro networks) or Semantic model  that will yield a better accuracy than a logistic regression model (baseline machine learning). We used hugging face to classify our text of the news.
We also wanted to understand what, if any, limitations exist when using the above inputs to predict the news is fake or real.

Data Summary
a. Simple model/Logistic Model
This model basically tell us that the word is true or false and we added the hate speech sentiment and it used the word count to predict whether the news is real or fake.
b. Generative Pre Trained Transformer/Semantic Model
This model basically converted the text into vector and with the help of chat gpt and openai and hugging face, it tells us where these words belong to make the model more accurate.

Data Clean-Up and Model Training
	•	Reading in and merging the data 
	•	Dropping rows with NaN from the combined data frame
	•	Removing outliers
	•	Creating training and testing datasets with the following breakdown (2/3 training data vs. 1/3 Testing data)
