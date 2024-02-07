# NoSQL Challenge 
## Project Overview
This project involves setting up and analyzing a database of food establishments across the United Kingdom. The dataset, provided by the UK Food Standards Agency, contains ratings and information about various establishments. The objective is to perform data manipulation, updates, and exploratory analysis to assist a food magazine, Eat Safe, Love, in deciding where to focus future articles.

## Repository Contents
NoSQL_setup_starter.ipynb: Jupyter notebook for setting up the MongoDB database and performing initial data manipulation.
NoSQL_analysis_starter.ipynb: Jupyter notebook for exploratory analysis of the database.
establishments.json: JSON file containing data of food establishments.

## Part 1: Database and Jupyter Notebook Set Up
Steps:

Database Creation and Data Import:

Imported the establishments.json file into a MongoDB database named "uk_food" with a collection named "establishments".
Used the mongoimport command to import the data and dropped any existing establishments collection.
Library Imports and Client Creation:

Imported necessary libraries: PyMongo and Pretty Print (pprint).
Created an instance of the Mongo Client.
Confirmation and Data Retrieval:

Confirmed the creation of the database and loading of data.
Retrieved and displayed one document from the establishments collection using find_one and pprint.
Assigned the establishments collection to a variable.

## Part 2: Update the Database
Steps:

Database Modifications:

Added a new restaurant, "Penang Flavours", to the database with a NewRatingPending status.

Retrieved and updated the BusinessTypeID for "Restaurant/Cafe/Canteen" category.

Removed establishments within the Dover Local Authority.

Data Type Conversion:

Used update_many to convert latitude, longitude, and RatingValue fields to appropriate data types.

## Part 3: Exploratory Analysis

### Questions Explored:

Establishments with hygiene score equal to 20.

Establishments in London with a RatingValue greater than or equal to 4.

Top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to "Penang Flavours".

Number of establishments in each Local Authority area with a hygiene score of 0.

## References

UK Food Standards Agency. (2022). UK food hygiene rating data API. https://ratings.food.gov.uk/open-data/en-GB.
Contains public sector information licensed under the Open Government Licence v3.0.
Accessed on September 9, 2022, and September 12, 2022.
Establishment settings: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).

## Note:
This project is assigned by university Of Toronto in order to complete the certification of data analysis.



