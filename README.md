# Exploratory Analysis of UK Food Hygiene Ratings

The UK Food Standards Agency evaluates establishments across the United Kingdom and assigns them food hygiene ratings. This analysis aims to explore the ratings data to assist the editors of a food magazine, Eat Safe, Love, in identifying locations for future articles. The analysis involves setting up a MongoDB database, updating the database with new information, and conducting exploratory analysis to answer specific questions provided by the magazine editors.

## Database and Jupyter Notebook Set Up

Imported the provided data from the establishments.json file into MongoDB, naming the database uk_food and the collection establishments.
Verified the database and collection creation.
Imported necessary libraries such as PyMongo and Pretty Print (pprint).
Created an instance of the Mongo Client.
Confirmed database and collection existence and displayed a sample document using find_one and pprint.
Assigned the establishments collection to a variable for further use.

## Update the Database

Added a new halal restaurant, Penang Flavours, to the database with a NewRatingPending status.
Retrieved the BusinessTypeID for "Restaurant/Cafe/Canteen" and updated the new restaurant with the obtained BusinessTypeID.
Checked the number of documents containing the Dover Local Authority, removed establishments within the Dover Local Authority, and verified deletion.
Converted number values stored as strings to decimal numbers for latitude and longitude and integer numbers for RatingValue using update_many.

## Exploratory Analysis

Explored the dataset to answer specific questions provided by Eat Safe, Love magazine.
Conducted various queries using count_documents, pprint, and aggregation methods to find establishments meeting certain criteria.
Converted query results to Pandas DataFrames for further analysis and visualization.

## Questions Explored:

Which establishments have a hygiene score equal to 20?
Which establishments in London have a RatingValue greater than or equal to 4?
What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant, "Penang Flavours"?
How many establishments in each Local Authority area have a hygiene score of 0? Sorted the results from highest to lowest and printed out the top ten Local Authority areas.

## Conclusion:
This exploratory analysis provides valuable insights into the UK food hygiene ratings dataset. By addressing specific questions from Eat Safe, Love magazine, potential locations for future articles can be identified, helping food critics and journalists make informed decisions. The MongoDB database setup, data updates, and exploratory analysis steps are documented in the Jupyter Notebooks provided for reference.

### References
Past class activities, study groups with fellow cohorts, online resources, tutoring.
