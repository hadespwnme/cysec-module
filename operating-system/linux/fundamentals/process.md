# Processing 101 in Linux

## Apa itu Processing?

Processing di Linux adalah aktivitas di mana sistem operasi mengelola tugas-tugas atau proses yang sedang berjalan di komputer. Setiap aplikasi atau layanan yang berjalan dianggap sebagai proses. Sistem operasi mengalokasikan sumber daya, seperti CPU dan memori, untuk proses-proses ini agar mereka dapat berjalan dengan lancar.

## Cara Melihat dan Mengelola Proses di Linux

Berikut adalah daftar perintah yang sering digunakan untuk melihat dan mengelola proses di Linux:

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `ps aux`       | Menampilkan semua proses yang sedang berjalan, termasuk pengguna dan sumber daya. |
| `top`          | Menampilkan proses secara real-time dengan informasi seperti penggunaan CPU dan memori. |
| `htop`         | Alternatif interaktif untuk `top` (harus diinstal), memudahkan navigasi proses. |
| `kill -9 <PID>`| Menghentikan proses secara paksa berdasarkan PID.                           |
| `pkill <name>` | Menghentikan semua proses berdasarkan nama aplikasi.                        |
| `jobs`         | Menampilkan proses yang berjalan di background dalam terminal aktif.        |

{% hint style="info" %}
### **Tips**:
- Gunakan `htop` untuk navigasi yang lebih mudah, tekan panah atas/bawah untuk memilih proses, dan `F10` untuk keluar.
- Untuk mengetahui lebih banyak tentang sebuah perintah, gunakan `man <command>` di terminal.
- Berhati-hatilah saat menghentikan proses penting karena dapat memengaruhi stabilitas sistem.
{% endhint %}

## Sinyal Proses (Signals)
- **SIGTERM (15)**: Meminta proses untuk berhenti secara aman. Digunakan secara default oleh `kill`.
- **SIGKILL (9)**: Memaksa proses untuk berhenti segera tanpa menyimpan status. Berguna untuk proses yang tidak merespons.
- **SIGSTOP (19)**: Menangguhkan proses sementara tanpa mengakhiri, sehingga dapat dilanjutkan nanti dengan `kill -CONT`.

## Menjalankan Process saat boot
Beberapa aplikasi atau prosess bisa verjalan ketika prosess boot berlangsung. Sebagai contoh web server, database server atau file transfer server. Software ini penting dan sering kali diminta untuk dijalankan saat sistem di-boot oleh administrator.

Kita bisa gunakan `systemctl` untuk melakukan ini.

```bash
sudo systemctl enable <nama_service>
```

**Contoh:**
```bash
sudo systemctl enable apache2
```

Selain enable,ada 4 opsi juga untuk `systemctl`
+ Start
+ Stop
+ Enable (untuk bootup)
+ Disable (untuk bootup)

Kalian juga bisa menaruh process di background menggunakan shell operator yang kita pelajari sebelumnya `&` atau menggunakan `ctrl + z`, untuk mengembalikannya ke layar, kalian bisa gunakan `fg` (foreground).