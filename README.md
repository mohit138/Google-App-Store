# Google-App-Store

The data consists of various apps from Play store, with features like, Category, Size, Downloads, Genre, Reviers, Type, Price, Android Version, etc. I use this data to train, various models to predict rating of Various apps. 
Initially data was preprocessed and made suitable for training. Label Encoding of various features was done. Otheres were converted into mathematical data from string data. 

Histogram of Rating :

<img src="https://github.com/mohit138/Google-App-Store/blob/master/images/rating_hist.png" alt="drawing" width="500"/>

Features Before Pre-processing :
'App', 'Category', 'Rating', 'Reviews', 'Size', 'Installs', 'Type','Price', 'Content Rating', 'Genres', 'Last Updated', 'Current Ver','Android Ver'
Features After Pre-processing :
'Category_Label', 'Rating', 'Reviews_Log', 'Size', 'Installs_Size','Type_Label', 'Price_Num', 'Content_Rating_Label', 'Android_Ver'

Pairplot of processed features :
![alt text](https://github.com/mohit138/Google-App-Store/blob/master/images/pairlot.png?raw=true)

MAE and MSE were used as metrics for analysing accuracy of various Models. Sklearn was used to implement Linear Regression, Decision Tree and Support Vector Regression. 
Later Tensor Flow was also used to implement Neural Network. 
Results obtained were not upto mark, because there is a bias in data provided. No. of datas with a rating between 3.5-4.4 are too much in no. This results in a non-uniform data which results in biased training. To improvise this, we need to increse no of apps with ratings below 3.5.
