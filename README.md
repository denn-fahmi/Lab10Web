# Lab10Web
Nama: Den Fahmi Satria
Nim: 312410523
Kelas: TI.24.A5

# Praktikum 10 – PHP OOP (Object Oriented Programming)

## Deskripsi
Praktikum 10 bertujuan untuk menerapkan konsep **Object Oriented Programming (OOP)** pada aplikasi PHP yang telah dibuat pada praktikum sebelumnya.  
Pada praktikum ini dilakukan **modularisasi kode menggunakan class library**, khususnya untuk **koneksi database** dan **pembuatan form**, sehingga kode program menjadi lebih terstruktur, reusable, dan mudah dikembangkan.

Aplikasi yang dikembangkan masih menggunakan database dari praktikum sebelumnya, yaitu pengelolaan **data barang**.

---

## Tujuan Praktikum
1. Memahami konsep dasar Object Oriented Programming (OOP)  
2. Mengimplementasikan class dan object pada PHP  
3. Menerapkan class library untuk koneksi database  
4. Menerapkan class library untuk pembuatan form  
5. Mengintegrasikan OOP dengan routing dan modularisasi tampilan  

---

## Struktur Direktori Project
```
lab10_php_oop/
│
├── config/
│ └── config.php
│
├── classes/
│ ├── Database.php
│ └── Form.php
│
├── layout/
│ ├── header.php
│ └── footer.php
│
├── pages/
│ └── barang/
│ ├── list.php
│ ├── tambah.php
│ ├── ubah.php
│ └── hapus.php
│
├── index.php
└── style.css
```

---

## Penjelasan Implementasi

### 1. Class Database
Class **Database** digunakan sebagai **library koneksi database** dan pengelolaan query.  
Class ini menangani operasi CRUD (Create, Read, Update, Delete) menggunakan metode OOP, sehingga halaman lain tidak perlu menulis ulang kode koneksi database.
<img src="web8/xampp.PNG" width="700"> <p>
### 2. Class Form
Class **Form** digunakan sebagai **library pembuatan form**.  
Dengan class ini, form input dapat dibuat secara dinamis dan lebih terstruktur tanpa menuliskan HTML form berulang kali di setiap halaman.

### 3. Routing dan Template
Routing tetap menggunakan **index.php** sebagai pengatur halaman dengan parameter **page**.  
Tampilan halaman dimodularisasi menggunakan **header.php** dan **footer.php** sehingga seluruh halaman memiliki tampilan yang konsisten.

### 4. Halaman List Data
File `list.php` digunakan untuk menampilkan data barang dari database.  
Data diambil menggunakan object dari class `Database`.

### 5. Halaman Tambah Data
File `tambah.php** digunakan untuk menambahkan data barang baru.  
Form input dibuat menggunakan class **Form**, dan proses penyimpanan data menggunakan class **Database**.

### 6. Halaman Ubah Data
File **ubah.php** digunakan untuk mengubah data barang yang sudah ada berdasarkan ID.  
Data lama ditampilkan kembali di form untuk diedit.

### 7. Halaman Hapus Data
File **hapus.php** digunakan untuk menghapus data barang dari database berdasarkan ID yang dipilih.

## Hasil Praktikum
Aplikasi CRUD data barang berhasil diimplementasikan menggunakan konsep OOP dengan: <p>
- Class library untuk database <p>
- Class library untuk form <p>
- Routing terpusat <p>
- Tampilan modular <p>

Seluruh fungsi CRUD berjalan dengan baik. <p>

## Kesimpulan
Dengan menerapkan konsep Object Oriented Programming dan class library, kode program menjadi lebih terstruktur, mudah dipelihara, dan dapat digunakan kembali.  <p>
Penggabungan konsep OOP, modularisasi, dan routing menghasilkan aplikasi PHP yang lebih rapi dan profesional. <p>

## Repository
Repository ini dibuat untuk memenuhi tugas **Praktikum 10 – Pemrograman Web**.
