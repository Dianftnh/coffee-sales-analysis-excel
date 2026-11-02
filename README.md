# ☕ Analisis Penjualan Kopi & Dashboard Interaktif Menggunakan Microsoft Excel

## 📌 Gambaran Umum Proyek
Proyek ini merupakan analisis data penjualan kopi menggunakan Microsoft Excel yang bertujuan untuk memahami performa penjualan, mengidentifikasi tren penjualan dari waktu ke waktu, serta mengetahui produk dan pelanggan yang memberikan kontribusi terhadap total penjualan.

Analisis dilakukan dengan menggabungkan beberapa tabel data, melakukan pengolahan dan transformasi data menggunakan formula Excel, menganalisis data menggunakan PivotTable, serta menyajikan hasil analisis melalui dashboard interaktif.

Melalui proyek ini, data transaksi yang awalnya berbentuk data mentah diolah menjadi informasi yang lebih terstruktur dan dapat digunakan sebagai dasar pengambilan keputusan bisnis.

## 🎯 Tujuan Analisis
Beberapa pertanyaan bisnis yang ingin dijawab melalui proyek ini adalah:
1. Bagaimana perkembangan penjualan kopi dari waktu ke waktu?
2. Jenis kopi apa yang memberikan kontribusi penjualan terbesar?
3. Negara mana yang menghasilkan total penjualan tertinggi?
4. Siapa saja lima pelanggan dengan total pembelian tertinggi?
5. Bagaimana performa penjualan berdasarkan kategori kopi dan jenis roast?

## 📂 Dataset

Dataset terdiri dari tiga tabel utama:

| Tabel | Deskripsi |
|---|---|
| Orders | Informasi transaksi, tanggal pemesanan, ID pelanggan, ID produk, dan jumlah pembelian |
| Customers | Informasi pelanggan, negara, dan status kartu loyalitas |
| Products | Informasi produk, jenis kopi, jenis roast, ukuran, harga satuan, dan profit |

### Ringkasan Dataset

| Informasi | Jumlah |
|---|---:|
| Total baris transaksi | 1.000 |
| ID pesanan unik | 957 |
| Pelanggan unik | 913 |
| Variasi produk | 48 |
| Negara | 3 |
| Periode data | Januari 2019 – Agustus 2022 |

## 🛠️ Tools dan Teknologi

Tools dan fitur Microsoft Excel yang digunakan dalam proyek ini:

- **Microsoft Excel:** Pengolahan data, analisis, dan pengembangan dashboard.
- **XLOOKUP:** Mengambil informasi pelanggan berdasarkan Customer ID.
- **INDEX & MATCH:** Mengambil dan menggabungkan informasi produk berdasarkan Product ID.
- **IF:** Melakukan transformasi kategori data.
- **PivotTable:** Meringkas dan menganalisis data berdasarkan berbagai kategori.
- **PivotChart:** Menyajikan hasil analisis dalam bentuk visualisasi.
- **Interactive Dashboard:** Menampilkan ringkasan analisis penjualan secara dinamis.

## 🔄 Tahapan Pengerjaan

### 1. Data Preparation & Data Integration

Tahap pertama dilakukan dengan menggabungkan tiga tabel utama, yaitu Orders, Customers, dan Products.

Proses yang dilakukan:
- Menghubungkan data transaksi dengan data pelanggan menggunakan Customer ID.
- Menghubungkan data transaksi dengan informasi produk menggunakan Product ID.
- Menggunakan XLOOKUP untuk mengambil informasi pelanggan.
- Menggunakan INDEX-MATCH untuk mengambil atribut produk.
- Mengubah kode kategori menjadi informasi yang lebih mudah dipahami.

### 2. Data Transformation

Setelah proses penggabungan data, dilakukan transformasi untuk menghasilkan informasi tambahan yang dibutuhkan dalam analisis.

Salah satu perhitungan utama adalah nilai penjualan setiap transaksi.

**Rumus perhitungan:**

`Sales = Quantity × Unit Price`

Nilai penjualan tersebut digunakan sebagai dasar untuk menganalisis performa penjualan berdasarkan waktu, negara, jenis kopi, dan pelanggan.

### 3. Exploratory Data Analysis (EDA)

Analisis dilakukan menggunakan PivotTable untuk memperoleh gambaran mengenai performa penjualan.

Beberapa analisis yang dilakukan:

- Analisis tren penjualan berdasarkan tahun dan bulan.
- Analisis penjualan berdasarkan jenis kopi.
- Analisis penjualan berdasarkan negara.
- Identifikasi lima pelanggan dengan total penjualan tertinggi.

### 4. Dashboard Development

Hasil analisis kemudian disajikan dalam bentuk dashboard interaktif menggunakan Microsoft Excel.

Dashboard terdiri dari tiga visualisasi utama:

- **Total Sales Over Time:** Menampilkan tren penjualan bulanan berdasarkan jenis kopi.
- **Sales by Country:** Membandingkan total penjualan berdasarkan negara.
- **Top 5 Customers:** Menampilkan lima pelanggan dengan total nilai penjualan tertinggi.

