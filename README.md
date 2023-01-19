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
1. Boolean value representing whether the book is in the most popular 50 books
2. The maximum Jaccard simialrity between the list of users 
who read the given book and the list of users who read each book that the given user have read
3. Number of books that users have read
4. Number of users who read the given book
- After conveting each data to a feature vector, we used 50% of our data to train logistc regressor, 
25% to validate them, and 25% to test them.

## Category Prediction
- Tried 2 different ways to predict(creating own featuer vectors and tfidf), and decided to use tfidf
- Use first 50% of dataset to train my model
- Convert each review_text to tfidf vector after removing stopword to prevent confusion
