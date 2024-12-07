# Analisis RFM (Recency, Frequency, Monetary)

## Pendahuluan
Di era digital, data menjadi aset strategis yang sangat berharga bagi perusahaan, terutama data pelanggan pada e-commerce. Dengan meningkatnya volume transaksi online, perusahaan menghadapi tantangan untuk memahami perilaku konsumen secara mendalam. **RFM Analysis** hadir sebagai solusi komprehensif untuk mengubah data mentah menjadi wawasan strategis yang actionable.


## Tentang Dataset  
**Dataset terdiri dari beberapa informasi utama:**  
- **Informasi Pelanggan**: CustomerID, Gender, Location, Tenure_Months.  
- **Detail Transaksi**: Transaction_ID, Transaction_Date, Product_SKU, Product_Category.  
- **Informasi Keuangan**: Coupon_Status, Offline_Spend, Online_Spend, Discount_pct.

> **Link Dataset**: [🛒 Online Shopping Dataset 📊📉📈](#)

## Pernyataan Masalah
- Siapa 5 pelanggan dengan kontribusi pembelian tertinggi?
- Negara bagian mana yang memiliki kontribusi pembelian tertinggi?
- Kapan transaksi paling banyak terjadi, dan apa pola temporalnya?

## Implementasi RFM
1. **Recency**: Mengukur jumlah hari sejak transaksi terakhir hingga tanggal referensi (misalnya 2020/01/01).  
2. **Frequency**: Menghitung jumlah transaksi untuk setiap pelanggan.  
3. **Monetary**: Menjumlahkan total pengeluaran pelanggan.  

### Proses Segmentasi
- Pelanggan diberi skor 1-5 pada masing-masing dimensi (R, F, M) menggunakan metode binning.  
- Skor RFM dikombinasikan menjadi string kategorikal, seperti `R3F5M4`.

### Interpretasi RFM Score
| **Segmen**           | **Deskripsi**                                         |
|-----------------------|-------------------------------------------------------|
| **Champions**         | Pelanggan terbaik dengan frekuensi dan nilai tinggi.  |
| **Loyal Customers**   | Sering bertransaksi dengan nilai stabil.              |
| **Potential Loyalists** | Menunjukkan tanda-tanda loyalitas.                  |
| **New Customers**     | Baru pertama kali bertransaksi.                      |
| **Hibernating**       | Pelanggan jarang bertransaksi.                       |
| **At Risk**           | Dulunya aktif, kini mulai menjauh.                   |
| **Can't Lose**        | Pelanggan VIP dengan frekuensi yang menurun.         |
| **Promising**         | Pelanggan baru dengan potensi besar.                 |

## Visualisasi Data
### Treemap

Treemap menunjukkan distribusi kontribusi tiap segmen pelanggan:
- Segmen **"Loyal Customers"** dan **"Champions"** memiliki kontribusi terbesar.
- Segmen **"At Risk"** dan **"Can't Lose"** membutuhkan perhatian lebih untuk retensi.

### Dashboard
- **Link Tableau**: [🛒 Online Shopping Dataset 📊📉📈](#)

## Hasil Analisis dan Rekomendasi


---

> **Catatan**: Implementasi lengkap dan kode dapat dilihat pada repositori ini.
