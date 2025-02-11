Data Analysis of Anime Records
This project involves data analysis on a dataset of anime records. The analysis is performed using Python and Jupyter Notebook, leveraging libraries such as Pandas, NumPy, Seaborn, and Matplotlib.

Table of Contents
Introduction
Dataset
Libraries Used
Analysis Steps
Results
How to Run
Contributing
License
Introduction
The aim of this project is to analyze anime records to gain insights into various attributes such as ratings, popularity, and other characteristics. The analysis helps to understand trends and patterns within the anime dataset.

Dataset
The dataset used for this analysis is anime_dataset.csv, which contains the following columns:

Name
English Name
Image source
Synopsis
Rating
Rated by (number of users)
Rank
Popularity
Release time
Number of episodes
Duration
Status
Aired
Producers
Studio(s)
Genres
Theme
Demographic
Anime recommendations (by users and automated recommendations)
Libraries Used
The following Python libraries are used in this project:

numpy
pandas
seaborn
matplotlib
Analysis Steps
Import Libraries:

Python
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
Load Dataset:

Python
df = pd.read_csv("anime_dataset.csv")
Initial Data Exploration:

Display the first few rows of the dataset:
Python
df.head()
Check the shape of the dataset:
Python
df.shape
Check the data types of the columns:
Python
df.dtypes
Data Cleaning:

Drop unnecessary columns:
Python
df = df.drop(['English Name', 'Image source', 'Synopsis','Anime
recommendations (by users and autorec)'], axis=1)
Handle missing values by dropping rows with any null values:
Python
df = df.dropna()
Analysis:

Filter animes with a rating of more than 7.5:
Python
df2 = df[df["Rating"] >= 7.5]
Visualization:

Various visualizations can be created using seaborn and matplotlib to gain insights from the data.
Results
The results of the analysis include insights into the ratings, popularity, and other attributes of the anime records. Key findings can be visualized through plots and charts.
