# SC1015_Hit_Song_Predictor
## About 
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on audio features of songs from [Spotify API](https://developer.spotify.com/documentation/web-api/reference/#/operations/get-several-audio-features). For detailed walkthrough, please view the source code in order from:

1. [Data Extraction and Cleaning](https://github.com/Zhiyang123/SC1015_Hit_Song_Predictor/blob/main/Audio_Features.ipynb)
2. [Data Visualisation, Exploratory Data Analysis, Machine Learning]

## Contributors

- @YinJiann - 
- @Zhiyang123 - 
- @lawminghan - 

## Problem Definition 

- Our group intends to investigate the relationship between audio features and popularity of spotify tracks. For established artists, they can use this algorithm to assist and guide them in replicating their previously successful hits. For upcoming or new artists, they can use this algorithm to decide on which audio features they can focus on in order to maximise their likelihood of releasing a hit song. 

## Models Used
1. Multivariate Linear Regression Model 
2. Isolation Forest
3. Single Decision Tree
4. Random Forest 
5. Logistic Regression Model

## Conclusion 

- We started off investigating the individual correlations between audio features and popularity. THe resultant low correlation across the board make it obvious that our question could not use a regression model (linear and multivariate). Hence, we decided to approach from a different angle, it could perhaps be a classification problem. We went with decision trees and logistic regression. 
- From the analysis of the classification accuracies across all the classification models, we can conclude that Logistic Regression model performed the best compared to all other classification models. Although outliers were removed using the Isolation Forest as well as pre-pruning to regularise the data, there were still overfitting in the classification models. In contrast, based on the classification accuracies of train and test set for Logistic Regression model, overfitting was significantly reduced, while also improving the classification accuracies on the test set. Thus, we can conclude that Logistic Regression performed the best among the classification models used in the project. 

## What did we learn from this project?

- Spotify API and Spotipy 
- Isolation Forest (remove outliers)
- Pre-pruning (regularisation)
- Logistic Regression model 
- Other packages such as Spotipy, sklearn.metrics (roc_auc_score)
- Collaborating using GitHub

## References

- <https://developer.spotify.com/documentation/web-api/reference/#/operations/get-several-audio-features>
- <https://towardsdatascience.com/outlier-detection-with-isolation-forest-3d190448d45e>
- <https://towardsdatascience.com/introduction-to-logistic-regression-66248243c148>
- <https://towardsdatascience.com/understanding-auc-roc-curve-68b2303cc9c5>
- <https://scholar.smu.edu/cgi/viewcontent.cgi?article=1041&context=datasciencereview#:~:text=In%20general%2C%20logistic%20regression%20performs,variables%20increases%20in%20a%20dataset>
