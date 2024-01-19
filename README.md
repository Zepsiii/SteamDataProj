Motivation
•	My main motivation was the dollarization of the steam. I have been using steam very actively since 2020 but recently steam changed it’s pricing policy for Turkey and prices multiplied. Which means that I wont be able to use it actively from now on. So I thought It would be like a recap of my active steam usage, also maybe a bit like a memorial.

Data Source
•	Even though my data is not huge, it took various methods to collect it. I used steam API’s and also I had to scrape a website called SteamDB to gather my data. Then I merged them into a csv file.

Data Analysis
•	I started my analysis by visualizing the data I had. I calculated the correlations between my features.
•	I created two new features as “Cost per hour” and “Worthness”. They are closely related but not exactly the same. They both give an insight about if a game I purchased was worth it.

Machine Learning
•	I also used supervised learning by splitting my data into two as played and unplayed games. I used played games as train data and unplayed games as the test data. Than I visualized my top 20 unplayed games sorted by their predicted playtime.
•	I also visualized my top 20 unplayed games sorted by their predicted worthness according to my predicted playtime data.
•	Lastly I used unsupervised learning method to form clusters of playtime vs price, playtime vs release date and price vs release date.

Findings
•	I found out that I tend to prefer cheaper and relatively older games.
•	That I mostly remunerate the money I spent.
•	My data might not be enough enough for a precisely accurate prediction but my code says I would really enjoy Steins Gate series since it is my top 4 for predicted playtime.
•	But when it comes to worthness they lose the spotlight though I see that I might have to improve my worthness calculation or always set a numerically low threshold since I would consider all 20 of these games definitely worth the time and money.
•	Since my data is very limited it is hard to come to a proper conclusion but graphs show that my games tend to heap together in playtime vs price graph which shows that cheaper games are tend to have shorter playtimes.

What Coulld Be Done Better
•	I am aware of the inadequacies of my data which prevents me from further improving this project but I will try to further improve it and add new features to it. Some additions could be
o	Adding genres to game data to see where my data clusters.
o	Training the played games data set with respect to genres and using unpurchased game data as test data to be able to get decent suggestions from the program.
o	Getting some game data as input and use the trained data to decide if the given games is according to my likings.
o	Improving the project so that people can simply put in their steam id and give permissions for profile viewing to get proper game suggestions.
o	Creating an artificial neural network and training it with the steam data of every person to use the program and get it to categorize the players to get a better understanding of what kind of player prefers which games.