Dashboard memanfaatkan PivotTable dan PivotChart sehingga pengguna dapat mengeksplorasi informasi penjualan secara lebih dinamis.

## 📊 Hasil dan Temuan Analisis

Berdasarkan hasil pengolahan dan analisis data, diperoleh beberapa temuan berikut.

### 1. Performa Penjualan Keseluruhan

Total nilai penjualan yang diperoleh dari keseluruhan transaksi mencapai **45.134,26** dalam satuan mata uang dataset.

Analisis mencakup periode Januari 2019 hingga Agustus 2022 dengan total 1.000 baris transaksi.

### 2. Penjualan Berdasarkan Negara

Amerika Serikat menjadi negara dengan kontribusi penjualan terbesar, diikuti oleh Irlandia dan Inggris.

| Negara | Total Penjualan |
|---|---:|
| Amerika Serikat | 35.638,89 |
| Irlandia | 6.696,87 |
| Inggris | 2.798,51 |

Temuan ini menunjukkan bahwa Amerika Serikat merupakan pasar utama berdasarkan nilai penjualan dalam dataset.

### 3. Penjualan Berdasarkan Jenis Kopi

Excelsa menjadi jenis kopi dengan total penjualan tertinggi dibandingkan kategori lainnya.

| Jenis Kopi | Total Penjualan |
|---|---:|
| Excelsa | 12.306,44 |
| Liberica | 12.054,08 |
| Arabica | 11.768,50 |
| Robusta | 9.005,25 |

Hasil tersebut menunjukkan adanya perbedaan kontribusi penjualan di antara empat jenis kopi yang dianalisis.

### 4. Lima Pelanggan dengan Penjualan Tertinggi

Berikut lima pelanggan berdasarkan total nilai penjualan:

| Nama Pelanggan | Total Penjualan |
|---|---:|
| Allis Wilmore | 317,07 |
| Brenn Dundredge | 307,04 |
| Terri Farra | 289,11 |
| Nealson Cuttler | 281,67 |
| Don Flintiff | 278,01 |

Informasi ini dapat digunakan untuk mengidentifikasi pelanggan dengan kontribusi penjualan tertinggi.

## 📈 Dashboard Interaktif

Dashboard dikembangkan menggunakan Microsoft Excel untuk menyajikan ringkasan performa penjualan secara visual dan dinamis.

Fitur utama dashboard meliputi:

- Visualisasi tren penjualan berdasarkan waktu.
- Perbandingan penjualan berdasarkan negara.
- Peringkat lima pelanggan dengan total penjualan tertinggi.
- Eksplorasi data melalui fitur interaktif Excel.

Untuk melihat dashboard dan mencoba fitur interaktifnya, silakan unduh file Excel berikut:

**[📥 Lihat Dashboard & Hasil Analisis (Excel)](dashboard/coffeeOrdersProject.xlsx)**

## 💡 Rekomendasi Bisnis

Berdasarkan hasil analisis, terdapat beberapa rekomendasi yang dapat dipertimbangkan:

1. **Mempertahankan Pasar Utama:** Amerika Serikat memiliki kontribusi penjualan terbesar sehingga strategi pemasaran dan hubungan pelanggan di pasar tersebut perlu diperhatikan.
2. **Evaluasi Performa Produk:** Excelsa dan Liberica menunjukkan kontribusi penjualan yang tinggi sehingga dapat menjadi perhatian dalam pengembangan strategi produk.
3. **Meningkatkan Retensi Pelanggan:** Data pelanggan dengan nilai pembelian tertinggi dapat dimanfaatkan sebagai referensi untuk mengembangkan program loyalitas.
4. **Memantau Tren Penjualan:** Analisis penjualan bulanan dapat membantu bisnis memahami pola permintaan dan mendukung perencanaan stok maupun promosi.

## 📁 Struktur Repository

```text
coffee-sales-analysis-excel/
│
├── data/
│   └── coffeeOrdersData.xlsx
│
├── dashboard/
│   └── coffeeOrdersProject.xlsx
│
└── README.md
```

## 🎓 Skills yang Dikembangkan

Beberapa kemampuan yang diterapkan dan dikembangkan dalam proyek ini:

- Data Preparation & Data Integration
- Data Transformation
- Exploratory Data Analysis (EDA)
- Microsoft Excel Formulas
- XLOOKUP, INDEX & MATCH
- PivotTable & PivotChart
- Data Visualization
- Interactive Dashboard Development
- Business Insight Generation
- Data-Driven Decision Making

## 👩‍💻 Tentang Saya

**Dian Fatonah**

Lulusan Teknik Informatika | Data Analyst Enthusiast

Memiliki ketertarikan pada bidang Data Analytics, Data Science, dan Artificial Intelligence. Proyek ini merupakan bagian dari portofolio untuk mengembangkan kemampuan dalam mengolah data, melakukan analisis, serta menyajikan informasi yang dapat mendukung pengambilan keputusan.

- GitHub: [Dianftnh](https://github.com/Dianftnh)
- Portfolio: [Website Portofolio](https://website-dian-fatonah.vercel.app/)

---

*Proyek ini dibuat sebagai bagian dari pengembangan portofolio Data Analytics menggunakan Microsoft Excel.*
