# H&m-fashion-recommendation-system

# H&M Fashion Recommendation System

A hybrid product recommendation engine that combines **content-based filtering** using TF-IDF and **collaborative filtering** using autoencoders, built on the H&M Personalized Fashion Recommendation dataset. This system recommends fashion items based on user preferences, article descriptions, and purchase history.

---

## Dataset

- Source: [H&M Personalized Fashion Recommendation](https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data)
- Main files:
  - `articles.csv`
  - `customers.csv`
  - `transactions_train.csv`
  - Image folder: `/images/0xxxx/0xxxxxx.jpg`

---

## Features Implemented

### Data Preprocessing & EDA
- Missing value treatment
- Age distribution, club member status, category analysis
- Article popularity and pricing over time

### Content-Based Filtering
- TF-IDF vectorization on `detail_desc`
- Cosine similarity for article-article recommendation

### Image Display
- Dynamically loads top purchased and recommended article images

### Collaborative Filtering
- Binary interaction matrix from transactions
- Autoencoder with dropout regularization
- Recommendation score matrix generated from trained latent representation

---

##  Recommendation Methods

| Method              | Technique                   | Description                                      |
|---------------------|-----------------------------|--------------------------------------------------|
| Content-Based       | TF-IDF + Cosine Similarity  | Recommends similar items using descriptions      |
| Collaborative       | Autoencoder Neural Network  | Recommends based on customer-article interactions |
| Hybrid              | Visual + Text + Behavior    | Combines article descriptions and purchase patterns |

---

## Example Visual Output

### Articles Previously Purchased

![Purchased Items]
![image](https://github.com/user-attachments/assets/e81acf1a-2710-48a1-993a-07d8da266672)


### Recommended Articles
![image](https://github.com/user-attachments/assets/86565e13-6fd5-4a17-8568-a9651ca41eda)

![Purchased Items]

![image](https://github.com/user-attachments/assets/0b5f2e77-0bc3-48d4-bd8a-9ff01c8c218d)
![image](https://github.com/user-attachments/assets/df749dfd-88c9-4c5a-8221-60a989cf5238)





