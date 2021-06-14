# Flatiron Phase 4 Project - Twitter Sentiment NLP Predictive Model

## Business Problem
A smartphone consortium led by Apple and Google want to prove via a 2-week proof-of-concept whether Twitter data can be used to detect sentiment with the highly desirable consumers at SXSW.

Requirements:
- Develop predictive model to classify tweet sentiment
- Explain performance and any limitations for positive and negative model predictions
- Suggest potential solutions and next steps to evolve beyond a POC model

## Project Deliverable
The project involved analyzing, cleansing, natural language processing, featurizing and modeling roughly 9K Twitter tweets about Apple or Google technology during the music event South-by-Southwest. Tweets were cleaned and tokenized, and four models were developed: 1) Support Vector Machines, 2) Neural Network - Sequential LSTM w/ Embeddings, 3) Same as 2 but against tokens, and 4) Neural Network bi-directional LSTM with gloVe embeddings. Each model was trained on 68% of the historical data, using 12% as validation (to total 80% for model development). I predicted sentiment on the remaining 20% test data. I used the tools and libraries from Python, Numpy, Pandas, Seaborn, Scikit Learn, Keras, NLTK, spaCy, among others. Here you can find my [final business presentation][1] and my final [Jupyter notebook][2].

## Repository Contents
Below is a list of the contents of this repository - instructions for using them are in the next section.

- README.md: The README for this repo branch explaining it's contents - you're reading it now.
- Twitter-Sentiment-Analysis-NLP.ipynb: Jupyter Notebook containing data sources, Python scripts, data engineering, analysis, feature engineering and models.
- Tweet_Sentiment_Analysis_Exec_Summary.pdf: Final business presentation targeting a 5-minute summary pitch
- data folder: Folder contains source data files as well as the best models saved from fitting and optimization
- images folder: A folder for some images of plots used in presentation
- .gitignore: A hidden file that tells git to not track certain files and folders


[1]: <https://github.com/cutterback/p04-twitter-sentiment-nlp/blob/2e65c792fe16bcd162b053ff61f23ca6f35d46de/Tweet_Sentiment_Analysis_Exec_Summary.pdf> "Twitter Sentiment Analysis Executive Summary"
[2]: <https://github.com/cutterback/p04-twitter-sentiment-nlp/blob/2e65c792fe16bcd162b053ff61f23ca6f35d46de/Twitter-Sentiment-Analysis-NLP.ipynb> "Jupyter Notebook Twitter Sentiment Prediction Model" 
