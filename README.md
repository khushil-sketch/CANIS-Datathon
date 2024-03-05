# The Goal
In this Datathon, were tasked with the open-ended goal of searching for signs of covert Foreign Interference in Canada orchestrated via state-sponsored social media accounts and then distilling our findings into understandable insights via a presentation directed towards government officials, ensuring they are equipped with a clear understanding to make informed decisions on this critical issue.

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

## Comparing Followers and Likes
Another way to catch accounts masquerading as authentic is by analysing their likes and followers. Suspicious accounts have high followers and low likes.

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/dca6905c-00c9-420f-8153-8df4c0c68a38)

Out of all the Twitter accounts represented above, 29 were anomalous, but are all of them worth investigating?
![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/e5f7ebf5-5793-48bb-8237-e1b6bfc399e9)

Out of all the 29 anomalies, there's only 4 that are significant enough to investigate.
What makes them significant is that the average number of Like Counts for these 4 anomalies were calculated based on a large sample of tweets unlike the other potential anomalies which had a low tweet count.

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/713b07c7-1cea-4caf-b82a-42c143f8594d)

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/a342060f-ee19-44a4-bb18-7dcdb9acf959)

Out of the 4 anomalies, 2 are run by individual people. Let's look at metadata of Serena Dong's account

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/ce9a3824-4fe8-4d80-a092-c0b91d6fd14a)
![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/4dd0b682-f39d-4b14-8b1e-f89ad9bdac2c)

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/e28288d8-2203-4e76-93f8-320ba314d7a9)

For an account such as Serena's, where she has 47800 followers, the distribution of her Tweet Views, Likes and Retweets seems pretty normal and within the realm of possibility. 
However 3 things need to be done:
1. A benchmark has to be created of what constitutes a normal distribution of Tweet Views, Likes and Retweets for accounts with a similar level of following
2. Further analysis needs to be done of the anomalies (popular posts) in Serena's account
3. Perhaps investigating Twitter Views Shall reveal more information

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/e83237f3-907f-4d18-883d-984c53f01ac5)

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/31ebfd1d-53a6-48db-8954-06416c535472) ![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/b2714a62-f500-45df-b19c-3cf523e072f7)

There are lot of anomalous accounts revealed by the scatterplots. This begs the question - why do some accounts have disproportionately higher Tweet views than followers? The Sentiment Analysis can provide some clues

## What regions have the most positive and negative Tweet sentiment?

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/de4a3167-2937-4fd2-951c-e5d4c00ff893)

## What is the distribution of Sentiment Scores for the 6000 tweets?

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/fd30d2d6-8f1a-424d-9afd-927b3b410d62)

## Do Polarising tweets get Seen More?
A notable observation is that even though there are fewer tweets that have a negative sentiment score, a large number of them get a high number of views.
This shows that the accounts are quite successful at dividing opinion i.e. influencing the masses 

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/f503847f-2acc-4b58-8359-8c4a6195c167)

## Investigating the anomalies: Highly Viewed Tweets that have extreme sentiment scores

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/774cbfdc-71f5-461a-a5b2-248c755636cf)


### Our Presentation

Lastly, we presented the results of our analysis in a manner that was both clear and concise, ensuring comprehensibility for a diverse audience. This included making our work accessible even to those who don't have domain expertise in statistics.

