# 🛍️ Product Recommendation System

This is a simple **content-based recommendation system** that suggests similar products based on their textual descriptions. It uses natural language processing techniques and cosine similarity to recommend items that are frequently bought together or have similar names.

---

## 📦 Dataset

- **Source:** [Online Retail Dataset on Kaggle](https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset/data)
- This dataset contains 500,000+ transactions from a UK-based online retail store between 2010 and 2011.

---

## 🔧 Features

- Text preprocessing of product descriptions  
- Vectorization using `CountVectorizer`  
- Similarity calculation using `cosine_similarity`  
- Recommends top-N similar products based on user input  
- Includes fuzzy matching to handle partial or misspelled names  
- Handles missing values and noisy data

---

## 🧠 How It Works

1. **Data Cleaning**: Removes spaces, special characters, and null values.
2. **Feature Creation**: Combines product name and code to form a unique text feature.
3. **Vectorization**: Transforms text into numerical vectors using Bag-of-Words.
4. **Similarity Matrix**: Computes pairwise cosine similarity between all products.
5. **Recommendation**: When a product name is entered, it returns a sorted list of similar items with similarity scores.

---

## 🚀 Usage

1. Clone this repository.
2. Make sure the dataset file (`online_retail.csv`) is in the project directory.
3. Install required packages:

   ```bash
   pip install pandas sklearn numpy
