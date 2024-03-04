# Canadian Information Security Datathon Goal
In this Datathon, were tasked with the open-ended goal of searching for signs of Foreign Interference in Canada via social media and then distilling our findings into understandable insights via a presentation directed towards government officials, ensuring they are equipped with a clear understanding to make informed decisions on this critical issue.

We were provided with a dataset of State Affiliated Social Media accounts, which served as our starting point. After some exploratory data analysis, I found that Twitter was the most popular platform and we decided to focus our analysis on it. 

## Important

This repo contains datasets, code files and presentation for the 72hr Canadian Network & Information Security (CANIS) Hackathon. 

Check out our Jupyter Notebook: [https://colab.research.google.com/drive/1emBGbJVeE6vVSzEzPkSXX5NvRF9azT6W?usp=sharing](https://colab.research.google.com/drive/1emBGbJVeE6vVSzEzPkSXX5NvRF9azT6W?usp=sharing)

Check out our Presentation: https://prezi.com/view/Y6Qm9wQupHFbJIEw8BA7/

Collaborators: Khushil Nagda, Adel Müürsepp, Jeffrey Zhou

### Step 1: Scrapping the data

We scrapped 6000 tweets from the Twitter accounts in the dataset 

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/c66c1dbf-c6e2-43a3-9e53-37f31594dd51)

We took the direction of analyzing and comparing China's covert foreign influence and interference operations in 2 different contexts: what these operations look like when their targets are Western countries, and what these operations look like when their targets are non-Western countries. 
In order to gather more data about Chinese social media accounts, we scrapped information from each individual social media account, extracting information such as the engagement of each post and its Likes count

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/da650d53-f382-4e36-afd8-d99ceb4cc659)

## Step 2: Sentiment Analysis and Visualisation
We built our visuals using 2 main datasets: the one we were given and one containing tweets that we scraped. We cleaned these datasets using **Pandas**, and then NLTK's Vader library to analyze the Sentiment of the Tweets and assign them the relevant metrics. Thereafter, we used both **Matplotlib** and **Tableau** to visualize our findings and derive insights from them.

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/5e101658-9f2e-4072-bdb1-2fe2fa8276e5)

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/de4a3167-2937-4fd2-951c-e5d4c00ff893)

![image](https://github.com/khushil-sketch/Canadian-Inforomation-Security-Datathon/assets/52947378/48648fb3-f5dc-45dc-95f0-84c31ea72309)

## Do Polarising tweets get Seen More?
A notable observation is that even though there are fewer tweets that have a negative sentiment score, a large number of them get a high number of views.
This shows that the accounts are quite successful at dividing opinion i.e. influencing the masses 

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/f503847f-2acc-4b58-8359-8c4a6195c167)

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/fd30d2d6-8f1a-424d-9afd-927b3b410d62)


## Comparing Followers and Likes
Another way to catch accounts masquerading as authentic is by analysing their likes and followers. From the scatter plots below, there are a couple of anomalies that have suspicious likes vs follower ratios.

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/dca6905c-00c9-420f-8153-8df4c0c68a38)

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/e3cb813a-a4de-4da6-a313-4fbff0d261de)

![image](https://github.com/khushil-sketch/Canadian-Information-Security-Datathon/assets/52947378/03cb10d2-3a3b-4f84-8636-9cfe23859b94)

### Our Presentation

Lastly, we presented the results of our analysis in a manner that was both clear and concise, ensuring comprehensibility for a diverse audience. This included making our work accessible even to those who don't have domain expertise in statistics.

