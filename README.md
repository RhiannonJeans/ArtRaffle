Python Art Raffle Scripts

These scripts are designed to programmatically generate the winner of an art raffle. I ran art raffles on Twitter by making a single post which people are instructed to follow + like + retweet in order to enter. These scripts will programmatically extract your followers, the likes and retweets on the post, and then find the intersection between them. It will then randomize the list to pick the winner.

These scripts were originally set up in Anaconda Navigator and run in Jupiter Notebooks. It uses Python 3.8.5 and I have included a list of packages in my environment in the environment.yml file. You can build the environment with the following code:

conda env create -f environment.yml

Motivations
I decided to use Python owing to the availability of the Tweeepy API. At the time I made these scripts I was also teaching myself Python.

How to Install
I installed this by installing Anaconda, then creating a custom library. I used the Anaconda Navigator to organise my Jupiter Notebook files.

How to Use
To use these scripts you will need a Twitter account, a post that you want to run the code on.

Credits
Credits are included within the file themselves but I will compile them here as well:

License
https://creativecommons.org/licenses/by-nc/4.0/