# 🚀 Cleaning-Data-1

## 📌 Deskripsi
Repositori **Cleaning-Data-1** berisi berbagai dataset yang digunakan untuk **pembersihan data (data cleaning)**.  
Tujuan utama dari repositori ini adalah untuk melakukan **preprocessing data** agar siap digunakan dalam **analisis data** atau **pemodelan machine learning**.  

## 📂 Dataset yang Tersedia
Repositori ini mencakup beberapa dataset dari berbagai domain, yaitu:  
- 🎧 **Audible Price Dataset** - Data harga audiobook di Audible  
- 🏡 **House Price Dataset** - Data harga properti dan spesifikasinya  
- 💻 **Laptop Price Dataset** - Data harga dan spesifikasi laptop  
- 📱 **Mobile Phone Price Dataset** - Data harga dan spesifikasi ponsel  
- 💰 **Salary Dataset** - Data gaji berdasarkan berbagai faktor  

## 📁 Struktur Folder
```
Cleaning-Data-1/
│── Audible_Price_Dataset/
│── House_Price_Dataset/
│── Laptop_Price_Dataset/
│── Mobile_Phone_Price_Dataset/
│── Salary_Dataset/
└── README.md
```
Setiap folder berisi dataset dalam berbagai format seperti **CSV** atau **Excel** yang akan digunakan dalam proses cleaning.  

## 🛠️ Langkah-langkah Data Cleaning
Berikut adalah langkah-langkah utama dalam proses pembersihan data:  
✅ **Menghapus nilai yang hilang (missing values)**  
✅ **Menghapus atau mengganti nilai yang tidak valid**  
✅ **Menormalisasi format data**  
✅ **Menghapus duplikasi data**  
✅ **Mengubah tipe data sesuai kebutuhan**  
✅ **Menghapus atau mengisi outlier jika diperlukan**  

## 🚀 Cara Menggunakan

### 📥 Clone repositori
```bash
git clone https://github.com/sanfla/Cleaning-Data-1.git
```

### 📂 Masuk ke direktori proyek
```bash
cd Cleaning-Data-1
```

### ⚙️ Install dependencies
Pastikan Anda telah menginstal **Python** dan pustaka berikut sebelum menjalankan kode:
```bash
pip install pandas numpy openpyxl
```

### 🧹 Jalankan skrip cleaning
Setelah semua persiapan selesai, jalankan skrip berikut untuk melakukan pembersihan data:
```bash
python cleaning_script.py
```

### 💡 Contoh Kode Cleaning
Berikut adalah contoh kode sederhana untuk membersihkan data menggunakan **Pandas**:
```python
import pandas as pd

# Membaca dataset
df = pd.read_csv("data/dataset.csv")

# Menghapus nilai yang hilang
df.dropna(inplace=True)

# Menghapus duplikasi
df.drop_duplicates(inplace=True)

# Mengonversi tipe data
df["harga"] = df["harga"].astype(float)

# Menyimpan hasil
df.to_csv("data/cleaned_dataset.csv", index=False)

print("✅ Data cleaning selesai!")
```
