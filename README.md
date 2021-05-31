# Movies-ETL

# Project Overview
## The moving wikipidea data set in json format is very mess. In this case, the data clean process includes label consistence, such as changing 'Country of orgin' to 'Country', unifing number in one format and reformting numeric data for later usage. 

## Method 
## In this case, the numeric data are processed are budget, boxoffice, runtime and date. regular expression are used to extract certain format of budget and boxoffice data. the number format are in string type, some of them are in US dollar, some of them are in million unite and some of them are in billion unite. two form of regular expression are formed to capture and transform into float number can be analyzed. 
## Example 


## cleaned and transformed wiki_moive and kaggle rating data are merged together into a big dataset. this big dataset are loaded into prostgres database by using postgres API. the Extract, Transfrom and Load pipline process are constructed!

## Result
