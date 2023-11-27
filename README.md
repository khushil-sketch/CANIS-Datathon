# CANIS-Data-Visualization-Foreign-Interference-Hackathon

Check out our Jupyter Notebook: https://colab.research.google.com/drive/1emBGbJVeE6vVSzEzPkSXX5NvRF9azT6W?usp=sharing

Check out our Presentation: https://prezi.com/view/Y6Qm9wQupHFbJIEw8BA7/

### Hackathon Goal

This Hackathon was focused on analyzing & visualizing the scale of China's influence on social media as well as investigating whether there have been attempts at foreign influence through these accounts.

### Scrapping the data

In order to do this, we were given a raw, uncleaned dataset containing metadata on Chinese owned/affiliated social media accounts as a starting point

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/c66c1dbf-c6e2-43a3-9e53-37f31594dd51)

We took the direction of analyzing and comparing China's covert foreign influence and interference operations in 2 different contexts: what these operations look like when their targets are Western countries, and what these operations look like when their targets are non-Western countries. 
In order to gather more data about Chinese social media accounts, we scrapped information from each individual social media account, extracting information such as the engagement of each post and its Likes count

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/da650d53-f382-4e36-afd8-d99ceb4cc659)

## Sentiment Analysis and Visualisation
We built our visuals using 2 main datasets: the one we were given and one containing tweets that we scraped. We cleaned these datasets using **Pandas**, and then NLTK's Vader library to analyze the Sentiment of the Tweets and assign them the relevant metrics. Thereafter, we used both **Matplotlib** and **Tableau** to visualize our findings and derive insights from them.

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/5e101658-9f2e-4072-bdb1-2fe2fa8276e5)

![image](https://github.com/khushil-sketch/CANIS-Data-Visualization-Foreign-Interference-Hackathon/assets/52947378/66a3bc04-36cf-4d34-8524-1bdbe44a4572)

### Challenges and our Presentation

The biggest challenge we ran into was difficulty scraping tweets from Twitter, as we were unfortunately only able to scrape tweets from about 150 of the 573 accounts that we wanted to access. Although this still amounted to about 6500 tweets that we were able to derive analyses from, a future improvement would be to gain access to a wider range of tweets from a wider range of accounts.

Lastly, we wove together a story, presenting the results of our analysis in a manner that was both clear and concise, ensuring comprehensibility for a diverse audience. This included making our work accessible even to those who are not proficient in statistics.

