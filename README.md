# Sentiment-Analysis
Sentiment Analysis of a large-scale data set using NLP, classification models, and Dask. 

The dataset is available at https://snap.stanford.edu/data/web-FineFoods.html.
- The dataset contains over 5 million records of review left on Amazon.com for "Fine foods". The records are formatted in JSON and encoded as cp1252.
- The reviews also contain a 1 to 5 star review for the records. For this analysis, reviews with >3 start are "positive" and <3 are "negative".

The overall objective is to classify the reviews as "positive" or "negative" based on the text of the reviews using NLP (binary vectorization)
 and three different classification models.
 
Included here are:
1) Jupyter notebook containing the analysis
2) Cleaned_Dataset that contains .zarr files of the dataset post NLP processing

The notebook is broken into four parts:
 1) Data cleaning and pre-processing
 2) Natural Language Processing (Tokenization) and Binary Vectorization
 3) Modelling (Logistic Regression, Bagged Decision Trees, Random Forests)
 4) Discussion
 
The overall results:
- The combination of binary vectorization and Random Forest classification results in a model that correctly classifies 87-88% of the reviews. 
- Random forest does better than either the Logistic Regression (with hyperparameter tuning) or Bagged Decision Trees. 
