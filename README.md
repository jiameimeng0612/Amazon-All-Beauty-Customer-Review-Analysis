# Amazon-All-Beauty-Customer-Review-Analysis
I chose Amazon Customer Review Dataset under All Beauty category. The data in this category includes 371,345 reviews and metadata including descriptions, price, sales-rank, brand information, and co-purchasing links for 32,992 product.
* With the embedding file “word2vec-google-news-300”, which is used skip-gram architecture for computing vector representations of words, the sentiment analysis is performed on the content of review text of Amazon All Beauty customer reviews. 
* Then, the reviews are converted to vectors by averaging the vectors of words of each customer’s review content. Meanwhile, BOW is used as another embedding method in this project as well.
* In this work, logistic regression and random forest are used to build classification models, and multiple metrics, including AUC, accuracy and f1 score, are used to measure the performances of classifiers. The logistic regression model with BOW performs the best among four models. 
* By using LIME, the predictions of logistic regression model with BOW and random forest model with BOW are explained with the same instance in the test set. It’s found that logistic regression model performs better than random forest model with the explanation on the instance.
