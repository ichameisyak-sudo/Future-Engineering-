# Natural Language Processing & Feature Engineering Task

Repositori ini berisi notebook Python untuk melakukan pengolahan data berbasis teks menggunakan dua metode utama: Text Preprocessing dan Feature Engineering.

---

## Deskripsi Proyek

Notebook ini terbagi menjadi dua bagian utama:

### 1. Text Preprocessing
- Pembersihan Teks: Menghapus tag HTML, URL, hashtag, tanda baca, dan angka menggunakan Regular Expression (re).
- Normalisasi Teks: Mengubah seluruh teks menjadi huruf kecil (lowercasing).
- Filtering & Stemming: Menghapus stopwords dan melakukan stemming pada teks.
- Output: spaceflight_preprocessed.csv berisi teks hasil preprocessing.

### 2. Feature Engineering & Embeddings
- TF-IDF Vectorization: Mengubah teks menjadi matriks bobot TF-IDF menggunakan scikit-learn.
- Word Embeddings (Word2Vec & FastText): Memetakan kata ke dalam ruang vektor kontinu menggunakan gensim.
- Document Vector Aggregation: Menghitung rata-rata vektor kata (mean pooling) untuk representasi level dokumen.
- Visualisasi UMAP: Mereduksi dimensi vektor kata menjadi 2D dan memvisualisasikannya secara interaktif menggunakan Plotly.

---

## Library yang Digunakan

- pandas — Menyusun dan menampilkan data dalam bentuk tabular (DataFrame).
- numpy — Pemrosesan data array dan operasi vektor.
- nltk — Pemrosesan bahasa alami (tokenisasi, stopwords).
- scikit-learn — Ekstraksi fitur teks menggunakan TF-IDF.
- gensim — Membangun model Word2Vec dan FastText.
- umap-learn — Reduksi dimensi fitur kata.
- plotly — Visualisasi grafik interaktif.

---

## Cara Menjalankan

1. Clone repositori ini:
   git clone https://github.com/ichameisyak-sudo/Web-Scraping.git
