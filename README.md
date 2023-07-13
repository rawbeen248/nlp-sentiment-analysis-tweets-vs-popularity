# Sentiment Analysis and Twitter Post Popularity: A Data-Driven Investigation of the Correlation

Main goal of this research is to investigate the corrleation between sentiments of the tweets of popular people with its popularity (number of likes and shares).

For this project two different datasets are used. One is labeled (0 and 1 for positive and negative sentiments respectively) dataset and the other one is unlabeled dataset. There is no single dataset with labels and the features required for this investogation therefore this approach is taken.

Main features wrequired in a single dataframe to conduct this research are: tweet text, number of likes for that tweet, number of shares for that tweet and the sentiment score for that tweet so that correlation could be computed. As it was not possible to conduct the research using single dataset, the following steps are followed:

1. After performing all the required preprocessing of the data, a classifcation model on the labeled dataset is trained.

2. Then that trained classification model is used to predict the labels for the unlabeled dataset along with sentiment score which in this case is computed using predict_proba function of the classifier model.

3. Then the popularity score is computed using the features: number of likes and number of shares.

4. Finally linear and non-linear correlation between the populariy and the sentiment score is computed.

The steps are explained along with the code in more details on the notebook.

#### Datasets used: 
___
* Training Dataset: Dataset from Sentimnet140 (link: https://docs.google.com/file/d/0B04GJPshIjmPRnZManQwWEdTZjg/edit?resourcekey=0-betyQkEmWZgp8z0DFxWsHw)

* Main Dataset: Available along with the notebook. 

#### Libraries: 
___
You can find all the required libraries in requirements.txt file. And install those through terminal with this command:</br>
!pip install -r requirements.txt
