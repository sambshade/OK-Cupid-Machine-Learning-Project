# OK-Cupid-Machine-Learning-Project
The following code analyzes the data of several members of a fictional online dating database. The code examines the distribution of several variables and uses machine learning to attempt to predict religion, body type, and astrological signs based on the other variables.

The columns in the dataset include: 

* `age`: continuous variable of age of user
* `body_type`: categorical variable of body type of user
* `diet`: categorical variable of dietary information
* `drinks`: categorical variable of alcohol consumption
* `drugs`: categorical variable of drug usage
* `education`: categorical variable of educational attainment
* `ethnicity`: categorical variable of ethnic backgrounds
* `height`: continuous variable of height of user
* `income`: continuous variable of income of user
* `job`: categorical variable of employment description
* `offspring`: categorical variable of children status
* `orientation`: categorical variable of sexual orientation
* `pets`: categorical variable of pet preferences
* `religion`: categorical variable of religious background
* `sex`: categorical variable of gender
* `sign`: categorical variable of astrological symbol
* `smokes`: categorical variable of smoking consumption
* `speaks`: categorical variable of language spoken
* `status`: categorical variable of relationship status
* `last_online`: date variable of last login
* `location`: categorical variable of user locations

And a set of open short-answer responses to :

* `essay0`: My self summary
* `essay1`: What I’m doing with my life
* `essay2`: I’m really good at
* `essay3`: The first thing people usually notice about me
* `essay4`: Favorite books, movies, show, music, and food
* `essay5`: The six things I could never do without
* `essay6`: I spend a lot of time thinking about
* `essay7`: On a typical Friday night I am
* `essay8`: The most private thing I am willing to admit
* `essay9`: You should message me if…


# Conclusions: 

* Data visualization proved that some categories tend to have a relationship with the sex of the user, while most do not. 
* The machine learning models used for predicting various user categories proved to be not the most accurate: 
  * For predicting religion, the data was found to be skewed towards four specific religions (Agnosticism, Other, Atheism, Christianity) making the prediction lean towards those options. This can be easily visualized in the confusion matrix heatmap showing that true positives for the other religions aren't as available. The analysis was still conducted and the model with the best results came from the Decision Tree model; however, this model was vastly overfit with a depth of almost 60. The K Nearest Neighbors model would be the most accurate model with a 46% accuracy.
  * For predicting body type, similar results were found to religion with heavy data imbalance towards specific body types. This can be easily visualized in the confusion matrix heatmap showing that true positives for the other body types not as well-represented aren't as available. The analysis was still conducted and the model with the best results came from the Decision Tree model; however, this model was vastly overfit with a depth of almost 60. The K Nearest Neighbors model would be the most accurate model with a 46% accuracy.
  * For predicting astrological signs, the data was not imbalanced as opposed to the data for religion and body type. The analysis was conducted and the model with the best results came from the Decision Tree model; however, this model was vastly overfit with a depth of almost 60. The K Nearest Neighbors model would be the most accurate model with a 33% accuracy. 

# Future Projects:

* Future analysis can try:
    * Capping the depth of the Decision Tree Model to see if there's a better represented model than the KNN model without overfitting for the data. 
    * Providing different machine learning models (ADABoost, Random Forest, etc.) to see if other models better predict religion, body type, and astrological signs.
    * Conducting the same three models for other categorical variables to see if any of these yield better results. 
