# Movies-ETL

# Project Overview
## The moving wikipedia data set in json format is very messy. In this case, the data clean process includes label consistency, such as changing 'Country of origin' to 'Country', unifying numbers in one format and formatting numeric data for later usage. 

## Method 
## In this case, the numeric data processed are budget, boxoffice, runtime and date. regular expressions are used to extract certain formats of budget and box office data. The number formats are in string type, some of them are in US dollars, some of them are in million units and some of them are in billion units. two forms of regular expression are formed to capture and transform into float numbers that can be analyzed. 
## Example 
### Before Transformatting
![](https://github.com/ftjyangf/Movies-ETL/blob/master/pic/originalbudget.PNG) 
### After transformatting ![](https://github.com/ftjyangf/Movies-ETL/blob/master/pic/boxoffice.PNG)


## cleaned and transformed wiki_moive and kaggle rating data are merged together into a big dataset. This big dataset is loaded into the postgres database by using the postgres API. The Extract, Transform and Load pipeline processes are constructed!

## Result
![](https://github.com/ftjyangf/Movies-ETL/blob/master/pic/uploading.PNG)
## This data has more than 2,600,000 rows and it took almost 1 hour to load into our database for later usage!

