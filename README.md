# Spaceflight News Feature Engineering Task

Repositori ini berisi notebook Python untuk melakukan ekstraksi data berita dari Spaceflight News API serta pembentukan fitur berbasis Word Embeddings (Word2Vec & FastText), agregasi vektor dokumen, dan visualisasi reduksi dimensi UMAP.

---

## Deskripsi Proyek

Notebook ini terbagi menjadi dua bagian utama:

### 1. Ekstraksi Data & Tokenisasi
- Mengambil data ringkasan artikel berita antariksa dari Spaceflight News API (SNAPI v4).
- Mengubah teks ringkasan (summary) menjadi bentuk Lowercase dan melakukan Tokenisasi Kata (word tokenization) menggunakan NLTK.
- Output: Daftar token kalimat (sentences) yang siap diproses untuk pembentukan embedding.

### 2. Feature Engineering & Word Embeddings
- Model Word2Vec: Membangun model Word2Vec (Skip-Gram/CBOW) berdimensi 100 dengan Gensim, menyimpan model ke space_news.w2v, dan menampilkan analisis kata mirip (similar words).
- Model FastText: Membangun model FastText dengan n-gram sub-word (3-6) berdimensi 100, menyimpan model ke space_news.fasttext, dan melakukan pencarian kata mirip.
- Document Vector Aggregation: Menghitung nilai rata-rata vektor kata (mean pooling) dari setiap dokumen ringkasan untuk menghasilkan matriks fitur tingkat dokumen (df_w2v & df_ft).
- Visualisasi UMAP: Mereduksi dimensi vektor kata menjadi 2D (umap1, umap2) dan memvisualisasikan sebaran kata secara interaktif menggunakan Plotly.

---

## Library yang Digunakan

- requests — Mengambil data ringkasan artikel dari Spaceflight News API.
- pandas — Mengolah dan menyusun data ke dalam bentuk DataFrame.
- numpy — Melakukan kalkulasi rata-rata vektor (mean pooling) dokumen.
- nltk — Melakukan tokenisasi kata (word_tokenize).
- gensim — Membangun, menyimpan, dan memuat model Word2Vec dan FastText.
- umap-learn — Mereduksi dimensi vektor kata menjadi 2D.
- plotly — Memvisualisasikan scatter plot kata secara interaktif.

---

## Cara Menjalankan

1. Clone repositori ini:
   git clone https://github.com/ichameisyak-sudo/Web-Scraping.git
