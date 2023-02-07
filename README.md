# Movielens-Analysis
Analyzing movielens dataset using Azure databricks

The objective of this project was to generate movie recommendations using the combination of Python and Spark on Microsoft Azure. To start, I first understood the problem and downloaded the Movielens dataset from the GroupLens website. Then, I set up a subscription for Microsoft Azure, organizing my resources into a resource group.

I created a standard storage account to store all the necessary data for the movie recommendation system. This was followed by the creation of a standard storage blob account within the same resource group. I created containers within the standard storage account and the standard storage blob account and uploaded the Movielens zip file dataset into the standard storage blob account.

Next, I created an Azure data factory and a copy data pipeline to begin linking the standard blob storage account to the Azure data factory. Using the copy data pipeline in the Azure data factory, I copied the data from the Azure blob storage to the Azure data lake storage.

I then created the Databricks workspace and cluster and accessed the Azure data lake storage from Databricks. I created mount points and extracted the zip file to get the CSV files. Finally, I uploaded the files into Databricks, read the datasets into Spark dataframes, and analyzed the dataset to generate the movie recommendations.
