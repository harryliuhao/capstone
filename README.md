## links I researched to build the n-gram model
https://github.com/j-wang/DataScienceCapstone/blob/master/final/TestingModels.Rmd

##Note 2/20/2017
###Statistics from 50% sample 
1. data cleaning time (tm_map) is 23 mins (1380 sec)
2. Tokenization time is 128 mins and counting when interrupted (2+ hours) for just bi-token. Too long. 

##Next steps
* test if breaking down documents to sentences will speed up the tokenization process
* test what's the best method to break down documents
* test if release memory will reduce the crash during tokenization
* If above steps don't work, test the sample size at 20%, and how does it answer the question of 90% word etc.
