# Automation & Package Manager

## Otomatisasi (Automation)

Mungkin adakalanya user ingin menjadwalkan tindakan atau tugas tertentu untuk dilakukan setelah sistem di-boot. Misalnya, menjalankan perintah, mencadangkan file, atau me-launch program favorit nya di Spotify atau Google Chrome. Kita bisa menggunakan yang namanya `crontab`.

Crontab adalah salah satu proses yang dimulai saat boot, yang bertanggung jawab untuk memfasilitasi dan mengelola pekerjaan `cron`. **Crontab hanyalah file khusus dengan format yang dikenali oleh 
_cron_**
proses untuk mengeksekusi setiap baris step by step. Crontab memerlukan 6 nilai khusus:


| Field    | Description                          | Range                          |
|----------|--------------------------------------|--------------------------------|
| `Minute` | Menentukan menit eksekusi tugas.     | 0-59                           |
| `Hour`   | Menentukan jam eksekusi tugas.       | 0-23                           |
| `Day`    | Menentukan hari dalam bulan.         | 1-31                           |
| `Month`  | Menentukan bulan eksekusi tugas.     | 1-12 atau Jan, Feb, Mar, dst.  |
| `Weekday`| Menentukan hari dalam seminggu.      | 0-6 (0 = Minggu) atau Sun-Sat. |

---

### Format Crontab

Setiap baris dalam file crontab mengikuti format berikut:

```bash
* * * * * * <perintah_untuk_dijalankan>
```

### Contoh Penggunaan

1. **Menjalankan tugas setiap hari pada pukul 3:30 pagi:**
   ```bash
   30 3 * * * /path/to/command
   ```
2. **Menjalankan tugas setiap Senin pada pukul 12 siang:**
   ```bash
   0 12 * * 1 /path/to/command
   ```
3. **Menjalankan tugas pada tanggal 1 Januari setiap tahun:**
   ```bash
   0 0 1 1 * /path/to/command
   ```
4. **Menjalankan tugas setiap 5 menit:***
   ```bash
   */5 * * * * /path/to/command
   ```

{% hint style="info %}
**Tips:**
+ Gunakan wildcard (*) untuk menunjukkan semua kemungkinan nilai dalam kolom tertentu.
+ Format seperti */N memungkinkan tugas dijalankan setiap N interval, misalnya */15 untuk setiap 15 menit.
+ Kalian juga bisa generate crontab menggunakan [Crontab Generator](https://crontab-generator.org/) atau [Cron Guru](https://crontab.guru/)
{% endhint %}


## Manager Paket (Package Manager)

Kalau developer ingin mengirimkan tools ke komunitas, **mereka akan mengirimkannya ke repositori**. Jika disetujui, program dan tools mereka akan dirilis ke publik. Dua fitur Linux yang paling bermanfaat terlihat jelas di sini: **Aksesibilitas pengguna dan keunggulan alat sumber terbuka**.

Sementara vendor Sistem Operasi akan mengelola repositori mereka sendiri, kalian juga dapat menambahkan repositori komunitas ke daftar repositori kalian! Ini memungkinkan kalian untuk meningkatkan kemampuan OS kalian. Repositori tambahan dapat ditambahkan dengan menggunakan perintah `add-apt-repository` atau dengan mencantumkan penyedia lain! Misalnya, beberapa vendor akan memiliki repositori yang lebih dekat dengan lokasi geografis mereka. Misal di indonesia ada beberapa repositori seperti **repo UGM**, **Kebo PENS**,dan lain-lain

Berikut adalah beberapa package manager populer yang digunakan di berbagai distro Linux:

| Package Manager | Distribution         | Description                                                                              |
|------------------|----------------------|------------------------------------------------------------------------------------------|
| `apt`           | Debian, Ubuntu       | Advanced Package Tool untuk mengelola paket pada distro berbasis Debian.            |
| `yum`           | CentOS, RHEL         | Yellowdog Updater Modified, digunakan untuk menginstal dan mengelola paket di RHEL/CentOS. |
| `dnf`           | Fedora, CentOS 8+    | Pengganti `yum`, menawarkan peningkatan kecepatan dan fitur untuk distro berbasis RPM. |
| `zypper`        | openSUSE, SLES       | Package manager untuk distro berbasis SUSE, mendukung manajemen repositori.         |
| `pacman`        | Arch Linux           | Simple package manager untuk Arch dan distro turunannya seperti Manjaro.           |
| `rpm`           | RHEL, CentOS, Fedora | Package manager dasar untuk distro berbasis Red Hat, digunakan untuk file `.rpm`.   |
| `emerge`        | Gentoo               | Package manager berbasis source-code yang fleksibel, mendukung kompile dari kode sumber.|
| `snap`          | Ubuntu, Universal    | Universal package manager untuk menginstal aplikasi dalam bentuk container.            |
| `flatpak`       | Universal            | Sistem distro aplikasi universal yang mendukung berbagai distro Linux.          |
| `portage`       | Gentoo               | Sistem manajemen paket untuk Gentoo, berbasis `ebuild` dan sangat dapat disesuaikan.    |

{% hint style="info" %}
## Tips:
- Pastikan sistem kalian menggunakan package manager yang sesuai dengan distro.
- Untuk distro berbasis Debian, gunakan `apt` dengan perintah seperti `sudo apt update` untuk memperbarui indeks paket.
- Gunakan `snap` atau `flatpak` untuk aplikasi yang tidak tersedia di repositori distro kalian.
{% endhint %}

### Menambahkan atau menghapus repositori

Kita biasa yang menggunakan debian based menggunakan `apt` untuk menginstall tools ke sistem operasi kita. 

Salah satu metode untuk menambahkan repositori adalah dengan menggunakan `add-apt-repositoryperintah`. Meskipun kalian dapat menginstal tools melalui penggunaan penginstal paket seperti `dpkg`, manfaat `apt` adalah setiap kali kita memperbarui sistem kita -- repositori yang berisi tools yang kita tambahkan juga akan diperiksa untuk pembaruan.

Saat menambahkan tools, integritas apa yang kita unduh dijamin dengan penggunaan apa yang disebut Kunci GPG(GNU Privacy Guard) . Kunci ini pada dasarnya adalah pemeriksaan keamanan dari developer yang mengatakan, "ini lho tools buatan kami". Jika kunci tidak sesuai dengan apa yang dipercayai sistem Anda dan apa yang digunakan pengembang, maka tools tidak akan diunduh.