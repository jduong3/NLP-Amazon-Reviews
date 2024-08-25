# NLP Amazon Reviews

For my final project in my Machine Learning course, I chose the "Amazon Product Reviews" dataset from Kaggle. This dataset contains 21,000 reviews evenly distributed across five ratings. Driven by my interest in natural language processing, my objective was to use machine learning to predict the ratings based on the written reviews.

Product reviews are valuable not only for potential customers but also for businesses, offering insights into product improvement. Machine learning is crucial for real-time sentiment analysis, allowing businesses to detect shifts in customer sentiment and respond accordingly.

I started by preprocessing the data, standardizing the text, and filtering out duplicates and non-English samples. I then moved on to exploratory data analysis, including sentiment analysis using TextBlob and feature extraction with CountVectorizer. I categorized ratings into binary and multiclass cases, analyzing the sentiment polarity and common words used in reviews.

To address the issue of uneven data distribution, I used SMOTE and trained various machine learning models for binary and multinomial classification. Logistic Regression emerged as the best-performing model in both cases.

My results demonstrated the effectiveness of machine learning in sentiment classification, particularly with Logistic Regression. This project highlights the potential of machine learning in enhancing business performance, especially with well-balanced datasets.


