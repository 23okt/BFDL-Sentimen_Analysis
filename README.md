# BFDL-Sentimen_Analysis

# 🎯 Sentiment Analysis Komentar YouTube Windah Basudara

Proyek ini bertujuan untuk melakukan analisis sentimen pada komentar video YouTube dari channel **Windah Basudara**, menggunakan pendekatan _Natural Language Processing (NLP)_ dan _Machine Learning_.

Oleh: Muhammad Gilang Ramadhan  
Program: Laskar AI - AI Engineer 2025

---

## 📌 Deskripsi Proyek

Komentar pada video YouTube dapat mengandung opini beragam. Dalam proyek ini, dilakukan scraping komentar dari salah satu video populer Windah Basudara dan dianalisis apakah komentar tersebut bernada **positif**, **netral**, atau **negatif** menggunakan model klasifikasi teks.

---

## 🧾 Struktur Proyek

1. **`scrapping.ipynb`**

   - Mengambil komentar dari video YouTube menggunakan YouTube API dan `pytube`
   - Menyimpan hasil scraping dalam bentuk dataframe
   - Proses cleaning komentar (menghilangkan emoji, simbol, stopwords, dsb.)

2. **`model.ipynb`**
   - Melabeli data sentimen secara manual/semi-otomatis (positif, netral, negatif)
   - Pra-pemrosesan teks: tokenisasi, stopword removal, stemming (menggunakan Sastrawi)
   - Ekstraksi fitur: TF-IDF
   - Model klasifikasi: Random Forest
   - Evaluasi: Akurasi, Confusion Matrix, Classification Report
   - Prediksi sentimen terhadap komentar-komentar yang telah di-scrape

---

## 🔍 Tools & Library

- Python
- pandas, numpy
- Sastrawi (stemming bahasa Indonesia)
- scikit-learn
- matplotlib, seaborn
- pytube / Google API Client (untuk scraping komentar YouTube)
- Jupyter Notebook

---

## 🧠 Metodologi

1. **Scraping Data Komentar**
   - Menggunakan `pytube` untuk mengambil komentar dari video YouTube tertentu
2. **Preprocessing Teks**
   - Lowercasing, menghapus simbol, angka, dan stopword bahasa Indonesia
3. **Labeling Data**
   - Komentar dikategorikan ke dalam sentimen `Positif`, `Negatif`, dan `Netral`
4. **Ekstraksi Fitur**
   - Menggunakan TF-IDF untuk mengubah teks menjadi fitur numerik
5. **Pelatihan Model**
   - Menggunakan Random Forest Classifier untuk memprediksi sentimen
6. **Evaluasi**
   - Menggunakan metrik evaluasi standar klasifikasi

---

## 📈 Hasil

Model mampu mengklasifikasikan komentar YouTube dengan tingkat akurasi yang cukup baik dan memberikan wawasan terkait sentimen penonton terhadap konten Windah Basudara.

---

## 🚀 Cara Menjalankan

1. **Install dependensi**:
   ```bash
   pip install pandas numpy scikit-learn sastrawi matplotlib seaborn pytube
   ```
2. Buka notebook:
   Jalankan Jupyter dan buka:

- scrapping.ipynb → untuk mengambil dan membersihkan komentar
- model.ipynb → untuk membangun dan evaluasi model sentimen

📚 Pembelajaran

- Penerapan NLP dalam Bahasa Indonesia
- Membangun pipeline text classification dari nol
- Penerapan Machine Learning untuk analisis media sosial
- Analisis opini publik melalui komentar YouTube
