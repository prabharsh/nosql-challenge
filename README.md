 nosql-challenge
Module 12 challenge

## Background
The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. The scenario presented is that i have  been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

## Part 1: Database and Jupyter Notebook Set Up
1.	Import the data provided in the establishments.json file from your Terminal. Name the database uk_food and the collection establishments. 
2.	Within the notebook, import the libraries: PyMongo and Pretty Print (pprint).
3.	Create an instance of the Mongo Client.
4.	Confirm that you created the database and loaded the data properly:
a. List the databases you have in MongoDB. Confirm that uk_food is listed.
b. List the collection(s) in the database to ensure that establishments is there.
c. Find and display one document in the establishments collection using find_one and display with pprint.
5.	Assign the establishments collection to a variable to prepare the collection for use.

## Part 2: Update the Database
The magazine editors have some requested modifications for the database before you can perform any queries or analysis for them. Make the following changes to the establishments collection:
1.	An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis. Add the following information to the database:
2.	Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
3.	Update the new restaurant with the BusinessTypeID you found.
4.	The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.
5.	Some of the number values are stored as strings, when they should be stored as numbers. Use update_many to convert latitude and longitude to decimal numbers.

## Part 3: Exploratory Analysis
Eat Safe, Love has specific questions they want you to answer, which will help them find the locations they wish to visit and avoid.

Use the following questions to explore the database, and find the answers, so you can provide them to the magazine editors.
Unless otherwise stated, for each question:
1. Use count_documents to display the number of documents contained in the result.
2.	Display the first document in the results using pprint.
3. Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.
4.	Which establishments have a hygiene score equal to 20?
5.	Which establishments in London have a RatingValue greater than or equal to 4?

