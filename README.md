# 🛍️ Image-Based Fashion Recommendation System

This project implements an image similarity search engine for fashion products using a pretrained ResNet18 model. Given a reference image (either from the dataset or uploaded by a user), the system recommends visually similar fashion items based on image embeddings and cosine similarity.

---

## 📌 Problem Statement

Traditional text-based search fails to capture visual features like patterns, colors, and textures. This project solves that by enabling **image-based search and recommendation**, which is especially valuable in fashion e-commerce.

---

## 🔍 Use Case

- Upload an image (e.g., from your phone or internet)
- The model returns the top visually similar fashion items
- Helps in better product discovery and improves customer experience

---

## 🧠 Approach

1. **Dataset**: [Fashion Product Images (Kaggle)](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-small)
2. **Model**: Pretrained ResNet18 from PyTorch
3. **Feature Extraction**: Convert all images into 512-dim vectors
4. **Similarity Matching**: Cosine similarity between input and dataset vectors
5. **Visualization**: Top recommendations shown in grid layout

---

## 📂 Project Structure

image-similarity-recommendation/
│
├── notebooks/
│ └── image_similarity_project.ipynb ← Full implementation
│
├── data/
│ ├── styles.csv ← Metadata
│ ├── df_embs.pkl ← Precomputed embeddings
│
├── user_test_images/
│ └── test5.jpg ← Example user images
│
├── requirements.txt
├── README.md


---

## 🚀 How to Run

1. Clone this repository:

```bash
git clone https://github.com/yourusername/image-similarity-recommendation.git
cd image-similarity-recommendation

## Install dependencies:
pip install -r requirements.txt

## Open the notebook:
jupyter notebook notebooks/image_similarity_project.ipynb

## Test It Yourself
recm_user_input('your_image.jpg')
