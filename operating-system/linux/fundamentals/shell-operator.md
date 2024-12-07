# Shell Operators

Shell operators adalah simbol atau karakter yang digunakan di dalam terminal Linux untuk mengoperasikan atau menggabungkan perintah-perintah yang ada. Operator ini memudahkan pengguna untuk menjalankan beberapa perintah sekaligus atau mengarahkan output dari perintah ke tempat lain.

Berikut adalah beberapa shell operators yang sering digunakan:

## 1. Operator `>`

Operator `>` digunakan untuk mengalihkan output dari perintah ke file, menggantikan isi file tersebut. Kalau file belum ada, file baru akan dibuat.

### Contoh:
```bash
echo "Hello, World!" > hello.txt
```

Perintah ini akan menulis Hello, World! ke dalam file hello.txt. Jika file hello.txt sudah ada, isinya akan digantikan dengan teks yang baru.

## 2. Operator `>>`

Operator `>>` digunakan untuk menambahkan output dari perintah ke akhir file yang sudah ada, tanpa menggantikan isi file tersebut.

### Contoh:
```bash
echo "Saya text baru" >> hello.txt
```

Perintah ini akan menambahkan `Saya text baru` di akhir file hello.txt. Jika file tersebut belum ada, file baru akan dibuat.

## 3. Operator `&`5
Operator `&` digunakan untuk menjalankan perintah di background, sehingga terminal tetap bisa digunakan untuk perintah lainnya.

### Contoh:
```bash
iniScript &
```

Perintah ini menjalankan `iniScript` di background, dan kalian bisa tetap menjalankan perintah lainnya di terminal tanpa menunggu tugas tersebut selesai.

## 4. Operator `&&`
Operator `&&` digunakan untuk menjalankan perintah kedua hanya jika perintah pertama berhasil dijalankan tanpa error.

### Contoh:
```bash
sudo apt update && sudo apt upgrade -y
```

perintah ini akan menjalankan update system lalu dilanjutkan dengan meng upgrade system.

