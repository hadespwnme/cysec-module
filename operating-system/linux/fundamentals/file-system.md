# Linux Fundamentals: Interacting with the File System

Linux adalah sistem operasi berbasis Unix yang menggunakan file system untuk mengatur dan menyimpan data. Dalam Linux, interaksi dengan file system sangat penting untuk mengelola file dan direktori. Berikut adalah beberapa konsep dasar dan perintah yang digunakan untuk berinteraksi dengan file system di Linux.

## Struktur File System Linux

Linux menggunakan struktur **hierarkis** untuk menyimpan file. Semua file dan direktori di Linux terletak di bawah direktori **root** (`/`), yang menjadi titik awal dari seluruh file system. Beberapa direktori penting dalam file system Linux adalah:

- *`/`*  
  Merupakan root directory, yang merupakan akar dari seluruh sistem file. Semua direktori lainnya berada di bawahnya.

- **`/bin`**  
  Berisi file eksekusi biner penting yang dibutuhkan untuk sistem berfungsi, seperti perintah dasar (`ls`, `cat`, dll.).

- **`/boot`**  
  Menyimpan file yang dibutuhkan untuk proses booting, seperti kernel Linux dan boot loader.

- **`/dev`**  
  Berisi file perangkat virtual untuk berinteraksi dengan perangkat keras, seperti disk (`/dev/sda`) atau perangkat input.

- **`/etc`**  
  Menyimpan file konfigurasi sistem dan aplikasi, seperti konfigurasi jaringan, daftar pengguna, dll.

- **`/home`**  
  Direktori home untuk setiap pengguna. Setiap pengguna memiliki folder sendiri, seperti `/home/user`.

- **`/lib`**  
  Berisi library (pustaka) sistem yang dibutuhkan oleh program di `/bin` dan `/sbin`.

- **`/media`**  
  Titik mount untuk perangkat penyimpanan eksternal, seperti USB drive atau CD-ROM.

- **`/mnt`**  
  Direktori sementara untuk mounting perangkat penyimpanan manual.

- **`/opt`**  
  Berisi aplikasi tambahan yang diinstal secara manual oleh pengguna.

- **`/proc`**  
  Sistem file virtual yang menyediakan informasi tentang proses dan kernel Linux.

- **`/root`**  
  Direktori home untuk user root (administrator).

- **`/sbin`**  
  Berisi perintah sistem administratif yang biasanya hanya digunakan oleh root.

- **`/tmp`**  
  Direktori untuk file sementara yang dibuat oleh aplikasi. File di sini biasanya dihapus saat sistem reboot.

- **`/usr`**  
  Berisi program, library, dan dokumentasi yang digunakan oleh pengguna. Contohnya: `/usr/bin`, `/usr/lib`.

- **`/var`**  
  Berisi file yang sering berubah, seperti log sistem, cache, dan spool cetakan.


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
+ **`$ cd` (Change Directory)**
  ```bash
  cd folderku
  ```
  {% hint style="info" %}
  Kalian juga dapat menggunakan cara seperti beriku: `cd folder1/folder2/folder3` untuk langsung mengarah ke folder3.
  Atau kalian dapat menggunakan `cd ~` untuk langsung kembali ke /home atau cukup `cd`
  Untuk kembali ke folder diatasnya, kalian dapat menggunakan `cd ..`, dan untuk kembali ke folder sebelumnya,kalian dapat menggunakan `cd -`
  {% endhint %}
+ **`$ ls` (list)**
  ```bash
  ls
  ```
  {% hint style="info" %} 
  Untuk menampilkan lebih banyak detail, kalian dapat menambahkan opsi -l, seperti: `ls -l`. Jika ingin menampilkan file tersembunyi (file yang dimulai dengan titik .), gunakan `ls -a`. Atau kalian gabungkan contoh `ls -la`
  {% endhint %}
+ **`$ mkdir` (make directory)**
  ```bash
  mkdir folderBaru
  ```
  {% hint style="info" %}
  Untuk membuat direktori beserta subdirektori secara otomatis, gunakan `mkdir -p path/to/directory`.
  {% endhint %}
+ **`$ rm` (remove)**
  ```bash
  rm mysecret.txt
  ```
  {% hint style="warning" %} 
  Berhati-hatilah saat menggunakan perintah ini. File yang dihapus tidak dapat dipulihkan kecuali jika menggunakan opsi -i untuk meminta konfirmasi sebelum penghapusan. Gunakan `rm -r` untuk menghapus direktori beserta isinya.
  {% endhint %}
+ **`$ cp` (copy)**
  ```bash
  cp mysecret.txt /home/user/FolderKu/.
  ```
  {% hint style="info" %} 
  Untuk menyalin direktori beserta isinya, gunakan `cp -r folder1 folder2`.
  {% endhint %}
+ **`$ mv` (move)**
  ```bash
  mv mysecret.txt notsecret.txt
  ```
+ **`$ chmod` (change mode)**
  ```bash
  chmod 755 script.sh
  ```
  {% hint style="info" %}
  Opsi 755 memberikan izin baca, tulis, dan eksekusi kepada pemilik file, serta izin baca dan eksekusi kepada grup dan pengguna lain. Gunakan `chmod -R 755 folder/` untuk memberikan izin secara rekursif ke seluruh isi direktori.
  {% endhint %}
+ **`$ chown` (change owner)**
  ```bash
  chown user:user file.txt
  ```