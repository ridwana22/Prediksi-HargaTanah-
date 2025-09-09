🌍 Aplikasi Prediksi Harga Tanah dengan IDWAplikasi web interaktif yang dibangun dengan Streamlit untuk memprediksi harga tanah menggunakan metode interpolasi Inverse Distance Weighting (IDW) dan memvisualisasikannya di peta Folium.Fitur UtamaUnggah Data: Pengguna dapat mengunggah data harga tanah dalam format CSV.Pembersihan Data Otomatis: Aplikasi secara otomatis membersihkan data, memvalidasi koordinat, menangani nilai yang hilang, dan memfilter outlier.Parameter Interaktif: Sesuaikan parameter IDW seperti pangkat (p), metode jarak (Haversine/Euclidean), dan jumlah tetangga (k) melalui sidebar.Visualisasi Peta:Peta interaktif menggunakan Folium dengan pilihan basemap dari Google (Maps, Satellite, Hybrid).Tampilan titik data acuan asli.Heatmap yang menunjukkan sebaran prediksi harga di seluruh area.Prediksi Titik Baru:Lakukan prediksi untuk satu lokasi dengan mengisi form.Lakukan prediksi untuk banyak lokasi (batch) dengan mengunggah CSV atau memasukkan data teks.Ekspor Hasil: Unduh hasil prediksi grid dan prediksi batch sebagai file CSV.Struktur Proyek.
├── app.py                # Kode utama aplikasi Streamlit
├── requirements.txt      # Daftar pustaka Python yang dibutuhkan
├── data/
│   └── contoh_data.csv   # Contoh file data untuk diunggah
└── README.md             # File ini
Cara Menjalankan AplikasiPastikan Python TerinstalPastikan Anda memiliki Python 3.10 atau versi yang lebih baru terinstal di sistem Anda.Buat Lingkungan Virtual (Opsional tapi Direkomendasikan)python -m venv venv
source venv/bin/activate  # Di Windows, gunakan: venv\Scripts\activate
Instal Pustaka yang DiperlukanNavigasikan ke direktori proyek dan jalankan perintah berikut di terminal Anda:pip install -r requirements.txt
Jalankan Aplikasi StreamlitSetelah instalasi selesai, jalankan aplikasi dengan perintah:streamlit run app.py
Buka di BrowserAplikasi akan otomatis terbuka di browser web default Anda. Jika tidak, buka browser dan navigasikan ke alamat URL yang ditampilkan di terminal (biasanya http://localhost:8501).Selamat mencoba!
