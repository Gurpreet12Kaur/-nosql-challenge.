# -nosql-challenge.

Background

I have been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help our journalists and food critics decide where to focus future articles.


**Part 1: Database and Jupyter Notebook Setup**

1. Import the provided data from the "establishments.json" file into MongoDB. Name the database "uk_food" and the collection "establishments." Note the import command in a Markdown cell.

2. In your Jupyter Notebook, import the necessary libraries: PyMongo and Pretty Print (pprint).

3. Create a Mongo Client instance.

4. Confirm the database and data loading:
   - List the available databases in MongoDB and verify that "uk_food" is present.
   - List the collections in the database to ensure "establishments" exists.
   - Use `find_one` to retrieve and display one document from the "establishments" collection using `pprint`.
   - Assign the "establishments" collection to a variable for future use.
  
  **Part 2: Database Modifications**

In NoSQL_setup_starter.ipynb, follow these steps to update the "establishments" collection:

1. Add information for a new halal restaurant in Greenwich to the database.

2. Find and update the BusinessTypeID for "Restaurant/Cafe/Canteen."

3. Remove all establishments in the Dover Local Authority.

4. Convert latitude and longitude to decimals and RatingValue to integers using `update_many`.

Execute these updates as per the magazine's instructions.



**Part 3: Exploratory Analysis**

In NoSQL_analysis_starter.ipynb, perform the following tasks:

1. Explore the database and find answers to the following questions:
   - Which establishments have a hygiene score equal to 20?
   - Which establishments in London have a RatingValue greater than or equal to 4?
   - What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant "Penang Flavours"?
   - How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

2. For each question, use `count_documents` to display the number of documents contained in the result, display the first document using `pprint`, convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.

Execute these tasks to explore the database and find answers to the magazine's questions.

