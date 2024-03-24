# Building a Movie Recommender System 

This is a data engineering project for movie suggestions based on [MovieLens](https://grouplens.org/datasets/movielens/) raw dataset. It is built using below mentioned Azure services.

1) Azure blob storage
2) Azure data lake storage gen2
3) Azure Data Factory
4) Azure databricks
5) Azure Synapse Analytics

The Architecture Diagram for this project is shown below - 
</br>

<img src=./images/Architecture_Diagram.png width="700" height="500">

</br>
I have used azure data factory as a orchestration tool for building and executing data pipeline. The main tasks involved are - 

</br>

1) Data cleaning using ADF's data flow by removing duplicate rows and null values and ingesting them to Azure data lake storage gen2 in parquet format.
2) Data transformation in azure databricks by calculating Bayesian average ratings and top 5 tags for each movie using spark SQL.
3) Data analysis and best movie by genre or rating calculations in Azure synapse analytics.

</br>


<img src=./images/Pipeline.png width="900" height="600">

