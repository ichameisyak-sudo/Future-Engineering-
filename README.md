# Spaceflight News Analysis & Feature Engineering

Repositori ini berisi proyek Natural Language Processing (NLP) dan Web Scraping menggunakan Python. Proyek ini mencakup alur kerja end-to-end dari pengambilan data berita via API, text preprocessing, hingga feature engineering menggunakan statistik dan word embeddings (Word2Vec & FastText) serta visualisasi UMAP.

## Fitur Utama

- Web Scraping via API: Mengambil data artikel berita antariksa dari Spaceflight News API v4.
- Text Preprocessing:
  - Pembersihan HTML tags, URL, hashtag, angka, dan tanda baca.
  - Normalisasi teks ke lowercase.
  - Stopwords removal dan Stemming.
- Feature Engineering:
  - TF-IDF Vectorization (scikit-learn) untuk ekstraksi bobot kata.
  - Word2Vec Embedding (gensim) untuk pemetaan vektor kata berdasarkan konteks.
  - FastText Embedding (gensim) untuk penanganan n-gram sub-kata.
  - Document Vector Aggregation (mean pooling) untuk representasi level dokumen.
- Data Visualization: Reduksi dimensi vektor kata menggunakan UMAP dan Plotly.

## Teknologi & Library

- Python 3.x
- Pandas & NumPy
- Requests & JSON
- NLTK & Scikit-Learn
- Gensim (Word2Vec & FastText)
- UMAP-Learn & Plotly

git clone [https://github.com/USERNAME_KAMU/NAMA_REPO_KAMU.git](https://github.com/USERNAME_KAMU/NAMA_REPO_KAMU.git)
cd NAMA_REPO_KAMU
