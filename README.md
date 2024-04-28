# nosql-challenge
 

- Setup process:
The code sets up a MongoDB database named uk_food and imports data from the establishments.json file into a collection named establishments.
- The initial process involves importing the collection establishments.json file into the MongoDB database named uk_food.
- The code retrieves and prints the first document from the establishments collection to review its structure and content.
- A new restaurant named "Penang Flavours" is added to the database using the insert_one() method.
- The code checks how many documents contain the Dover Local Authority, removes any establishments within the Dover Local Authority from the database using the delete_many() method, and then confirms that they were deleted.
- The latitude, longitude, and RatingValue fields are converted from strings to decimal numbers and integer numbers, respectively, using the update_many() method.
- The code prints out the first document in the collection after the updates to confirm that the coordinates and rating value are now numbers and correct datatypes.


Analysis: 
The code performs several exploratory analysis tasks using MongoDB aggregation queries:
Question 1: Finds establishments with a hygiene score equal to 20; Question 2: Finds establishments in London with a RatingValue greater than or equal to 4; Question 3: Finds the top 5 establishments with a RatingValue of 5, sorted by the lowest hygiene score, and nearest to a new restaurant named "Penang Flavours"; Question 4: Counts the number of establishments in each Local Authority area that have a hygiene score of 0.

The code leverages MongoDB's powerful aggregation framework to perform complex data analysis tasks directly within the database.By using MongoDB's native aggregation capabilities, it minimizes data transfer between the database and the Python application, resulting in efficient processing.