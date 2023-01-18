# Read and Category Prediction

## Two types of predictions are made
- If the user read the certain book
- The category(genre) of the book

## Dataset overview
- Each data from dataset is the review about the book that the user read
- Each data contains information about review text, rating, user id, book id, etc.

## Read Prediction
- Used Logistic regression to determine whether user had read or not
- Given input for the predction was user id and the book id
- Feature vector contains:
1. Boolean value 
