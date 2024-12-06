# Linux Fundamentals: Interacting with the File System

Linux adalah sistem operasi berbasis Unix yang menggunakan file system untuk mengatur dan menyimpan data. Dalam Linux, interaksi dengan file system sangat penting untuk mengelola file dan direktori. Berikut adalah beberapa konsep dasar dan perintah yang digunakan untuk berinteraksi dengan file system di Linux.

## Struktur File System Linux

Linux menggunakan struktur **hierarkis** untuk menyimpan file. Semua file dan direktori di Linux terletak di bawah direktori **root** (`/`), yang menjadi titik awal dari seluruh file system. Beberapa direktori penting dalam file system Linux adalah:

- `/bin`: Menyimpan file eksekusi penting untuk sistem.
- `/etc`: Menyimpan file konfigurasi sistem.
- `/home`: Direktori untuk menyimpan data pengguna.
- `/var`: Menyimpan file yang sering berubah, seperti log dan database.
- `/usr`: Menyimpan program dan file sistem yang digunakan oleh pengguna.

Berikut adalah beberapa daftar command untuk berinteraksi dengan file sistem:

| Command  | Deskripsi                                  |
|----------|--------------------------------------------|
| `pwd`    | Menampilkan direktori kerja saat ini.      |
| `cd`     | Berpindah ke direktori tertentu.           |
| `ls`     | Menampilkan daftar file dan direktori.     |
| `mkdir`  | Membuat direktori baru.                    |
| `rmdir`  | Menghapus direktori kosong.                |
| `touch`  | Membuat file baru atau memperbarui file.   |
| `cp`     | Menyalin file atau direktori.              |
| `mv`     | Memindahkan atau mengganti nama file.      |
| `rm`     | Menghapus file atau direktori.             |
| `cat`    | Menampilkan isi file teks.                 |
| `chmod`  | Mengubah hak akses file atau direktori.    |
| `chown`  | Mengubah kepemilikan file atau direktori.  |
| `mount`  | Memasang perangkat penyimpanan.            |
| `umount` | Melepas perangkat penyimpanan.             |


### Contoh penggunaan:
+ **`cd` (Change Directory)**
  ```bash
  cd folderku
  ```
  {% hint style="info" %}
  Kalian juga dapat menggunakan cara seperti beriku: `cd folder1/folder2/folder3` untuk langsung mengarah ke folder3.
  Atau kalian dapat menggunakan `cd ~` untuk langsung kembali ke /home atau cukup `cd`
  Untuk kembali ke folder diatasnya, kalian dapat menggunakan `cd ..`, dan untuk kembali ke folder sebelumnya,kalian dapat menggunakan `cd -`
  {% endhint %}
+ 