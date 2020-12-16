# Movie Analysis on Spark

This is the group project of class MSBD5003 BIg Data Computering

Movie Analysis based on Spark

## Introduction
### Background
There are thousands of fantastic movies every year. And many factors will influence the popularity of a movie’s commercialization and revenue. Modeling a movie intrinsic qualities could be a nice challenge. Big data technologies could be a significant tool in researching the movie market. 

### Main Task
This is a Wide project. In this project, we try to make use of multiple Big Data Technologies to observe detailed data generated from over 350,000 movies among 90,000 directors and analyse the relationship between the popularity of movies and many significant factors. Furthermore, we will make predictions of a movie’s score based on the analysis results.

### Dataset
https://www.kaggle.com/stephanerappeneau/350-000-movies-from-themoviedborg

### Technologies
Distributed file system

Dataframe

SparkSQL

SparkML

Graphframes

### Environment
Platform: Azure Databricks

Framework: Spark

API: Python

Libraries: graphframes, mlflow, xgboost, etc.

## Conclusion
In this project, we analysis movie data through Spark. In order to explore the latent laws of the film industry, there are three tasks have been completed, including movie popularity and score prediction, movie genre classification and generating relationship graph of staff. 

For the first task: movie popularity and score prediction, we can predict the both of them correctly with about 0.8 mse. We observed that the reputation of one movie is not easy to predict if only focus on the normal attributes. We speculate that it’s because the content of the movie is really important, and the public aesthetic is not uniform. The features like tagline, budget, director awards number have limited support for movie reputation.

With regard to movie classification, it is hard to classify directly since movies often have multiple genres, and the genres are very diverse and chaotic, there are 22 kinds in total. Moreover, the samples are very unbalanced. If only consider about the first genre of movies, our model can only achieve 36\% accuracy in this 22-class classification task. Besides, we tried clustering task based on K-means, when k is equal to 5, the Silhouette Score is over 0.7, which is the best result.

In terms of relationship graph generation, we exploded the relation between directors, actors and producers. In addition, this complex and huge network of relationships is stored in the form of graphs, and the partnerships between staff can be easily searched and visualized.
