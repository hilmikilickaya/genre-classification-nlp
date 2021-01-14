# Genre Classification

<p align="center">
  <img width="800" height="420" src="https://github.com/hilmikilickaya/genre-classification-nlp/blob/main/images/band_wc.png">
  </p>
  
  Music tells us a lot about who we are.  Spotify says you are what you stream. I like music apps and always find it impressive how they make it easier for us to create playlists by the genre. I wanted to know if I could create a classification model with lyrics using Natural Language Processing?
  
## Data
  My dataset contains over five thousand songs and six genres. After plotting songs by genre, I figured that I have an imbalanced class. I decided to remove electronic dance music to have a better model.
 <p align="center">
 <img width="580" height="400" src="https://github.com/hilmikilickaya/genre-classification-nlp/blob/main/images/genres_count.png">
 </p>
  
## Tf-idf
  I started my cleaning process. I lowercase the text and then tokenize, strip out undesirable text, removing stop words, and lastly lemmatize it. After cleaning the text data I vectorize my bag of words.
<p align="center">
  <img width="480" height="410" src="https://github.com/hilmikilickaya/genre-classification-nlp/blob/main/images/most_common.png">
</p>

## Random Forest Classification
Random forests or random decision forests are an ensemble learning method for classification, regression, and other tasks that operate by constructing a   multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean/average prediction (regression) of the individual trees.

After trying a few models for classification like Scoasthic Gradient Descent, logistic regression, I decided to go with Random Forest Classifier. I got almost 60 percent accuracy, but I realized that my model does not make predictions well for pop and rock songs. I  investigated a few misclassifications I found out there are a lot of common words between rock on pop songs. There is conflicting about how people label song genres.
  
  <p align="center">
  <img width="600" height="420" src="https://github.com/hilmikilickaya/genre-classification-nlp/blob/main/images/base_heatmap.png">
  </p>
  
 ## Feature Importance
 Feature importance refers to a class of techniques for assigning scores to input features to a predictive model that indicates the relative importance of each feature when making a prediction.
  <p align="center">
  <img width="460" height="300" src="https://github.com/hilmikilickaya/genre-classification-nlp/blob/main/images/base_feature_imp.png">
  </p>
 
