Report

1. Which insights did you gain from your EDA? Were any columns highly correlated? If so, name them.
    
    The exploratory data analysis helped me to gain valuable insights that helped to guide my data cleaning, feature selection and modeling processes. Firstly, I observed that the column for song length showed a right skew, with most songs between 25-100. I also saw that most of the songs were either pop or country, and the hip hop genre had the least amount of songs represented in the dataset. From this, I had an idea that the model might not generate a seperate cluster for hip hop songs, and instead group them with other songs based on some other characteristic, since there is not enough of the in the dataset compared to the other genres. Another important observation was that around 6000 songs had a topic of sadness, and the clustering algorithm can possibly cluster songs based on their topic. I did not see any unusual or very high correlations between features, but I did observe that the correlation between len and obscene was around 0.44.


2.How did you determine which columns to drop or keep? If your EDA informed this process, explain which insights you used to determine which columns were not needed.
    
    In order to determine which columns to drop or keep, I relied mostly on my plan and outlook for the model.  Since I was not going to focus on the lyrics, I decided to drop the lyrics column first. I determined that the approach i wanted to follow was to focus on the columns that described song content rather than information like name, artist name and release date. Therefore, I decided to drop artist and track name, release date, age and len. i was left with the columns that described the songs content, genre, topic and how much it relfelcted certain topics on a scale of 0 to 1.


3.What was the optimal number of clusters in your cluster model? Explain how you determined this value.
    
    The optimal number of clusters that I found in my model was 8 clusters. I decided to use an Elbow plot and I was able to find that the optimal number of clusters is 8


4.Take a look at the respective songs that fell into your clusters. Describe these clusters in human terms to the best of your ability using the columns in your dataset (for example high-gospel songs, low-gospel songs, etc). Feel free to listen to these songs as well to get a sense of what nuance your algorithm picked up on.
    
    For the analysis, I decided to look at the first 5 clusters. With Cluster 0, We can see that a majority of the songs in this cluster are blues, with very low violence scores as well as a high feelings score. Within Cluster 1,there is a mix of genres, with 2 songs being country. The songs have higher obscenity score which may explain their grouping as well as the topic of the songs being obscene. In Cluster 2 there a mix of genres, with higher violence scores as well as a topic label of violence. Upon analyzing cluster 3, i found that This cluster has more pop songs. Most of the songs in this cluster also have a higher sadness score and fititngly the topic for all of them is also sadness. Finally, cluster 4 has a mix of genres, with all songs having a topic of romantic as well as the age of the songs being on the higher end


5. Take a look at the clusters that your algorithm assigned to your test samples. Based on these clusters, which songs would you recommend to this user?

    With the test samples, the clustering algorithm assigned the most to cluster 1. Cluster 1 has 3 out of 10 samples. Upon observing this cluster, I saw that 2 songs are pop while 1 is jazz, and they have medium level violenece scores. They also have a topic of violence. The next 2 largest clusters are 4 and 7 which have 2 samples each. Cluster 4 shows a medium to high sadness score and an accompanying topic of sadness, with an age at the higher end of the scale. Cluster 7 has a topic of night/time and a medium age, showing that this cluster is likely assigned on topic. Based on these clusters, I would probably recommend pop or jazz songs that have the topics of violence or sadness.





