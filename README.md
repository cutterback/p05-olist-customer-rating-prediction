# Flatiron Capstone Project - Olist Bad Customer Reviews Predictive Model

## Medium Blog Post - Towards Data Science

For a narrative summary and key insights on this project, please read my blog post [Using Data Science to Predict Negative Customer Reviews][3] on Medium.

## Business Problem
Kaggle contains a Brazilian ecommerce public dataset of orders made at Olist Store. This dataset was generously provided by Olist, the largest department store in Brazilian marketplaces. Olist connects small businesses from all over Brazil to channels without hassle and with a single contract. Those merchants are able to sell their products through the Olist Store and ship them directly to the customers using Olist logistics partners.

The dataset has information of 100k orders from 2016 to 2018 made at multiple marketplaces in Brazil. Its features allows viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. Olist also released a geolocation dataset that relates Brazilian zip codes to lat/lng coordinates. This is real commercial data, it has been anonymised, and references to the companies and partners in the review text have been replaced with the names of Game of Thrones great houses. The data for this project was sourced from Kaggle:

https://www.kaggle.com/olistbr/brazilian-ecommerce/home (9 tables)

https://www.kaggle.com/olistbr/marketing-funnel-olist (2 tables)

For this project, we'll be analyzing and trying to predict bad customer reviews. Customer reviews range from 1 (worst) to 5 (best). We have defined bad review as either a 1 or 2 review score which when combined represent 13.2% of all reviews. Our business objective includes the follow requirements:

- Understand dynamics that cause customers to leave a bad review
- Find the best prediction model to classify a bad review from a customer
- Deliverables should explain the relative influence of each predictor on the model
- Deliverables should suggest potential solutions to preventing bad customer reviews

## Project Deliverable
The project involved analyzing, cleansing, featurizing and modeling roughly 100K orders and customer reviews. Seven classification models were developed: 1) Random Forest, 2) AdaBoost, 3) Gradient Boost, 4) Logistic Regression, 5) SGD Classifier, 6) Gaussian Naive Bayes, and 7) XG Boost. Each model was trained on 80% of the data using 5-fold cross-validation to prevent overfit. We then comparatively scored our models on the remaining 20% unseen test data. I used the tools and libraries from Python, Numpy, Pandas, Seaborn, Scikit Learn, XGBoost, among others. 

Here you can find my [final business presentation][1] with conclusions and my final [Jupyter notebook][2] which contains all the data transformations and modeling results.

## Repository Contents
Below is a list of the contents of this repository - instructions for using them are in the next section.

- README.md: The README for this repo branch explaining it's contents - you're reading it now.
- Olist_Customer_Rating_Model.ipynb: Jupyter Notebook containing data sources, Python scripts, data engineering, analysis, feature engineering and models.
- Olist_Bad_Customer_Reviews_Prediction.pdf: Final business presentation targeting a 5-minute summary pitch
- data folder: Folder contains source data files from above Kaggle links
- images folder: A folder for some images of plots used in presentation
- tableau folder: Contains a primary Tableau workbook and .hyper file, alongside a few smaller workbooks used for visualizations.
- .gitignore: A hidden file that tells git to not track certain files and folders


[1]: <https://github.com/cutterback/p05-olist-customer-rating-prediction/blob/532920f813e90bc82f08f861534836ec2b578054/Olist_Bad_Customer_Reviews_Prediction.pdf> "Olist Predicting Negative Customer Reviews Executive Summary"
[2]: <https://github.com/cutterback/p05-olist-customer-rating-prediction/blob/532920f813e90bc82f08f861534836ec2b578054/Olist_Customer_Rating_Model.ipynb> "Jupyter Notebook Olist Customer Review Prediction Model" 
[3]: <https://towardsdatascience.com/using-data-science-to-predict-negative-customer-reviews-2abbdfbf3d82?sk=a084b6fb96f42291d3db5780dde47108> "Towards Data Science Article - Using Data Science to Predict Negative Customer Reviews" 
