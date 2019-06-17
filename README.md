# Cryptocurrency_Analysis

## Goal
The goal of this project was to see if using 540 days worth of data for 9 seperate cryptocurrencies if we can predict whether or not within a day will provide us with an increase or decrease in price from the previous day. I ran three seperate analysis methods on our data which were Market Basket Analysis, Support Vector Machines, and Decision Trees.

## Getting Started
In order to utilize Market Basket Analysis, we need to manipulate the data to fit a transaction cart. The SYEFinalProjectDataPrime file goes through each data set and adds a new variable called "inBasket". If the price of the day we are looking at ended up higher than the previous day than it is coded as a 1, otherwise it is a 0. After this was done, a whole new data set was created with all 9 inBasket variables which is our transaction cart dataset. Once that had been done, I went through the transcation cart dataset and replaced the 1s with the name of the actual coin (so that we know which coin is in the cart for the day), otherwise, it was left blank.

