# Praktikum5
# PENJELASAN PROGRAM INPUT NILAI MAHASISWA

Program ini dibuat menggunakan Python dan memanfaatkan struktur data Dictionary untuk menyimpan data mahasiswa. Program dapat menambah, mengubah, menghapus, menampilkan, dan mencari data mahasiswa melalui menu interaktif.



## 1. Tujuan Program

Program ini bertujuan:

Mengelola daftar nilai mahasiswa menggunakan dictionary.

Menyediakan menu interaktif yang memudahkan pengguna:

L : Lihat Data

T : Tambah Data

U : Ubah Data

H : Hapus Data

C : Cari Data

K : Keluar Program


Menghitung nilai akhir berdasarkan bobot yang ditentukan:

Tugas = 30%

UTS = 35%

UAS = 35%





## 2. Struktur Data (Dictionary)

Data mahasiswa disimpan dalam dictionary dengan format berikut:

data = {
    "NIM": {
        "nama": "...",
        "tugas": nilai,
        "uts": nilai,
        "uas": nilai,
        "akhir": nilai
    }
}

Key utama = NIM mahasiswa

Value = dictionary berisi data nilai mahasiswa


Struktur ini dipilih karena:

Mudah diakses menggunakan kunci

Cocok untuk menyimpan data banyak mahasiswa

Mudah diubah dan dihapus




## 3. Perhitungan Nilai Akhir

Nilai akhir dihitung menggunakan rumus:

Nilai Akhir = 30% * Tugas + 35% * UTS + 35% * UAS

Dalam program ditulis sebagai:

akhir = round((0.30 * tugas) + (0.35 * uts) + (0.35 * uas), 2)

Fungsi round() digunakan agar nilai akhir hanya tampil 2 angka di belakang koma.



## 4. Penjelasan Menu Program



###  (L) Lihat Data

Menu ini menampilkan seluruh data mahasiswa dalam bentuk tabel.

Jika data masih kosong, program akan menampilkan:

TIDAK ADA DATA



###  (T) Tambah Data

Pengguna memasukkan:

NIM

Nama

Nilai Tugas

Nilai UTS

Nilai UAS


Program menghitung nilai akhir, lalu menyimpan data ke dictionary.




###  (U) Ubah Data

Pengguna memasukkan NIM mahasiswa yang ingin diubah.

Jika NIM ditemukan:

Program meminta input nama dan nilai baru

Program menghitung ulang nilai akhir

Data diperbarui


Jika tidak ditemukan:

Data tidak ditemukan!



###  (H) Hapus Data

Pengguna memasukkan NIM mahasiswa yang ingin dihapus.

Jika ada → data dihapus
Jika tidak → tampil pesan error



###  (C) Cari Data

Pengguna memasukkan NIM untuk dicari.

Jika ditemukan → tampil data mahasiswa dalam bentuk tabel
Jika tidak → pesan error



###  (K) Keluar Program

Mengakhiri program.
