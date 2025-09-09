# 🌍 Aplikasi Prediksi Harga Tanah dengan IDW

Aplikasi web interaktif berbasis **Streamlit** untuk memprediksi harga tanah menggunakan metode interpolasi **Inverse Distance Weighting (IDW)**, dilengkapi dengan visualisasi interaktif menggunakan **Folium**.

---

## ✨ Fitur Utama

* 📂 **Unggah Data**: Upload dataset harga tanah dalam format CSV.
* 🧹 **Pembersihan Data Otomatis**: Validasi koordinat, tangani nilai hilang, dan filter outlier.
* ⚙️ **Parameter Interaktif**: Atur parameter IDW di sidebar:

  * Pangkat (*p*)
  * Metode jarak (*Haversine / Euclidean*)
  * Jumlah tetangga (*k*)
* 🗺️ **Visualisasi Peta**:

  * Peta interaktif Folium dengan basemap Google (Maps, Satellite, Hybrid).
  * Titik data acuan asli.
  * Heatmap sebaran prediksi harga.
* 📍 **Prediksi Titik Baru**:

  * Input lokasi tunggal melalui form.
  * Prediksi batch melalui CSV atau input teks.
* 💾 **Ekspor Hasil**: Unduh hasil prediksi grid dan batch dalam format CSV.

---

## 📂 Struktur Proyek

```bash
.
├── app.py                # Kode utama aplikasi Streamlit
├── requirements.txt      # Daftar pustaka Python yang dibutuhkan
├── data/
│   └── contoh_data.csv   # Contoh file data
└── README.md             # Dokumentasi proyek
```

---

## 🚀 Cara Menjalankan

### 1. Persiapan

Pastikan sudah terinstal **Python 3.10+** di sistem Anda.

### 2. Buat Virtual Environment (opsional tapi direkomendasikan)

```bash
python -m venv venv
```

Aktifkan environment:

* **Windows**

  ```bash
  venv\Scripts\activate
  ```
* **Linux / macOS**

  ```bash
  source venv/bin/activate
  ```

### 3. Instalasi Dependensi

```bash
pip install -r requirements.txt
```

### 4. Jalankan Aplikasi

```bash
streamlit run app.py
```

### 5. Akses di Browser

Aplikasi akan terbuka otomatis di browser. Jika tidak, buka URL berikut secara manual:
👉 [http://localhost:8501](http://localhost:8501)

---

## 📊 Contoh Dataset

File contoh tersedia di folder [`data/contoh_data.csv`](data/contoh_data.csv).

Format minimal:

```csv
latitude,longitude,harga
-6.200,106.816,5000000
-6.210,106.820,5200000
```

---

## 🛠️ Teknologi yang Digunakan

* [Streamlit](https://streamlit.io/)
* [Pandas](https://pandas.pydata.org/)
* [NumPy](https://numpy.org/)
* [Folium](https://python-visualization.github.io/folium/)
* [streamlit-folium](https://github.com/randyzwitch/streamlit-folium)

---
