## Heroes of Pymoli

You've been assigned the task of analyzing the data for the fantasy game, Heroes of Pymoli.

Like many others in its genre, the game is free-to-play, but players are encouraged to purchase optional items that enhance their playing experience. As a first task, the company would like you to generate a report that breaks down the game's purchasing data into meaningful insights.

Your final report should include each of the following:

#### Player Count

- Total Number of Players

#### Purchasing Analysis (Total)

- Number of Unique Items
- Average Purchase Price
- Total Number of Purchases
- Total Revenue

#### Gender Demographics

- Percentage and Count of Male Players
- Percentage and Count of Female Players
- Percentage and Count of Other / Non-Disclosed

#### Purchasing Analysis (Gender)

- The below each broken by gender
  - Purchase Count
  - Average Purchase Price
  - Total Purchase Value
  - Average Purchase Total per Person by Gender

#### Age Demographics

- The below each broken into bins of 4 years (i.e. <10, 10-14, 15-19, etc.)
  - Purchase Count
  - Average Purchase Price
  - Total Purchase Value
  - Average Purchase Total per Person by Age Group

#### Top Spenders

- Identify the the top 5 spenders in the game by total purchase value, then list (in a table):
  - SN
  - Purchase Count
  - Average Purchase Price
  - Total Purchase Value

#### Most Popular Items

- Identify the 5 most popular items by purchase count, then list (in a table):
  - Item ID
  - Item Name
  - Purchase Count
  - Item Price
  - Total Purchase Value

#### Most Profitable Items

- Identify the 5 most profitable items by total purchase value, then list (in a table):
  - Item ID
  - Item Name
  - Purchase Count
  - Item Price
  - Total Purchase Value
  
  
  ### Summary
  
  The purpose of this project was to create a straight-forward analysis of sale and user statistics for a game developer. These statistics would be useful in determining how best to market their game, as well promoting in-game purchases to players. 
  
  The player analysis was fairly simple, starting with a formula to determine the length of unique player IDs for the total number of players and a value count on the Gender field. 
  
  We can see from the gender breakdown that most players are male.
  
  
  For sale analysis, I started with a basic summary of the total count of purchases, total number of unique items sold, the total sales figure, and the average sales price. 
  
  I then combined the gender data with the sales analysis. This was accomplished by first grouping the inital data frame by gender, then applying the same statistical analysis used for the total sales (count, mean, and sum).
  
  
  From these results, it's clear that female players make much fewer purchases than male players, even in relation to the ratio of male to female players. A possible insight that could be gained from this information is that developers should be creating more DLC/content for purchase that appeals to female players. Alternatively, the marketing department could adjust how they advertise these in-game purchases to engage female players.
  
  
  This leads us into analyzing players and purchases by age. I started by binning the inital purchase data frame into age groups and getting a count per group. 
  
  
  This breakdown shows that players were distributed evenly over a bell curve, with the majority of players being aged 15 to 29. 
  
  From there, we applied the same sales analysis as used previously on the age groups. 
  
  
  While these results show that the purchase totals generally followed the player age distribution, there was a clear difference between the extreme ends of the age groups. Very young players (14 and under) purchased much more than the older players (35+). 
  
  The analysis then transistions to looking at individual players and items for purchase. I started by ranking the players by the total amount spent on the game. This was accomplished by grouping the player data frame by Screen Name, applying sales statistics, then sorting by purchase total.
  
  
  I then ranked the items that were most purchased. To make this simpler, I only extracted the relevant columns from the purchase data frame (Item ID, Item Name, and Price). Similar to the top spenders, I applied the sales statistics and sorted by item count. 
  
  
  For a slightly different metric, I took that same item data and sorted by total purchase. 
 

