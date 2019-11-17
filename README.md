# Beauty-Products-Recommender
## Objective
The recommending system is needed in order to help the customers to find a product the she/he may want to buy and to suggest them some additional products. 
The aim is to recommend similar products based on the user's current selection.
## The Data
The Dataset includes rating of 249,274 products os a scale of 1-5, rated by 1,210,271 users.
The Columns were:
UserId, ProductID, Rating and timestamp.
The csv file data was transformed into a pandas dataframe.
## The Solution:
### 1.Identify groups of users that purchased the same product and gave the same rating to the product.
### 2.Identify products the recommended user did not purchase  and the other users in the group did purchase.
### 3.Calculate per these products the overall Rating 
### 4. Chose the K(=5) highest Rated products and recommend them to the user.
*if there is no recommender user we return the overall top 5 rated products.
## Algorithms
### 1.Bayesian Average Rating: 
       If m is the mean of the ratings and n is the number of the ratings: rating(m'n) = mn/(n+K)
### 2.Arithmetical Average: regular average
### 3.Unreliability : used for reducing noises and integrating the amount of ratings
