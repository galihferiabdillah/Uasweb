# Uasweb

#NAMA:MUHAMMAD GALIH FERI ABDILLAH 

#E-Inventory Management System

E-Inventory adalah aplikasi sederhana untuk mengelola data inventaris barang dan kategori. Aplikasi ini dibangun menggunakan konsep Single Page Application (SPA) sehingga perpindahan halaman dilakukan tanpa me-refresh browser secara penuh.

Sistem ini terhubung dengan REST API yang dibuat menggunakan framework CodeIgniter 4, sehingga data dapat diakses, ditambah, diubah, dan dihapus secara dinamis melalui AJAX/Fetch API.

<img width="1366" height="214" alt="Capture" src="https://github.com/user-attachments/assets/0e5cd379-245e-4817-b3d5-50c9370f22b2" />

#Struktur Menu
1. Dashboard (Home)

Halaman utama aplikasi yang menampilkan informasi umum sistem inventaris.

Tampilan

Pada halaman Home terdapat:

Judul Dashboard E-Inventory
Menu navigasi:
Home
Barang
Kategori

# MENU BARANG 

<img width="1366" height="337" alt="Capture1" src="https://github.com/user-attachments/assets/a6f6fc43-42be-4051-9c21-d90ef9d9720a" />

Halaman ini digunakan untuk mengelola data barang.

Tampilan

Terdapat form input:

Field	Keterangan
Nama Barang	Nama barang yang akan disimpan
Stok	Jumlah stok barang
Kategori ID	ID kategori barang
Simpan	Tombol untuk menyimpan data

Di bawah form terdapat tabel:

Kolom
ID
Nama
Stok
Aksi
Fungsi Menu Barang
Tambah Barang

Pengguna dapat memasukkan:

Nama Barang
Jumlah Stok
Kategori ID

Kemudian klik tombol Simpan.

Data akan dikirim ke API:

POST /barang
Menampilkan Barang

Saat halaman dibuka, sistem mengambil data dari API:

GET /barang

dan menampilkannya ke tabel.

Edit Barang

Tombol Edit digunakan untuk mengubah data barang.

API yang digunakan:

PUT /barang/{id}
Hapus Barang

Tombol Hapus digunakan untuk menghapus data barang.

API yang digunakan:

DELETE /barang/{id}
3. Menu Kategori

Menu ini digunakan untuk mengelola kategori barang.

Tampilan

Tabel kategori terdiri dari:

Kolom
ID
Nama Kategori
Fungsi Menu Kategori
Menampilkan Kategori

Sistem mengambil data kategori dari API:

GET /kategori

kemudian menampilkannya pada tabel.

Menambah Kategori

Data kategori baru dikirim ke API:

POST /kategori
Mengubah Kategori

Menggunakan endpoint:

PUT /kategori/{id}
Menghapus Kategori

Menggunakan endpoint:

DELETE /kategori/{id}


