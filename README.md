# NLPHotelReview

1. Tokenize the data
use split to split all the words, i.e. df['Positive'].str.split(' ')
2. Take the tokenized corpus/file and make document term matrix using the bag of words model  == CountVectorizer()

### 1. Instantiate 
bagofwords = CountVectorizer()

### 2. Fit 
i.e.,bagofwords.fit(small_reviews["Review"])

### 3. Transform
i.e., small_transformed = bagofwords.transform(small_reviews["Review"])
 i.e.,small_transformed

### 4. bagofwords.get_feature_names_out()


### 5. converting the sparse matrix into a numpy array
i.e., small_transformed.toarray()

### 6.  We can extract the information and put it in a data frame to make it easier to see what has occured
i.e., my_df = pd.DataFrame(columns=bagofwords.get_feature_names_out(), data=small_transformed.toarray())
 i.e., display(my_df)

### Using a pipeline, combine PCA with a decision tree classifier.

Logistic Regression Accuracy: 0.7277908343125734
Decision Tree Accuracy: 0.7198589894242068

ROC-AUC with no sampling -- 0.8381
ROC-AUC with SMOTE -- 0.8666

| |recall|precision|f1|
|-|------|---------|--|
|**logreg on unsampled data**|73.0%|82.3%|0.77%|
|**logreg on SMOTE-sampled data**|81.6%|81.2%|0.81%|
