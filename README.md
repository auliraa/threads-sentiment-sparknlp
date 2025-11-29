# Threads App Sentiment Analysis with SparkNLP 🚀

Project ini adalah implementasi **SparkNLP** untuk melakukan analisis sentimen terhadap 37.000 ulasan aplikasi "Threads" (by Meta). Tujuannya adalah mengklasifikasikan ulasan pengguna secara otomatis menjadi **Positive**, **Negative**, atau **Neutral** untuk membantu tim pengembang memprioritaskan perbaikan bug.

## 📋 Dataset
Dataset yang digunakan berisi 37.000+ ulasan dari Google Play Store dan Apple App Store.
- **Source:** https://www.kaggle.com/datasets/shuvammandal121/37000-reviews-of-thread-app-dataset
- **Size:** 37,000 entities

## 🛠 Teknologi yang Digunakan
- **Python**
- **Apache Spark (PySpark)**
- **Spark NLP** (Library NLP untuk Big Data)
- **Pretrained Pipeline:** `sentimentdl_use_twitter` (Deep Learning model based on Universal Sentence Encoder)

## 📊 Hasil Analisis
Model berhasil mengklasifikasikan sentimen dengan distribusi sebagai berikut:
- **Positive:** ~21,000 ulasan (Mayoritas pengguna puas)
- **Negative:** ~13,000 ulasan (Fokus utama untuk perbaikan)
- **Neutral:** ~2,000 ulasan

*Insight:* Model mampu mendeteksi kalimat sarkasme sederhana dan slang internet (contoh: "Osm" terdeteksi positif).
