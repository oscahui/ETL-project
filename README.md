# ETL-project

Team members: Zheng Qi, Oscar Hui, Chad Melenaar, Joe Quin

## Overview

This project aims to help gamers and game publishers/developers access data through SQL/MongoDB to better understand and/or for analyses for information such as game sales/genre popularity etc.

This project will be done in two parts. Part one focuses on the populartiy information of publisher/genres/price of different games. Part two focuses on the relationship between game regional price and region GDP.

The program should be run as the following order:

* Part_One_GameGenres_and_Feedback-DataExtraction
* Part_One_GameGenres_and_Feedback-TransAndLoad
* Part_Two_Steam_Game_Price_Index

## Data source

The dataset is extracted from the several APIs and Kaggle.com with formats of json or csv.

* [Steamspy](https://steamspy.com/api.php)

* [Steamstore](http://store.steampowered.com/api/appdetails/)

* [Foreignexchangerates](https://exchangeratesapi.io/)

* [isthereanydeal](https://api.isthereanydeal.com/)

* [Kaggle](https://www.kaggle.com/)

The dataset includes the information of publisehr/developer/comments number/playtime/genres for games and also the regional price information of most popular games with corresponding region GDP.

The extracted data formart are mostly json style, which is stored as csv or json format on local machine for later transfomration processes, depending on the structure of extracted information.

The ERD of different datasets can be find in Part_One_ERD.png and Project_ERD_Part_One_and_two.png.

## Data transformation

Different transformation processes are applied to the datasets. Two final tables for two parts are generated to investigate the relationship between different variables.

## Data load

The data/results are loaded to MongoDB due to the different structures of data.
The final output data is also saved in json/csv files for easier grading.
