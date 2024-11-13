Depression and Anxiety Detection using NLP on Social Media
Project Overview
This project leverages Natural Language Processing (NLP) techniques to analyze and predict depression and anxiety from social media messages. By using sentiment analysis, we aim to help identify individuals who may be suffering from these mental health conditions based on their posts, enabling early intervention and support.

The project walks through the entire process of sentiment analysis, from data gathering and cleaning to building a machine learning model for classification. It also explores the challenges of automating sentiment detection and suggests possible areas for improvement.

Key Features:
Sentiment Analysis: Classify text from social media posts into depression, anxiety, or neutral categories.
Data Visualization: Word clouds to better understand the themes and keywords associated with depressive, anxious, and positive sentiments.
Machine Learning Model: Predict mental health conditions based on user-generated content on social media platforms.
Motivation
Depression and anxiety are increasingly prevalent in today's fast-paced, stressful world. Early detection using text-based data can help individuals seek help before the situation worsens, improving both individual well-being and the broader community’s mental health outcomes.

Project Workflow
The project is broken down into five major steps:

Step 1: Gathering Data
The data for this project was collected from the following sources:

Sentimental Analysis for Tweets (Kaggle)
Sentiment140 (Kaggle)
Additionally, sentiment labels were manually added to the dataset. You can access the sentiment-labeled data here:

SentimentAnalysisData.csv
Manual sentiment analysis revealed insights into the limitations of fully automated systems and suggested areas for improvement in the field.

Step 2: Data Cleaning
Cleaning the data is an essential step for improving model accuracy. The following preprocessing techniques were applied:

Stop-word Removal: Filtered out commonly used words that don't contribute to sentiment analysis (e.g., "the," "and").
Lemmatization: Reduced words to their base forms (e.g., "running" → "run").
Text Cleaning: Removed non-word characters, URLs, extra spaces, and other irrelevant symbols.
Step 3: Data Analysis
Data analysis was performed to visualize and better understand the content of the dataset. The following visualizations were created:

Word Cloud for Depression Sentiments: Highlights key terms associated with depressive sentiments.
Word Cloud for Depressive + Negative Tweets: Combines depressive and negative sentiments to identify recurring themes.
Word Cloud for Positive Tweets: Displays key terms associated with positive sentiment.
Step 4: Building the Model
We applied machine learning techniques to build a sentiment classification model. The key steps in this process were:

Data Splitting: Divided the dataset into training and testing subsets.
Text Vectorization: Transformed text data into numerical format (e.g., using TF-IDF or word embeddings) to input into machine learning models.
Step 5: Testing and Evaluating the Model
After training the model, we evaluated its performance using various metrics, such as precision, recall, and F1-score. The results for the classification of sentiment are summarized below:

Sentiment	Precision	Recall	F1-score	Support
Negative (-1)	0.93	0.70	0.80	430
Neutral (0)	0.78	0.75	0.76	160,202
Positive (4)	0.76	0.79	0.78	161,431
Overall Accuracy	0.77			322,063
Evaluation Summary:
The model achieved an overall accuracy of 77%.
The negative sentiment class showed the highest precision, but a lower recall.
The neutral and positive sentiment classes had more balanced precision and recall scores.
