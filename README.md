# Out of 20 newsgroups category which does this document belong to ?
Context - This is a text classification problem where we have 20 newsgroup document collection (approx 20k)
Approach- 
1. Clean and Collect all the non-stop words having length ? 3 - 
   1.1 Go through all 20k documents
   1.2 Within a doc, go throgh all the words
   1.3 Ignore a word if it is a stop word or length <=3
   1.4 Append the cleaned list of words with category of doc
2. Now you have tokenized and cleaned your data. Next step is to spilt your data into train and test (14000,6000) in order to test your model from your end.
3. Now we are going to make BoW/ vectorize our text - 
   3.1 Take your training data and count each word
   3.2 Take 2000 top words, (why ? beacause these 2k words are going to be our features)
4. Create BoW with the help of these 2k words
5. Apply MultiNomial Naive Bayes Algorithm (from scratch or use sklearn libraby)
6. Score - Classification report, Accuracy
