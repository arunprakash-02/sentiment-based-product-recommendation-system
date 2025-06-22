# Ebuss Sentiment-Based Product Recommendation System
---
Welcome to the Sentiment-Based Product Recommendation System, an end-to-end Machine Learning project designed as part of the upGrad & IIIT-B Machine Learning and AI Program – April 2024.This project simulates a real-world scenario at a fictional e-commerce company named Ebuss, aiming to enhance product recommendations by combining collaborative filtering and sentiment analysis.


## Problem Statement
---
With rising competition in the e-commerce space, Ebuss wants to offer highly personalized product recommendations to its users. As a Senior ML Engineer, your mission is to build a sentiment-driven recommendation system using product reviews and ratings.

The system will:

Analyze customer reviews to extract sentiment.

Use these sentiments to improve product recommendations.

Deploy the entire system as a web app using Flask and Heroku.


---

  ## Project Structure

```
├── app.py                   # Flask app to run backend logic
├── model.py                 # Contains final ML model + recommendation logic
├── index.html               # Frontend UI for user interaction
├── sentiment_model.pkl      # Trained sentiment classification model
├── recommendation.pkl       # Saved recommendation system
├── templates/
│   └── index.html           # HTML file for web interface
├── requirements.txt         # Python dependencies
└── README.md                
```

**Workflow Summary:**
- **Data Preprocessing & Sentiment Analysis:**
  1.  Exploratory Data Analysis (EDA)
  2.  Text Cleaning & Preprocessing : Lowercasing, punctuation removal, stopword filtering, lemmatization
  3.  Feature Extraction: TF-IDF Vectorization
  4.  Model Building (at least 3 models out of 4):
      Logistic Regression
      Naive Bayes
      Random Forest
      XGBoost
  6.  Best Model Selection based on Accuracy, F1-Score, etc.

- **Recommendation System:**
  1.  User-Based Collaborative Filtering
  2.  Item-Based Collaborative Filtering
Chosen Approach based on performance metrics: RMSE
Output: Recommend 20 products per user based on historical ratings

-  **Sentiment-Driven Filtering:**
From the top 20 recommendations, we pick the top 5 products with the highest positive sentiment scores (based on review text).

-  **Deployment:**
 1.  Built interactive UI using Flask
 2.  Deployed on Heroku

---

## Tech Stack

- **Python:** Version 3.7 or higher
- **NLP:** NLTK, scikit-learn
- **Modeling:** XGBoost
- **Deployment:** Heroku
- **Web Framework:** Flask
- **Libraries:**  Pandas, NumPy, Pickle, Matplotlib


### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/arunprakash-02/sentiment-based-product-recommendation-system.git
   cd sentiment-based-product-recommendation-system
   ```

2. **Install Dependencies:**

   ```bash
  
   pip install -r requirements.txt
   ```
3. **Run locally:**

   ```bash
  
   python app.py
   ```
  Visit http://127.0.0.1:5000/ in your browser.

4.**Deployment on Heroku:**
  Push your code to a Heroku app using Git.
  Make sure to include: Procfile , requirements.txt

## Dataset Overview
  Reviews: 30,000+
  Users: 20,000+
  Products: 200+
  Key Fields:  reviews_username, reviews_rating , reviews_text, product_name

## License

This project is open-source and available under the [MIT License](LICENSE).

---

## Contact & Acknowledgements

For questions or further information, please reach out to:

- **Maintainer:** [Arun Prakash]
- **Email:** [prakash.arun01@gmail.com]
