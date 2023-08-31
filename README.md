# Unsupervised-Capstone-Project
![image](https://github.com/shaikh111-Z/Unsupervised-Capstone-Project/assets/83855661/a3f9da1e-36e4-4ba4-9ed5-139ab4d47852)







Netflix movies and TV Shows Clustering
Netflix is the world's largest online streaming service provider, with over 220 million subscribers as of 2022-Q2. It is crucial that they effectively cluster the shows that are hosted on their platform in order to enhance the user experience, thereby preventing subscriber churn.

# Table of Content
- Problem Statement
- Objective
- Dataset
- Data Pipeline
- Conclusion

# Problem Statement
In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset. We will be able to understand the shows that are similar to and different from one another by creating clusters, which may be leveraged to offer the consumers personalized show suggestions depending on their preferences.

# Objective
The goal of this project is to classify/group the Netflix shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

# Dataset
This dataset consists of tv shows and movies available on Netflix as of 2019. It includes over 7787 records and 12 attributes. Each attribute is provide information about movies/TV shows. More details of the dataset can be found in the kaggle website. https://www.kaggle.com/datasets/sambhajizambre/netflix-movies-and-tv-shows-clustering?select=netflix_titles.csv

# Data Pipeline
1. Analyze Data:
In this initial step we went to look for different features available and tried to understand the data . During this stage, we looked for the shape of data, data types of each feature, statistical summary etc.
2. EDA:
EDA or Exploratory Data Analysis is the critical process of performing the initial investigation on the data. So, through this we have observed certain trends and dependencies and drawn certain conclusions from the dataset that will be useful for further processing
3. Data Cleaning:
Checked duplicated values present in the dataset. After that comes the null value and outlier detection and treatment. For the null values imputation we simply replace with empty string and drop some of the null rows then analyze outlier and handling.
4. Textual Data Preprocessing:
During this stage, cluster the data based on the attributes: director, cast, country, genre, rating and description. Data preprocessing include Remove all stop words and punctuation marks, convert all textual data to lowercase. Stemming to generate a meaningful word out of corpus of words. Tokenization of corpus and Word vectorization. We used Principal Component Analysis (PCA) to handle the curse of dimensionality.
5. Clusters Implementation:
Use K Means and Agglomerative Hierarchical clustering algorithms to cluster the movies, obtain the optimal number of clusters using different techniques.

# Conclusion
In this project, we worked on a text clustering problem wherein we had to classify/group the Netflix shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

The dataset contained about 7787 records, and 12 attributes. We began by dealing with the dataset's missing values and doing exploratory data analysis (EDA)..

It was found that Netflix hosts more movies than TV shows on its platform, and the total number of shows added on Netflix is growing exponentially. Also, majority of the shows were produced in the United States.

Highest number of shows on Netflix are rated by TV-MA, followed by TV-14 and TV-PG

Around 50% of shows on Netflix are produced for adult audience. Followed by young adults, older kids and kids. Netflix has the least number of shows that are specifically produced for teenagers than other age groups.

The highest number of movies / TV shows were based out of the US, followed by India and UK.

The dramas is the most popular genre followed by comedies and documentaries.

As we can see from the above graph that most of the content was release in the year 2018 followed by 2017.

Most of the movies were released in the year 2017 and most number of TV Shows were released in the year 2020.

Majority of the content is about 70 to 120 min duration for movies.

Over the years, Netflix has consistently focused on adding more shows in its platform.

Though there was a decrease in the number of movies added in 2020, this pattern did not exist in the number of TV shows added in the same year.

This might signal that Netflix is increasingly concentrating on introducing more TV series to its platform rather than movies.

Netflix has several movies on its site, including those that were released in way back 1942.

As per the plot, movies made in the 1940s had a fairly short duration on average.

On average, movies made in the 1960s have the longest movie length.

The average length of a movie has been continuously decreasing since the 2000s

International, crime, and kids are the most popular genre for TV shows on Netflix.

United States stands at top with respect to most content produced country wise.

It was decided to cluster the data based on the attributes: director, cast, country, genre, rating and description. The values in these attributes were tokenized, preprocessed, and then vectorized using TFIDF vectorizer.

Through TFIDF Vectorization, we created a total of 10000 attributes. We used Principal Component Analysis (PCA) to handle the curse of dimensionality. 3000 components were able to capture more than 80% of variance, and hence, the number of components were restricted to 3000.

We first built clusters using the K-Means Clustering algorithm, and the optimal number of clusters came out to be 9. This was obtained through the elbow method and Silhouette score analysis.

Finally we observed the formation of clusters and vizualized the data in each clusters.

