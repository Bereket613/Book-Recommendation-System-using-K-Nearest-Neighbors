

# Book Recommendation System using K-Nearest Neighbors

## Overview
This project implements a book recommendation system based on the Book-Crossings dataset. The system uses the K-Nearest Neighbors (KNN) algorithm to recommend books that are similar to a given book title. The data includes ratings of over 270,000 books by 90,000 users. The KNN model helps in finding the "closeness" of books based on user ratings.
<img width="938" height="482" alt="image" src="https://github.com/user-attachments/assets/2bf4804d-7fb1-44cc-a56c-3b758ad52585" />

## Project Steps:
1. **Data Preprocessing**:
   - Import and clean the Book-Crossings dataset.
   - Filter out books with fewer than 100 ratings and users with fewer than 200 ratings.
   
2. **Creating a Book-User Rating Matrix**:
   - Pivot the dataset into a book-user matrix where each row represents a book and each column a user, with ratings as values.
   
3. **KNN Model**:
   - Use the `NearestNeighbors` algorithm from Scikit-learn to build the recommendation model.
   - The model computes cosine similarity between books based on their user ratings.
   
4. **Book Recommendations**:
   - Given a book title, the function `get_recommends` returns the top 5 similar books with their respective distances.

## Requirements:
- Python 3.x
- pandas
- numpy
- scikit-learn
- scipy

## How to Use:
1. Clone or download this repository.
2. Install the required libraries (if necessary):
   ```bash
   pip install -r requirements.txt
Run the Jupyter Notebook or Python script to see the results.

Example:
get_recommends("The Queen of the Damned (Vampire Chronicles (Paperback))")
License:
This project is based on a challenge from FreeCodeCamp.

---

You can copy this directly into your project’s GitHub repository. Let me know if you need any changes or additional details!

