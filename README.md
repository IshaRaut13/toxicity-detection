# Toxic-Comment-Detector
This project applies classification models with the aim of automating the detection of toxic comments on social media.

## Modeling:
Three main Machine Learning classification models are used:
* Multinomial Naive Bayes
* Logistic Regression
* Support Vector Machine (SVM)

According to the results, Naive Bayes classifier with TfidfVectorizer came with the best f1 score and recall: 0,85 and 0.88, respectively.
Because of this reason, it was used as the base model of the web application. 

## Full results: 
|       Models       | precision   | recall   | f1 score |
| -----------------  | ------------| ---------|----------|
|Multinomial NB      |    0.82     |   0.88   |   0.85   |
|Logistic Regression |    0.82     |   0.80   |   0.81   |
|SVM                 |    0.82     |   0.83   |   0.83   |

## Data:
Data for this project was obtained from the GitHub repository of [SurgeAI](https://github.com/surge-ai/toxicity), a powerful NLP data labeling platform.

### Data Description:
* Dataset consists of 1000 English examples gathered from different popular social media platform. 
* Each 500 examples in it are labeled as "toxic" and "non-toxic", respectively. 
* #### Columns:
  * ``` text ```: the text of the social media comment
  * ``` is_toxic```: whether the text is toxic or not
