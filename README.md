# 📺 STC Recommendation System

A movie recommendation engine developed for **STC Jawwy TV** to suggest movies to users based on their watch history and preferences. This system utilizes collaborative filtering techniques and machine learning models to identify patterns in user ratings and provide personalized content suggestions.

---

## 📂 Project Structure

- `stc TV_T3.ipynb`: Main Jupyter notebook that contains the data analysis, processing, model training, and recommendation logic.
- `stc TV Data Set_T3.xlsb`: The input dataset containing user ratings for movies, genres, and timestamps.
- `README.md`: Project documentation.

---

## 📊 Dataset Overview

The dataset contains:

- **user_id_maped**: Anonymized user ID
- **program_name**: The name of the movie/show
- **rating**: User rating (1-4)
- **date_**: Date of rating
- **program_genre**: Genre of the content

Total records: ~1,048,575 rows × 5 columns

---

## 🔍 Key Features

- **Data Cleaning**: Checked for missing values, verified types, and standardized genres and dates.
- **Pivot Table Construction**: Built a user-item matrix with users as columns and program names as rows.
- **Model Used**: `NearestNeighbors` from Scikit-Learn using cosine similarity.
- **Recommendation Logic**: For a given movie, the model finds similar titles based on user rating patterns.

---

## ⚙️ Getting Started

### Prerequisites

Make sure you have the following libraries installed:

```bash
pip install pyxlsb pandas numpy scikit-learn plotly matplotlib
