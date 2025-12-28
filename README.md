# British Airways Data Science Project

## Overview

This project simulates a **Data Scientist role at British Airways**, focusing on understanding customer sentiment and predicting booking behaviour. It is divided into two core tasks:

1. **Web Scraping & Sentiment Analysis** – Extracting and analyzing customer reviews to uncover insights into service quality.
2. **Predictive Modelling** – Building a machine learning model to predict whether a customer will complete a booking.

---
- **Task 1**
  - `WebScraping_and_Analysis.ipynb` – Scraping Skytrax reviews and performing sentiment analysis  

- **Task 2**
  - `BA_Task_2_Predicting_Customer_Buying_Behavior.ipynb` – EDA and predictive modelling  

- **Data**
  - `BA_reviews.csv` – Raw scraped review data  
  - `Cleaned_BA_reviews.csv` – Cleaned and processed review data  
  - `customer_booking.csv` – Dataset for booking prediction  

- **Presentation**
  - `BA_Task_1_WebScraping_Sentiment_Analysis.pptx` – Summary of insights and findings
  -  task 2 ppt 
---

## Task 1: Web Scraping & Sentiment Analysis

### Objective
To scrape customer review data from **Skytrax (airlinequality.com)** and analyze customer sentiment to identify strengths, weaknesses, and improvement opportunities.

### Key Steps

1. **Web Scraping**
   - Collected 2,000+ British Airways customer reviews using `BeautifulSoup` and `requests`.

2. **Data Cleaning**
   - Removed special characters and stopwords
   - Converted text to lowercase
   - Applied tokenization and lemmatization using `NLTK`

3. **Text Analysis**
   - Sentiment analysis to classify reviews as positive, negative, or neutral  
   - Word clouds to visualize frequent terms  
   - Topic modelling to identify recurring themes such as:
     - Baggage handling
     - Cabin crew & customer service
     - Food quality
     - Flight punctuality

---

## Task 2: Predicting Customer Buying Behaviour

### Objective
To build a machine learning model that predicts the likelihood of a customer completing a booking.

### Dataset Overview

The `customer_booking.csv` dataset includes:

- `sales_channel` (Internet / Mobile)
- `trip_type` (RoundTrip / OneWay / CircleTrip)
- `purchase_lead`
- `length_of_stay`
- `flight_hour`, `flight_day`
- `wants_extra_baggage`
- `wants_preferred_seat`
- `wants_in_flight_meals`

### Methodology

1. **Exploratory Data Analysis (EDA)**
   - Visualized feature distributions and booking trends

2. **Feature Engineering**
   - Encoded categorical variables
   - Handled missing values

3. **Machine Learning**
   - Trained a **Random Forest Classifier**
   - Used **Logistic Regression** as a baseline model

4. **Evaluation**
   - Evaluated model accuracy and performance metrics
   - Analyzed feature importance to explain booking behaviour

---

## Technologies Used

- **Python**
- **Web Scraping:** BeautifulSoup, requests
- **Data Manipulation:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn, WordCloud
- **Machine Learning:** scikit-learn
- **NLP:** NLTK

