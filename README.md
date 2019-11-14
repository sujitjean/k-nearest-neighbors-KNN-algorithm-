# k-nearest-neighbors-KNN-algorithm-
In the journey of exploring the flown of Data science and predictivemodeling, I explored this Very interesting algorithm k-nearest neighbors (KNN) algorithm.I have tried to leverage the ability of the Classification algorithm whichcomes under Supervised learning of Section of predictive modeling. I used the KNN algorithm for the classification of approvalrate of the projects submitted by the teachers of the United states for students.The main business context of the project was to reduce the manualevaluation of the projects that were done by volunteers as the process of evaluationcan take a long time, which may also be based on some factors and some irreducibleerrors could also be introduced into the processes. Some other import points are.·      How to scale current manual processes andresources to screen 500,000 projects so that they can be posted as quickly andas efficiently as possible·      How to increase the consistency of projectvetting across different volunteers to improve the experience for teachers·      How to focus volunteer time on the applicationsthat need the most assistance.The goal of the project is to predict whether or not aDonorsChoose.org project proposal submitted by a teacher will be approved,using the text of project descriptions as well as additional metadata about theproject, teacher, and school. DonorsChoose.org can then use this information toidentify projects most likely to need further review before approvalThe steps followed for Data Preparation and PredictiveModeling is as follows:Note: Giving Unstructured data (Garbage in common terms) toa machine-learning algorithm gives you random data (Garbage) again. All the code is written in a very clean and untestablemanner ignoring fancy methods where ever possible and reference for everything thatis used in coding is given above the code so that is it easy for everyone tounderstand the code and leverage the potential that AI has because I believein growing together and helping others as this makes me a great team player. Italso increases the storytelling ability and to represent data.For the implementation of all the code, I have used the SKlearn Library.  1.      Apply KNN (brute force version) on thesefeature sets1.      I have formed the different sets of thedata for checking which Vectorization of the text data works better than others.Set 1: categorical, numericalfeatures + project title (BOW) + preprocessed essay (BOW)Set 2: categorical, numericalfeatures + project title (TFIDF)+ preprocessed essay (TFIDF)Set 3: categorical, numericalfeatures + project title (AVG W2V) + preprocessed essay (AVG W2V)Set 4: categorical, numericalfeatures + project title (TFIDF W2V) + preprocessed essay (TFIDF W2V)2.      Hyperparameter tuning to find best K andMetrix used for evaluation of the model. 1.      Find the best hyperparameter which results inthe maximum AUC value2.    Find the best hyperparameter using k-foldcross-validation (or) simple cross-validation data3.  Use grid search-cv or random search-cv or write your own for loops to dothis task 3.      Representation of results1.      Plotting the performance of model both on traindata and cross-validation data for each hyperparameter.  2.      Once you find the best hyperparameter, you needto train your model-M using the best hyper-param. Now, find the AUC on testdata and plot the ROC curve on both train and test using model-M. 3.      Along with plotting ROC curve, you need to printthe confusion matrix with predicted and original labels of test data points  4.      . Select top 2000 features from the featureSet 2 using `SelectKBest` and then apply KNN on top of these features(this thesection wherein we select the best features from all the features we have)1.      Repeat the steps 2 and 3 on the data matrixafter feature selection 5.      Conclusion1.      Summarize the results at the end of thenotebook, summarizing is done in the table format.      
