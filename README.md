# 🎬 Netflix Prize Recommendation System

This project builds a **movie recommendation system** using the **Netflix Prize Dataset**.  
It applies data preprocessing, exploratory analysis, and collaborative filtering models to predict user ratings and generate personalized movie recommendations.

---

## 📊 Dataset

The dataset comes from the [Netflix Prize](https://www.kaggle.com/datasets/netflix-inc/netflix-prize-data), which contains:
- **100 million ratings** (1–5 stars) from **480,000+ users** on **17,000+ movies**.
- Data is spread across multiple text files (`combined_data_1.txt` to `combined_data_4.txt`).

---

## ⚙️ Project Workflow

1. **Data Preparation**  
   - Loaded and merged Netflix Prize text files.  
   - Cleaned and structured user–movie–rating interactions.  

2. **Exploratory Data Analysis (EDA)**  
   - Analyzed rating distribution and popularity of movies.  
   - Investigated user activity and sparsity of the dataset.  

3. **Modeling**  
   - Implemented **Collaborative Filtering** techniques:
     - User-based collaborative filtering  
     - Item-based collaborative filtering  
   - Considered matrix factorization methods (SVD).  

4. **Evaluation**  
   - Used RMSE (Root Mean Squared Error) to evaluate prediction accuracy.  
   - Compared model performance across different approaches.  

---

## 📈 Results and Conclusion

- Collaborative filtering successfully recommended movies based on user similarity and item similarity.  
- Matrix factorization methods like **SVD** offered better scalability and accuracy.  
- Insights show the potential of recommendation engines to personalize user experiences in streaming platforms.  

**Future work**:
- Implement deep learning approaches (Neural Collaborative Filtering, Autoencoders).  
- Add hybrid methods combining content-based and collaborative filtering.  
- Optimize performance for very large-scale datasets.
