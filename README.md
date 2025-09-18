# 🎬 Movie Recommendation System Using the Netflix Prize Dataset

This project builds a simple movie recommendation system using the **Collaborative Filtering** technique on the famous **Netflix Prize** dataset. The implemented model is **Singular Value Decomposition (SVD)**, which is used to predict the ratings a user might give to movies they haven't yet watched.



---

## 📊 Dataset

The dataset is a sample from the renowned **Netflix Prize** dataset, which contains millions of movie ratings from thousands of users. The structure consists of:
* **Cust_Id**: A unique ID for each customer.
* **Rating**: The rating given by the customer (on a scale of 1 to 5).
* **Movie_Id**: A unique ID for each movie.

This notebook loads and processes sample data from the `combined_data_1.txt` and `movie_titles.csv` files.

---

## ⚙️ Project Workflow

1.  **Data Loading and Processing**:
    * Raw rating data from the text file is loaded and transformed into a structured DataFrame.
    * The movie titles file is loaded to map `Movie_Id` to its corresponding title.
    * Initial analysis is performed to understand the distribution of ratings and the number of ratings per movie/user.

2.  **User-Item Utility Matrix Creation**:
    * The DataFrame is converted into a sparse utility matrix where rows represent users, columns represent movies, and the values are the ratings.
    * Due to the massive size of the dataset, only a sample is used for model training.

3.  **Modeling with SVD**:
    * **Singular Value Decomposition (SVD)** from the `surprise` library is used to perform matrix factorization on the rating data.
    * SVD breaks down the utility matrix into latent components that represent user preferences and movie characteristics.
    * The model is trained on a designated trainset.

4.  **Prediction and Recommendation**:
    * A function is created to provide movie recommendations for a specific user (`Cust_Id`).
    * This function predicts ratings for all movies the user has not yet watched.
    * The predictions are sorted to display the top 10 recommended movies.

---

## 📈 Results

The trained SVD model is capable of generating a personalized list of movie recommendations for any user in the dataset. The example output shows the top 10 recommended films that user `785314` is most likely to enjoy.
