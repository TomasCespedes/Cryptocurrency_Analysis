# Cryptocurrency_Analysis

## Goal
The goal of this project was to see if using 540 days worth of data for 9 seperate cryptocurrencies if we can predict whether or not within a day will provide us with an increase or decrease in price from the previous day. I ran three seperate analysis methods on our data which were Market Basket Analysis, Support Vector Machines, and Decision Trees.

## Getting Started
In order to utilize Market Basket Analysis and have a response as to whether or not the price will increase (0 or 1), we need to manipulate the data to fit a transaction cart dataset. The SYEFinalProjectDataPrime file goes through each data set and adds a new variable called "inBasket". If the price of the day we are looking at ended up higher than the previous day than it is coded as a 1, otherwise it is a 0. After this was done, a whole new data set was created with all 9 inBasket variables which is our transaction cart dataset. Once that had been done, I went through the transcation cart dataset and replaced the 1s with the name of the actual coin (so that we know which coin is in the cart for the day), otherwise, it was left blank. Once we have all the variables the way we want them, we then save the new dataset as a csv file to be analyzed. 

## Market Basket Analysis
The goal of market basket is to try and predict whether if certain items are in a "shopping cart", they will increase the probability of a specific item to also show up in the shopping cart. In my analysis, I wanted to see if an increase of price of some collection of coins would have a correlation to a specific coin increasing. For example, if Bitcoin, Neo, and Vertcoin go up, maybe we will see an increase in VeChain as well. Since there is no train/test option for Market basket, I ran the algorithm on the entire dataset, a random first half of the dataset, and the random second half of the dataset and compared results across all three outputs. 

