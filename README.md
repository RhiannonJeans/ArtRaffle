# Python Art Raffle Script

These scripts are designed to programmatically generate the winner of a Twitter art raffle. I ran art raffles on Twitter by making a single post which people are instructed to follow + like + retweet in order to enter. These scripts will programmatically extract your followers, the likes and retweets on the post, and then find the intersection between them. It will then randomize the list to pick the winner.

## Motivations
I decided to use Python owing to the open source nature of the Tweepy API. At the time I made these scripts I was also teaching myself Python. I wanted to overcome the inaccuracy of manually selecting followers for a raffle, I wanted to programmatically find the intersections and randomise the raffle winner so the procedure was fair.

## How to Install
First install Anaconda, then create a custom library. I used the Anaconda Navigator to access my Jupiter Notebook files.

### Python Version and Environment.yml
These scripts were originally set up in Anaconda Navigator and run in Jupiter Notebooks. It uses Python 3.8.5 and I have included a list of packages in my environment in the environment.yml file. You can build the environment with the following code:

  conda env create -f environment.yml

## How to Use
To use these scripts you will need a Twitter account, and a post that you want to run the code on. Some of the instructions are specific to the Windows OS. You will need to run the codes which extract data using Tweepy first, then the intersection script last. You will need to add your own variables:
- consumer_key= ''
- consumer_secret= ''
- access_token= ''
- access_token_secret= ''

These are explained in the Tweepy tutorial links below.

## Order to Run The Files
It is recommended to run the files in this order:
- Get_Twitter_Followers.ipynb
- Get_Tweet_Retweeters.ipynb
- Get_Twitter_Likes.ipynb
- ArtRaffle_Intersections.ipynb

Get_Twitter_Likes is listed last of the first 3 as it involves using a web scraper called GeckoDriver which involves additional steps. This is because Twitter Likes are not available in the Tweepy API as they are hidden within the javascript of the website. Be careful when controlling GeckoDriver as this is the most error-prone step (more advice in the file itself).

## Credits
Additional credits are included within the file themselves.

[Earth Science Tweepy Tutorial](https://www.earthdatascience.org/courses/use-data-open-source-python/intro-to-apis/twitter-data-in-python/)

[Earth Science Twitter API for Beginners](https://towardsdatascience.com/tweepy-for-beginners-24baf21f2c25)

[Web Scraping with GeckoDriver](https://towardsdatascience.com/data-science-skills-web-scraping-javascript-using-python-97a29738353f)
