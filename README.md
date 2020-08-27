# credit card fraud detection  
finding fraud under credit card is not easy , so in this folder i have two file one is sampling of credit card data and second is training the model to find the best accuracy.
# Data
data is downloaded from kaggle .
# Aim
to find the fraud , while keeping the outliers in mind.
# 1 -sampling
when ever we have less data , which is very bad signal for model , or if we less data plus imbalanced data too .Then its very bad scenario that model will perform will best .
so in this case im perfoeming smapling in data , sampling is of 3 type under smapling, over sampling, ratio sampling.
Sampling is a method that allows us to get information about the population based on the statistics from a subset of the population (sample), without having to investigate every individual.
# Why do we need Sampling?
Sampling is done to draw conclusions about populations from samples, and it enables us to determine a population’s characteristics by directly observing only a portion (or sample) of the population.
# libraries
      from imblearn.combine import SMOTETomek #over sampling
      from imblearn.under_sampling import NearMiss #under sampling
      from imblearn.over_sampling import RandomOverSampler #ratio sampling 
   
# 2 -credit card model
in credit card i have 30 features under which we have time , amount and labeled data is present that is 0 and 1 , 0 means not fraud and 1 means fraud,
so first i have checked number of fraud and non fraud and count them with respect to users , then checking the how much fraud or non fraud is done by each id ,
and further checking the realtion with amount , that how much time in second is taken by each id to do fraud and at last normalzing data to fit into model.
# libraries for model
      pandas
      numpy
      seaborn
      matplotlib
      from sklearn.preprocessing import StandardScaler
      from sklearn.linear_model import LogisticRegression
      precision,recall,accuracy score
      from sklearn.metrics import classification_report
# Model used 
logistic model (0-1)
# Result
99.9 % 
# Conclusion
 detailed conclusion has been provided in the creditcardfraud.ipynb  and sampling.pynb
