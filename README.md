# 📊 Analisis Klaster Pelanggan Toko Online

## 👥 Anggota Kelompok
-	Farel Nouval Daswara (1214070)
-	Aditya Firmansyah (714220038)
-	ALFIAN BENARDO RUSLI (714220048)


---

## 📌 Deskripsi Kasus

Pada era digital, toko online menghasilkan jutaan data transaksi yang berharga namun belum sepenuhnya dimanfaatkan. Penelitian ini bertujuan untuk melakukan segmentasi pelanggan berdasarkan perilaku belanja mereka menggunakan pendekatan RFM (Recency, Frequency, Monetary) dan metode clustering K-Means. Dengan segmentasi yang baik, toko online dapat menentukan strategi pemasaran yang lebih efektif untuk mempertahankan pelanggan loyal dan mengaktifkan kembali pelanggan yang pasif.

---

## 📁 Sumber Dataset

Dataset publik dari **Kaggle**:
- **Judul:** [Online Retail Dataset](https://www.kaggle.com/datasets/hellbuoy/online-retail)
- **Periode:** Desember 2010 – Desember 2011
- **Ukuran:** ± 397.884 baris transaksi

---

## 🔧 Langkah Preprocessing

1. Menghapus transaksi dengan `Quantity` dan `UnitPrice` ≤ 0
2. Menghapus data yang tidak memiliki `CustomerID`
3. Menambahkan kolom `TotalAmount` (Quantity × UnitPrice)
4. Menghapus duplikat transaksi
5. Menghitung nilai RFM untuk setiap pelanggan
6. Transformasi log dan normalisasi fitur RFM

---

## 🤖 Algoritma yang Digunakan

- **Segmentasi Pelanggan:**  
  - **RFM Analysis** (Recency, Frequency, Monetary)
  - **K-Means Clustering** (unsupervised learning)
  
- **Visualisasi Dimensi:**  
  - PCA (Principal Component Analysis) untuk reduksi dimensi 2D

---

## 📊 Evaluasi & Hasil

- **Elbow Method:** Menentukan jumlah klaster optimal (k = 4)
- **Silhouette Score:** Mengevaluasi kualitas klaster
- **PCA Scatter Plot:** Visualisasi persebaran klaster
- **Interpretasi Klaster:** Setiap klaster dianalisis berdasarkan nilai rata-rata RFM-nya untuk identifikasi tipe pelanggan (loyal, potensial, dorman, dll.)

---

## ▶️ Cara Menjalankan Proyek

1. **Clone repository:**
   ```bash
   git clone https://github.com/AditWiBu69/Analisis-Klaster-Pelanggan-Toko-Online
   cd nama-repo
2. ** Install dependencies
   pip install -r requirements.txt
3. ** Jalankan notebook
   -Buka file analisis_klaster_rfm.ipynb menggunakan jupyter notebook atau google colab
   - Eksekusi sel dari atas ke bawah
