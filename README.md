# The Goal
In this Datathon, were tasked with the open-ended goal of searching for signs of Foreign Interference in Canada via social media and then distilling our findings into understandable insights via a presentation directed towards government officials, ensuring they are equipped with a clear understanding to make informed decisions on this critical issue.

We were provided with a dataset of State Affiliated Social Media accounts, which served as our starting point. After some exploratory data analysis, I found that Twitter was the most popular platform and we decided to focus our analysis on it. 

## Important

This repo contains datasets, code files and the data-driven presentation for the 72-hour Canadian Network & Information Security (CANIS) Datathon. 

Check out our Jupyter Notebook, which contains most of the analysis and visualizations that I did: [https://colab.research.google.com/drive/1emBGbJVeE6vVSzEzPkSXX5NvRF9azT6W?usp=sharing](https://colab.research.google.com/drive/1emBGbJVeE6vVSzEzPkSXX5NvRF9azT6W?usp=sharing)

Check out our Presentation: https://prezi.com/view/Y6Qm9wQupHFbJIEw8BA7/

Collaborators: Khushil Nagda, Adel Müürsepp, Jeffrey Zhou

### Step 1: Scrapping the data

We scrapped 6000 tweets from the Twitter accounts in the dataset because I found that Twitter was the most popular social media platform in the dataset that we were provided.

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/8ac41054-1811-4fb3-9d1b-257410c44ae5)

A glimpse of the 6000 tweet dataset that we scrapped - we extracted crucial information such as the engagement of each post and its Likes count.

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/c66c1dbf-c6e2-43a3-9e53-37f31594dd51)


## Step 2: Sentiment Analysis 

With this huge dataset, there were multiple angles from which we could approach our foreign interference investigation. However, one crucial component was missing, a component that would help us identify specific accounts that were attempting to influence opinions: A Sentiment Analysis of Tweets.

Leveraging NLTK's Vader library, we analyzed the Sentiment and Subjectivity of the Tweets, assigning relevant metrics to quantify the negativity/positivity of tweets.

Now that the data collection was done, my work began. Using Pandas, Matplotlib and Plotly, I cleaned & transformed the datasets, investigated anomalies, performed exploratory visualizations and uncovered hidden insights that i brought to light in the final visualizations that I crafted.

## Who owns the accounts? What regions do they target?

![Network Flow Diagrams](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/ed7d6378-4dd5-4106-9e32-b6f79e55fc1a)

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/4023b9a3-289b-4738-b44f-9c15fd4aafd8)

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/5e101658-9f2e-4072-bdb1-2fe2fa8276e5)

## What regions have the most positive and negative Tweet sentiment?

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/de4a3167-2937-4fd2-951c-e5d4c00ff893)

## What is the distribution of Sentiment Scores for the 6000 tweets?

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/fd30d2d6-8f1a-424d-9afd-927b3b410d62)

## Do Polarising tweets get Seen More?
A notable observation is that even though there are fewer tweets that have a negative sentiment score, a large number of them get a high number of views.
This shows that the accounts are quite successful at dividing opinion i.e. influencing the masses 

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/f503847f-2acc-4b58-8359-8c4a6195c167)

## Comparing Followers and Likes
Another way to catch accounts masquerading as authentic is by analysing their likes and followers. Suspicious accounts have high followers and low likes.

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/dca6905c-00c9-420f-8153-8df4c0c68a38)

Out of all the Twitter accounts represented above, 29 were anomalous, but are all of them worth investigating?
![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/e5f7ebf5-5793-48bb-8237-e1b6bfc399e9)

Out of all the 29 anomalies, there's only 4 that are significant enough to investigate.
What makes them significant is that the average number of Like Counts for these 4 anomalies were calculated based on a large sample of tweets unlike the other potential anomalies which had a low tweet count.

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/713b07c7-1cea-4caf-b82a-42c143f8594d)

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/a342060f-ee19-44a4-bb18-7dcdb9acf959)


![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/e3cb813a-a4de-4da6-a313-4fbff0d261de)

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/03cb10d2-3a3b-4f84-8636-9cfe23859b94)



### Our Presentation

Lastly, we presented the results of our analysis in a manner that was both clear and concise, ensuring comprehensibility for a diverse audience. This included making our work accessible even to those who don't have domain expertise in statistics.

