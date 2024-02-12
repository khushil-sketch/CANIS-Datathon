# Datathon Goal
In this Datathon, were tasked with the open-ended goal of searching for signs of Foreign Interference in Canada via social media and then distilling our findings into understandable insights via a presentation directed towards government officials, ensuring they are equipped with a clear understanding to make informed decisions on this critical issue.

We were provided with a dataset of State Affiliated Social Media accounts, which served as our starting point. After some exploratory data analysis, I found that Twitter was the most popular platform and we decided to focus our analysis on it. 

## CANIS-Data-Visualization-Datahon

This repo contains datasets, code files and presentation for the 72hr Canadian Network & Information Security (CANIS) Hackathon. 

Check out our Jupyter Notebook: https://colab.research.google.com/drive/1emBGbJVeE6vVSzEzPkSXX5NvRF9azT6W?usp=sharing

Check out our Presentation: https://prezi.com/view/Y6Qm9wQupHFbJIEw8BA7/

Collaborators: Khushil Nagda, Adel Müürsepp, Jeffrey Zhou

### Scrapping the data

We scrapped 6000 tweets from the Twitter accounts in the dataset 

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/c66c1dbf-c6e2-43a3-9e53-37f31594dd51)

We took the direction of analyzing and comparing China's covert foreign influence and interference operations in 2 different contexts: what these operations look like when their targets are Western countries, and what these operations look like when their targets are non-Western countries. 
In order to gather more data about Chinese social media accounts, we scrapped information from each individual social media account, extracting information such as the engagement of each post and its Likes count

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/da650d53-f382-4e36-afd8-d99ceb4cc659)

## Sentiment Analysis and Visualisation
We built our visuals using 2 main datasets: the one we were given and one containing tweets that we scraped. We cleaned these datasets using **Pandas**, and then NLTK's Vader library to analyze the Sentiment of the Tweets and assign them the relevant metrics. Thereafter, we used both **Matplotlib** and **Tableau** to visualize our findings and derive insights from them.

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/5e101658-9f2e-4072-bdb1-2fe2fa8276e5)

![image](https://github.com/khushil-sketch/Canadian-Inforomation-Security-Datathon/assets/52947378/48648fb3-f5dc-45dc-95f0-84c31ea72309)

![image](https://github.com/khushil-sketch/Canadian-Inforomation-Security-Datathon/assets/52947378/075d4b67-ff23-4f09-8333-a208625fe5e2)


![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/6a38957a-7036-4d16-b079-db7ec42481a7)

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/ba8da9b6-b5c7-463d-9844-b32432451556) 





### Our Presentation

Lastly, we presented the results of our analysis in a manner that was both clear and concise, ensuring comprehensibility for a diverse audience. This included making our work accessible even to those who don't have domain expertise in statistics.

