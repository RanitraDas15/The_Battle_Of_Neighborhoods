# The_Battle_Of_Neighborhoods
To identify clusters of venues (cafes and restaurants) in Pune, India based on their rating and average prices

## Introduction
The aim of the project is to identify venues in Pune, India based on their rating and average prices. In this notebook, we will identify various venues in the city of Pune, India, using Foursquare API and Zomato API, to help visitors select the restaurants that suit them the best.

Whenever a user is visiting a city they start looking for places to visit during their stay. They primarily look for places based on the venue ratings across all venues and the average prices such that the locations fits in their budget.

Here, we'll identify places that are fit for various individuals based on the information collected from the two APIs and Data Science. Once we have the plot with the venues, any company can launch an application using the same data and suggest users such information.

## Data Collection from APIs 
To begin with, we will take a look at Pune on the Map using the **folium** library.

We will also fetch the data from two different APIs.

- ***Foursquare API:*** We will use the Foursquare API to fetch venues in Pune starting from the middle upto 44 Kilometers in each direction.
- ***Zomato API:*** The Zomato API provides information about various venues including the complete address, user ratings, price for two people, price range and a lot more.

## Pune
Pune, also known as Poona is a bustling metropolis in the Indian State of Maharashtra and the 8th most populous city in India with an estimated population of 7.2 million as of 2019. It is composed of a number of sectors spread across a total area of 150 sq Km. There are many venues (especially restaurants, hotels and cafes) which can be explored.

## Results and Discussion 
Based on our analysis above, we can draw a number of conclusions that will be useful to aid any visitor visiting the city of Pune, India.

After collecting data from the **Foursquare** and **Zomato APIs**, we got a list of 120 different venues. However, not all venues from the two APIs were identical. Hence, we had to inspect their latitude and longitude values as well as names to combine them and remove all the outliers. This resulted in a total venue count of 49.

We identified that from the total set of venues, majority of them were **Cafes** and **Indian Restaurants**. A visitor who loves Cafes/Indian Restaurants would love to travel to Pune.

While the complete range of ratings range from 1 to 5, the **majority venues have ratings close to 4**. This means that most restaurants provide **good quality food** which is liked by the people of the city, thus indicating the high rating. When we plot these venues on the map, we discover that there are clusters of venues around **Hinjewadi, Balewadi High Street and Baner.** These clusters also have very **high ratings (more than 3)**.

When we take a look at the price values of each venue, we explore that **many venues** have prices which are in the **range of Rs 400 to Rs 700 for one person**. However, the variation in prices is very large, given the complete range starts from Rs 100 and goes uptil Rs 1200. On plotting the venues based on their price range on the map, we discovered that venues located near **Hinjewadi and Baner are relatively priced lower than venues in Balewadi High Street**.

Finally, through clusters we identified that there are **many venues** which are **relatively lower priced but have an average rating of 3.55**. On the other hand, there are **few venues** which are **high priced and have average rating of 4.05**.

If you're looking for cheap places with relatively high rating, you should check **Hinjewadi**.
If you're looking for the best places, with the highest rating but might also carry a high price tag, you should visit **Baner and Balewadi High Street**.
A company can use this information to build up an online website/mobile application, to provide users with up to date information about various venues in the city based on the search criteria (name, rating and price).

## Conclusion 
The purpose of this project was to explore the places that a person visiting Pune West could visit. The venues have been identified using Foursquare and Zomato API and have been plotted on the map. The map reveals that there are three major areas a person can visit: Hinjewadi, Baner & Balewadi High Street. Based on the visitor's venue rating and price requirements, he/she can choose amongst the three places.
