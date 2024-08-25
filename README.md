# NLP Amazon Reviews

## Introduction

For my final project in my Machine Learning course, I chose the "Amazon Product Reviews" dataset from Kaggle. This dataset contains 21,000 reviews evenly distributed across five ratings. Driven by my interest in natural language processing, my objective was to use machine learning to predict the ratings based on the written reviews.

## Importance & Use of Machine Learning

Product reviews are invaluable not only for potential customers who rely on them to make informed purchasing decisions but also for businesses seeking to enhance their products and customer service. By analyzing review data, businesses can gain deep insights into customer sentiment, identifying strengths and weaknesses in their products. Machine learning is particularly powerful in this context because it allows for the automation of sentiment analysis, making it possible to monitor reviews in real-time. This capability enables businesses to quickly identify trends, such as a sudden increase in negative reviews, and take corrective actions as needed. For my project, I aimed to demonstrate how machine learning can be tailored to understand and predict customer sentiment, providing businesses with a tool to improve their products and services continuously.

## Techniques

I began the project by thoroughly preprocessing the data. This step was crucial in ensuring the quality of the analysis. I standardized the text data by converting it to lowercase, tokenizing the text, and removing punctuation. I also addressed the issue of data duplication—69% of the dataset consisted of duplicate reviews—by filtering out these duplicates and non-English samples. This cleaning process was essential in ensuring that the models would not be biased by repeated data or irrelevant content.

After preprocessing, I conducted exploratory data analysis (EDA) to uncover patterns and insights within the data. I used sentiment analysis with the TextBlob library, which is effective in processing textual data and assigning sentiment polarity values. I categorized the sentiment of the reviews as positive, neutral, or negative and visualized the results in both binary and multiclass formats. Additionally, I employed the CountVectorizer tool from scikit-learn to perform feature extraction, identifying the most common words in positive and negative reviews. This analysis revealed interesting patterns, such as the frequent appearance of words like "good" and "great" in both positive and negative reviews, highlighting the importance of context in sentiment analysis.

## Modeling

With the data preprocessed and analyzed, I moved on to building and training machine learning models. I split the dataset into training and testing sets to evaluate the models' performance accurately. Given the uneven distribution of ratings discovered during EDA, I used SMOTE (Synthetic Minority Over-sampling Technique) to address the class imbalance in the training data. This step was critical in ensuring that the models could learn effectively from the minority classes.

I explored both binary and multinomial classification approaches, using a variety of models including Logistic Regression, K-Nearest Neighbors (KNN), Random Forest, Gradient Boosting, Multinomial Naive Bayes, and Multilayer Perceptron (MLP). Among these, Logistic Regression consistently delivered the best results in both binary and multinomial classifications. This was likely due to its ability to effectively model the relationship between the input features and the output labels, especially in the case of binary classification.

## Conclusions

The outcomes of my project highlighted the significant role that machine learning can play in sentiment analysis and customer feedback interpretation. The higher accuracy achieved with binary classification underlined the challenges posed by class imbalance, which can be mitigated through techniques like SMOTE. Logistic Regression emerged as the most effective model, particularly in its ability to handle the linear relationships in the data. My project demonstrates that with a well-prepared dataset, machine learning can provide businesses with powerful tools to better understand and respond to customer needs, ultimately enhancing product performance and customer satisfaction.
