# Analisis Sentimen & Word Embedding Mobil Listrik (NLP Lanjutan)

> Proyek Pemrosesan Bahasa Alami (NLP) tingkat lanjut untuk analisis sentimen ulasan/komentar publik mengenai mobil listrik menggunakan Python, implementasi *Skip-Gram Word Embedding* dari awal (*from scratch*), serta visualisasi data eksploratif.

## 📌 Tentang Proyek
Proyek ini dikembangkan untuk menganalisis opini dan sentimen masyarakat terkait isu mobil listrik di Indonesia berdasarkan data ulasan (*dataset mobil_listrik.csv*). Repositori ini mendemonstrasikan kemampuan pengolahan teks bahasa Indonesia secara mendalam, mulai dari pembersihan data, normalisasi kata slang, *stopword removal* (Sastrawi), hingga pembangunan arsitektur *Word Embedding* mandiri menggunakan NumPy dan visualisasi statistik.

## 🚀 Fitur & Tahapan Proyek

### 1. Data Understanding & Preprocessing
* **Eksplorasi Data (EDA):** Membaca dataset, memeriksa tipe data, menangani nilai kosong (`dropna`), dan analisis statistik deskriptif.
* **Text Cleaning & Normalization:** Pengubahan teks menjadi huruf kecil (*lowercase*), normalisasi kata tidak baku/slang (misal: *dgn* -> *dengan*, *gue* -> *saya*, dll.), serta penghapusan *stopword* menggunakan pustaka `Sastrawi` dan `NLTK`.
* **Tokenisasi:** Memecah teks ulasan menjadi token kata bersih yang hanya berisi huruf alfabet.

### 2. Skip-Gram Word Embedding (From Scratch)
* **Training Pairs Generation:** Membentuk pasangan kata target dan konteks (*skip-gram*) berdasarkan *window size* tertentu.
* **Custom Neural Network Training:** Menginisialisasi matriks bobot (*W1* dan *W2*), fungsi aktivasi *softmax*, dan melatih model secara manual menggunakan NumPy (*training loop* dengan optimasi *gradient descent*).
* **Word Similarity Evaluation:** Menggunakan metrik *Cosine Similarity* untuk mengevaluasi kedekatan semantik antar kata berdasarkan vektor yang telah dilatih.

### 3. Visualisasi & Analisis Sentimen
* **Wordcloud:** Menghasilkan visualisasi awan kata (*word cloud*) untuk memetakan istilah yang paling dominan pada kategori sentimen Netral dan Negatif.
* **Distribusi Sentimen (Pie Chart):** Analisis proporsi kelas sentimen publik, yang menunjukkan dominasi ulasan Negatif (57.3%), diikuti Positif (33.3%), dan Netral (9.4%).

---

## 🛠️ Teknologi & Pustaka
* **Bahasa Pemrograman:** Python
* **NLP & Text Processing:** NLTK, Sastrawi, Regular Expressions (`re`)
* **Machine Learning & Math:** NumPy, Pandas, Scikit-Learn, Imbalanced-Learn (SMOTE)
* **Visualisasi Data:** Matplotlib, Seaborn, WordCloud
* **Environment:** Google Colab / Jupyter Notebook

## ⚙️ Cara Menjalankan
1. Clone repositori ini:
   ```bash
   git clone [https://github.com/wiwindaaulia/-PemrosesanBahasaAlamiLanjut.git](https://github.com/wiwindaaulia/-PemrosesanBahasaAlamiLanjut.git)
