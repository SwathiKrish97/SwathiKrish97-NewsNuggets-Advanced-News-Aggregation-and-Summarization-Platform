NewsNuggets-Advanced-News-Aggregation-and-Summarization-Platform

* Overview:
    * "NewsNuggets" addresses the challenge of information overload by providing quick, comprehensible summaries of news articles, categorized by topics and enhanced with sentiment analysis.
      
* Data Collection:
    * Used the BBC Dataset with 2,225 documents across five categories: business, entertainment, politics, sport, and tech.
    * Included sentiment dataset with positive and negative categories.
      
* Data Preprocessing:
    * Steps: tokenization, removal of URLs and punctuation, conversion to lowercase, removal of stopwords, and lemmatization.
    * Used Bag of Words (BoW) and Term Frequency-Inverse Document Frequency (TF-IDF) for text vectorization.
    * Applied SMOTE to balance the dataset.
      
* Model Details and Training:
    * News Category Classification: Implemented Logistic Regression, Decision Tree, Multinomial Naive Bayes, Random Forest, and AdaBoost with BoW and TF-IDF vectors.
        * Logistic Regression with TF-IDF achieved 98% accuracy.
    * News Sentiment Classification: Similar models and methods as category classification.
        * Logistic Regression with TF-IDF achieved 96.6% accuracy.
    * News Summarization: Implemented Word Frequency, TF-IDF, and TextRank Summarization techniques.
        * TF-IDF model consistently outperformed the others.
          
* Experiments and Evaluation Results:
    * News Category Classification: Evaluated using confusion matrix, accuracy, precision, recall, and F1-score.
    * News Sentiment Classification: Evaluated using accuracy, precision, recall, F1-score, confusion matrix, and ROC curve.
    * News Summarization: Evaluated using ROUGE and BLEU metrics.
      
* Deployment:
    * Integrated best models into the "NewsNuggets" application.
    * The app preprocesses, vectorizes, categorizes, analyzes sentiment, and summarizes news articles.
    * Built with HTML5, CSS, and Flask for a responsive UI and robust backend.
      
* Discussion:
    * Achieved high accuracy in category and sentiment classification using TF-IDF vectorization.
    * The TF-IDF summarization technique effectively captures essential content.
    * "NewsNuggets" improves user experience by providing quick and relevant news summaries.
      
* Future Improvements:
    * Enhance accessibility with multi-language support.
    * Incorporate advanced summarization models.
    * Improve infrastructure for scalability.
    * Integrate personalized news summaries.
    * Focus on domain-specific sentiment analysis for deeper insights.
      
* Dataset Source:
    * BBC News Dataset - http://mlg.ucd.ie/datasets/bbc.html
    * News Sentiment Dataset - https://www.kaggle.com/datasets/hoshi7/news-sentiment-dataset
