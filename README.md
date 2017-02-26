## links I researched to build the n-gram model
https://github.com/j-wang/DataScienceCapstone/blob/master/final/TestingModels.Rmd
https://rpubs.com/LL8054/MilestoneReport  
http://rpubs.com/bhaskarp/137200  
https://www.kaggle.com/enrique1500/integer-sequence-learning/predict-oeis-with-ngrams-1  
https://github.com/kbenoit/quanteda/issues/46  

##Note 2/20/2017
###Statistics from 50% sample 
1. data cleaning time (tm_map) is 23 mins (1380 sec)
2. Tokenization time is 128 mins and counting when interrupted (2+ hours) for just bi-token. Too long. 

##Next steps
* test if breaking down documents to sentences will speed up the tokenization process
* test what's the best method to break down documents
* test if release memory will reduce the crash during tokenization
* If above steps don't work, test the sample size at 20%, and how does it answer the question of 90% word etc.

##Note 2/25/2017
1. Sentence detect accomplished with quanteda package
2. data cleaning and tokenization dramatically quickened using quanteda package. Expanding to SparseMatrix no longer causes memory issue.
3. 50% sample only takes 20 mins. It will be possible to process the entire doc if necessary.

##Next steps
* how to aggregate dfm into a frequency, so it can be formatted into a dictionary
* or dfm can be used directly for textmodels
* ngrams may need to be separated before Markov backoff model can be appled. Right now I have different levels of ngrams in one dataset
* use topfeatures to extract the frequency table
* build the table to split n-grams to (n-1) grams + predicted word
* save the table on harddrive for prediction program
* modify the program to apply one sentence for testing dataset
* Predict
