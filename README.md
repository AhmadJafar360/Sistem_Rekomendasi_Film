# Sistem Rekomendasi Film

Proyek ini adalah **Sistem Rekomendasi Film** yang menggunakan **Natural Language Processing (NLP)** dan **Content Base Filtering** untuk merekomendasikan film berdasarkan kemiripannya dengan film yang dipilih. Rekomendasi dihitung dengan menganalisis deskripsi film, metadata, dan fitur lainnya.

---

## Fitur

1. **Content-Based Filtering**: Merekomendasikan film yang mirip dengan pilihan pengguna.
2. **NLP for Text Analysis**: Memproses deskripsi dan metadata dengan TF-IDF (Term Frequency - Inverse Document Frequency).
3. **Cosine Similarity**: Mengukur kesamaan antara film menggunakan fitur tekstual dan numerik gabungan.

---

## Instalasi

### Pra-Syarat
- Python 3.x
- Libraries:
  - pandas
  - scikit-learn
  - scipy

---

## Penggunaan
**Persiapkan data:**
  - Data berisi:
    - `title`: Judul Film
    - `description`: Deskripsi Film
    - `director`: Nama Sutradara
    - `cast`: Daftar Pemeran
    - `listed_in`: Genre Film
    - `release_year`: Tahun Rilis
    - `duration`: Durasi Film

---

## Model Perhitungan

### Preprocessing
  - `Case folding`: Ubah semua teks menjadi huruf kecil.
  - `Tokenizing`: Pisahkan teks menjadi token (kata-kata individu).
  - `Stopwords removal`: Hapus kata-kata umum seperti "dan", "atau", "yang".
  - `Stemming/Lemmatization`: Ubah kata ke bentuk dasarnya (misalnya, "berlari" menjadi "lari").
  - `TF-IDF Vectorization`: Representasikan teks menggunakan TF-IDF (Term Frequency - Inverse Document Frequency) untuk menghitung bobot kata-kata yang penting.

### Perhitungan
- Menggabungkan fitur TF-IDF dan normalized numerical features.
- Menggunakan **Cosine Similarity** to calculate the similarity between movies.

### Fungsi Rekomendasi
- Menemukan film yang paling mirip dengan judul yang diberikan.
- Mengurutkan berdasarkan skor kesamaan dan mengembalikan rekomendasi teratas.

---

## Library
- **Numpy**: Menyediakan array multidimensi, fungsi matematis, aljabar linear, transformasi Fourier, Numerik.
- **Scikit-learn**: Menyediakan alat untuk NLP dan pembelajaran mesin.
- **Pandas**: Digunakan untuk Pre-Processing.
- **Scipy**: Menangani Matriks.

---

## Saran Untuk Programmer AI & ML (Jika ingin menggunakan model lain)

1. **Collaborative Filtering**: Mengintegrasikan preferensi dan peringkat pengguna.
2. **Deep Learning**: Menggunakan jaringan saraf untuk rekomendasi yang lebih canggih.
3. **Web Application**: Implementasi ke frontend yang mudah digunakan menggunakan Flask, Django, atau Streamlit.

---

Thanks You!!
**MOHON MAAF JIKA ADA YANG SALAH DALAM PENJELASAN INI😁**