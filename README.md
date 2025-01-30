# nosql-challenge

# nosql-challenge
# UK Food Hygiene Data Analysis
## Part 1: Database & Jupyter Notebook Setup

### Import Data: 
1. Load establishments.json into MongoDB using Terminal.
2. Setup MongoDB Connection:
3. Import PyMongo and pprint.
4. Connect to MongoDB and verify the uk_food database and establishments collection exist.

### Initial Data Check:
Display one document using find_one().
Assign establishments to a variable for future use.

## Part 2: Database Updates
1. Add a New Restaurant:
    Insert "Penang Flavours" in Greenwich with a NewRatingPending = True.
2. Update BusinessTypeID:
    Find the BusinessTypeID for "Restaurant/Cafe/Canteen".
3. Update "Penang Flavours" with this ID.
4. Remove Dover Establishments:
      Count and delete all establishments in "Dover".
5. Convert Data Types:
      Update latitude & longitude to decimal numbers.
      Convert RatingValue to integers, replacing non-numeric values with null.
   
## Part 3: Exploratory Analysis
1. Find Establishments with a Hygiene Score of 20.
2. Find Establishments in London with a RatingValue ≥ 4 (using $regex for "London").
3. Find the Top 5 Establishments with a RatingValue of 5:
      Sort by lowest hygiene score.
      Filter by locations near "Penang Flavours" (±0.01 latitude/longitude).
4. Count Establishments with a Hygiene Score of 0:
      Group by LocalAuthorityName.
      Sort results highest to lowest.
      Display top 10 local authorities.
