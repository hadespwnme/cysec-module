Sekarang kita akan memasuki lebih dalam lagi tentang windows.

# Windows System Configuration

**System Configuration**, atau lebih dikenal sebagai *msconfig*, adalah alat bawaan Windows yang memungkinkan pengguna untuk mengelola berbagai aspek startup dan konfigurasi sistem. Alat ini sering digunakan untuk mendiagnosis dan memecahkan masalah pada sistem operasi, seperti masalah booting atau layanan yang tidak diperlukan.


## Cara Membuka System Configuration

1. **Melalui Kotak Dialog Run**:
   - Tekan `Win + R`, ketik `msconfig`, lalu tekan `Enter`.

2. **Melalui Search Bar**:
   - Ketik *System Configuration* di kotak pencarian menu Start dan pilih aplikasinya.


## Tab di System Configuration

### 1. **General**
   - Memberikan kontrol dasar atas cara Windows memulai.
   - **Pilihan Startup:**
     - **Normal Startup**: Memuat semua driver perangkat dan layanan.
     - **Diagnostic Startup**: Memuat hanya layanan dan driver dasar—berguna untuk memecahkan masalah.
     - **Selective Startup**: Memungkinkan pengguna memilih layanan atau item startup tertentu untuk dimuat.

### 2. **Boot**
   - Berisi pengaturan yang terkait dengan proses booting Windows.
   - **Pilihan Utama:**
     - **Safe Boot**: Mem-boot sistem dalam mode aman.
       - Minimal: Memuat layanan dan driver dasar.
       - Alternate Shell: Mem-boot ke mode aman dengan akses Command Prompt.
     - **Boot Log**: Membuat log proses booting.
     - **Base Video**: Mem-boot dengan driver video dasar.
     - **Timeout**: Mengatur waktu menunggu untuk memilih OS (jika ada beberapa OS).
   - Pengguna juga dapat mengatur OS default jika menggunakan sistem dual-boot.

### 3. **Services**
   - Menampilkan daftar layanan Windows yang berjalan atau dapat dijalankan saat startup.
   - **Fungsi:**
     - Centang atau hapus centang layanan untuk diaktifkan atau dinonaktifkan.
     - Opsi *Hide all Microsoft services* memungkinkan pengguna hanya melihat layanan pihak ketiga untuk mempermudah pengelolaan.

### 4. **Startup**
   - Pada Windows versi sebelumnya, tab ini digunakan untuk mengelola aplikasi startup. 
   - **Catatan**: Pada Windows 8 dan yang lebih baru, pengelolaan startup dialihkan ke **Task Manager**.

### 5. **Tools**
   - Berisi daftar pintasan ke alat administrasi Windows lainnya, seperti:
     - Command Prompt
     - Registry Editor
     - Event Viewer
   - Memudahkan akses ke alat diagnostik dan administrasi tanpa harus mencarinya secara manual.


## Menggunakan System Configuration

### Memperbaiki Masalah Startup
- Pilih **Diagnostic Startup** untuk memuat hanya layanan dan driver dasar, memudahkan diagnosis masalah.

### Mengelola Layanan
- Nonaktifkan layanan yang tidak penting di tab *Services* untuk meningkatkan performa sistem.
- Hati-hati saat menonaktifkan layanan sistem agar tidak menyebabkan ketidakstabilan.

### Mengakses Safe Mode
- Aktifkan opsi **Safe Boot** di tab *Boot* untuk mem-boot sistem ke mode aman tanpa perlu menekan tombol selama startup.

### Dual-Boot Management
- Jika memiliki beberapa sistem operasi, atur OS default dan waktu timeout di tab *Boot*.


## Tips Menggunakan System Configuration

1. **Cadangkan Konfigurasi**: Sebelum membuat perubahan, catat atau cadangkan konfigurasi saat ini untuk menghindari masalah yang tidak diinginkan.
2. **Hati-Hati dengan Layanan**: Jangan menonaktifkan layanan tanpa memahami fungsinya, terutama layanan Microsoft.
3. **Gunakan Safe Boot untuk Diagnosis**: Mode aman adalah cara terbaik untuk memulai sistem dengan hanya layanan dan driver penting.
4. **Periksa Startup di Task Manager**: Untuk versi Windows terbaru, kelola aplikasi startup langsung di Task Manager.


# Computer Management

**Computer Management** adalah alat bawaan Windows yang berfungsi sebagai pusat administrasi untuk mengelola berbagai aspek sistem komputer. Alat ini menggabungkan beberapa utilitas penting dalam satu antarmuka, sehingga memudahkan pengguna dan administrator untuk memantau dan mengelola sistem.


## Cara Membuka Computer Management

1. **Melalui Kotak Dialog Run**:
   - Tekan `Win + R`, ketik `compmgmt.msc`, lalu tekan `Enter`.

2. **Melalui Menu Start**:
   - Ketik *Computer Management* di kotak pencarian menu Start dan pilih aplikasinya.

3. **Klik Kanan pada "This PC" atau "My Computer"**:
   - Pilih **Manage** untuk langsung membuka Computer Management.


## Komponen Utama dalam Computer Management

### 1. **System Tools**
   Alat-alat untuk memantau dan mengelola konfigurasi sistem.
   - **Event Viewer**:
     - Digunakan untuk melihat log peristiwa sistem, seperti kesalahan, peringatan, atau informasi lain yang dicatat oleh Windows dan aplikasi.
   - **Task Scheduler**:
     - Membuat atau mengelola tugas terjadwal untuk menjalankan aplikasi atau perintah tertentu pada waktu tertentu.
   - **Device Manager**:
     - Menampilkan semua perangkat keras yang terhubung ke komputer. Pengguna dapat mengelola driver perangkat, mengaktifkan/menonaktifkan perangkat, atau memecahkan masalah perangkat.
   - **Shared Folders**:
     - Menampilkan daftar folder yang dibagikan melalui jaringan, sesi aktif, dan file yang dibuka oleh pengguna jaringan.


### 2. **Storage**
   Alat untuk mengelola perangkat penyimpanan.
   - **Disk Management**:
     - Mengelola partisi dan drive sistem.
     - Fungsi meliputi membuat, menghapus, memperluas, atau mengecilkan partisi, serta mengubah drive letter.
   - **Removable Storage** (Versi lama):
     - Mengelola perangkat penyimpanan yang dapat dilepas, seperti CD/DVD atau USB.


### 3. **Services and Applications**
   Alat untuk mengelola layanan dan aplikasi yang berjalan di sistem.
   - **Services**:
     - Menampilkan semua layanan Windows yang tersedia. Pengguna dapat memulai, menghentikan, atau mengubah pengaturan layanan.
   - **WMI Control (Windows Management Instrumentation)**:
     - Mengelola pengaturan WMI yang digunakan untuk memantau dan mengontrol sistem melalui skrip atau aplikasi.


## Manfaat Computer Management

1. **Pemantauan Sistem**:
   - Dengan *Event Viewer*, pengguna dapat dengan cepat menemukan kesalahan sistem atau aplikasi dan mencoba memperbaikinya.

2. **Manajemen Perangkat Keras**:
   - *Device Manager* memungkinkan pengguna untuk memperbarui atau memecahkan masalah perangkat keras dengan mudah.

3. **Pengelolaan Penyimpanan**:
   - *Disk Management* menyediakan antarmuka grafis yang intuitif untuk membuat atau mengelola partisi tanpa memerlukan alat pihak ketiga.

4. **Konfigurasi Layanan**:
   - Dengan *Services*, pengguna dapat memastikan layanan yang tidak diperlukan tidak berjalan, sehingga meningkatkan kinerja sistem.

5. **Manajemen Jaringan**:
   - Melalui *Shared Folders*, pengguna dapat memantau dan mengelola folder yang dibagikan untuk keamanan jaringan.


## Tips Penggunaan Computer Management

1. **Selalu Cadangkan Data**:
   - Sebelum melakukan perubahan pada partisi atau layanan sistem, pastikan untuk mencadangkan data penting.

2. **Gunakan dengan Hak Administrator**:
   - Beberapa fitur, seperti *Disk Management* atau *Services*, memerlukan izin administrator untuk digunakan.

3. **Periksa Event Viewer Secara Rutin**:
   - Log di *Event Viewer* dapat membantu mengidentifikasi masalah yang tidak terlihat secara langsung, seperti kesalahan perangkat keras atau masalah jaringan.


# System Information

**System Information** adalah alat bawaan Windows yang menampilkan informasi terperinci tentang perangkat keras, perangkat lunak, dan konfigurasi sistem komputer kalian. Alat ini sangat berguna untuk memecahkan masalah atau menganalisis konfigurasi sistem.


## Fitur Utama System Information

1. **Informasi Sistem Umum**  
   Menampilkan detail perangkat keras, seperti nama sistem, model, versi BIOS, jenis prosesor, dan total memori.

2. **Komponen**  
   Memberikan informasi mendetail tentang perangkat keras seperti perangkat input, kartu jaringan, perangkat audio, dan lainnya.

3. **Lingkungan Perangkat Lunak**  
   Menyediakan data tentang proses yang sedang berjalan, driver sistem, variabel lingkungan, dan program startup.


## Cara Membuka System Information

1. **Melalui Kotak Dialog Run**:  
   - Tekan `Win + R`, ketik `msinfo32`, lalu tekan `Enter`.

2. **Melalui Menu Start**:  
   - Ketik *System Information* pada kotak pencarian menu Start dan pilih hasilnya.

3. **Melalui Command Prompt atau PowerShell**:  
   - Jalankan perintah berikut:
     ```bash
     msinfo32
     ```



## Bagian-Bagian dalam System Information

### 1. **System Summary**  
   Menampilkan informasi utama perangkat, seperti:
   - Nama komputer
   - Versi sistem operasi
   - Jenis prosesor
   - Versi firmware (BIOS/UEFI)
   - Kapasitas RAM

### 2. **Hardware Resources**  
   Menampilkan informasi detail perangkat keras, termasuk:
   - Penggunaan IRQ (Interrupt Request)
   - Konflik perangkat keras
   - Alokasi memori

### 3. **Components**  
   Menyediakan informasi tentang perangkat keras seperti:
   - Tampilan (display)
   - Jaringan
   - Penyimpanan (drive, disk)
   - Perangkat input/output

### 4. **Software Environment**  
   Menampilkan data perangkat lunak seperti:
   - Layanan yang berjalan
   - Driver sistem
   - Program startup
   - Variabel lingkungan


## Kegunaan System Information

- **Pemecahan Masalah Perangkat Keras**:  
  Memeriksa apakah perangkat keras dikenali dengan benar oleh sistem.

- **Analisis Kinerja Sistem**:  
  Melihat konfigurasi perangkat keras dan perangkat lunak untuk mengidentifikasi bottleneck.

- **Audit Sistem**:  
  Membantu mengumpulkan data lengkap tentang perangkat keras dan perangkat lunak untuk kebutuhan audit atau dokumentasi.

- **Pemeriksaan Kompatibilitas**:  
  Memastikan spesifikasi sistem memenuhi kebutuhan perangkat lunak atau pembaruan tertentu.


{% hint style="info" %}
## Tips Penggunaan
- **Ekspor Informasi ke File**:  
  kalian dapat menyimpan laporan System Information ke file dengan memilih menu **File > Export** untuk kebutuhan dokumentasi atau berbagi dengan tim teknis.

- **Gunakan Pencarian**:  
  Gunakan fitur pencarian dengan menekan `Ctrl + F` untuk menemukan informasi tertentu lebih cepat.

- **Akses Cepat Detail Spesifik**:  
  Jika kalian hanya memerlukan detail spesifik seperti model prosesor atau jumlah RAM, langsung buka bagian *System Summary*.
{% endhint%}


# Resource Monitor

**Resource Monitor** adalah alat bawaan Windows yang memungkinkan pengguna untuk memantau penggunaan sumber daya sistem secara real-time. Alat ini memberikan data mendetail tentang kinerja CPU, memori, disk, dan jaringan, yang sangat berguna untuk menganalisis masalah kinerja atau mengidentifikasi proses yang menghabiskan banyak sumber daya.

![resmon](./gitbook/assets/resmon.png)

## Fitur Utama Resource Monitor

1. **CPU (Central Processing Unit)**  
   - Menampilkan daftar proses yang sedang berjalan, termasuk konsumsi CPU mereka.  
   - Informasi tentang *handles* dan *threads* yang digunakan oleh setiap proses.  

2. **Memory (RAM)**  
   - Menunjukkan total memori yang digunakan, memori bebas, dan memori cadangan.  
   - Memberikan detail tentang proses yang menggunakan memori dan alokasi halaman memori.  

3. **Disk**  
   - Memantau aktivitas disk, termasuk kecepatan baca/tulis.  
   - Melihat proses mana yang sedang membaca atau menulis data pada disk tertentu.  

4. **Network**  
   - Memberikan data tentang koneksi jaringan aktif.  
   - Menampilkan informasi tentang aplikasi atau proses yang menggunakan jaringan.  


## Cara Membuka Resource Monitor

1. **Melalui Task Manager**:  
   - Buka *Task Manager* (`Ctrl + Shift + Esc`), lalu pilih tab **Performance**, dan klik **Open Resource Monitor**.

2. **Melalui Kotak Dialog Run**:  
   - Tekan `Win + R`, ketik `resmon`, lalu tekan `Enter`.

3. **Melalui Menu Start**:  
   - Cari *Resource Monitor* pada kotak pencarian menu Start dan pilih hasilnya.


## Bagian-Bagian dalam Resource Monitor

### 1. **Overview**  
   Menampilkan ringkasan dari keempat komponen utama (CPU, Memory, Disk, Network) dalam satu layar.

### 2. **CPU**  
   - Memantau penggunaan CPU oleh proses tertentu.  
   - Melihat *handles* dan *threads* aktif.

### 3. **Memory**  
   - Melacak konsumsi RAM oleh proses aktif.  
   - Melihat alokasi halaman memori (*paging*) dan penggunaan memori virtual.

### 4. **Disk**  
   - Melihat aktivitas baca/tulis pada disk.  
   - Menganalisis file yang diakses oleh proses tertentu.

### 5. **Network**  
   - Memantau aktivitas jaringan, termasuk koneksi TCP dan port terbuka.  
   - Menampilkan aplikasi yang menggunakan bandwidth.


## Kegunaan Resource Monitor

- **Identifikasi Proses Konsumsi Tinggi**  
  Menemukan aplikasi atau proses yang menggunakan terlalu banyak CPU, memori, atau disk.

- **Analisis Koneksi Jaringan**  
  Mengidentifikasi aplikasi yang menyebabkan lalu lintas jaringan tinggi.

- **Pemecahan Masalah Kinerja**  
  Menganalisis proses yang menyebabkan kinerja sistem lambat atau tidak responsif.

- **Monitoring Aktivitas Disk**  
  Melihat file atau proses yang menyebabkan beban berat pada disk.


## Tips Menggunakan Resource Monitor

- **Filter Berdasarkan Proses**  
  Klik kanan pada proses tertentu untuk memfilter aktivitas CPU, disk, memori, atau jaringan yang hanya terkait dengan proses tersebut.

- **Analisis Koneksi Jaringan**  
  Gunakan tab *Network* untuk memeriksa port atau IP address yang mencurigakan.

- **Cegah Overload Sistem**  
  Identifikasi dan hentikan proses yang menghabiskan sumber daya secara berlebihan langsung dari tab Resource Monitor.


# Command Prompt

**Command Prompt (CMD)** adalah antarmuka berbasis teks bawaan Windows yang memungkinkan pengguna menjalankan perintah untuk mengelola file, menjalankan aplikasi, atau mengkonfigurasi sistem. CMD sangat berguna untuk tugas administratif, skrip otomatisasi, dan memecahkan masalah sistem.

![cmd](/.gitbook/assets/ipconfig.png)

## Fitur Utama Command Prompt

1. **Manajemen File dan Direktori**  
   - Membuat, menghapus, menyalin, atau memindahkan file dan folder.

2. **Manajemen Sistem**  
   - Melihat informasi sistem, memeriksa koneksi jaringan, atau mengkonfigurasi pengaturan sistem.

3. **Automasi Tugas**  
   - Menjalankan skrip batch untuk mengotomatisasi proses tertentu.

4. **Diagnostik dan Pemecahan Masalah**  
   - Mengecek koneksi jaringan, memverifikasi file sistem, atau membersihkan cache.


## Cara Membuka Command Prompt

1. **Melalui Menu Start**  
   - Cari *Command Prompt* di kotak pencarian menu Start dan pilih hasilnya.

2. **Melalui Kotak Dialog Run**  
   - Tekan `Win + R`, ketik `cmd`, lalu tekan `Enter`.

3. **Sebagai Administrator**  
   - Klik kanan pada *Command Prompt* dan pilih **Run as administrator** untuk akses penuh ke sistem.


## Beberapa Perintah Dasar di Command Prompt

| Command               | Description                                               |
|-----------------------|-----------------------------------------------------------|
| `dir`                | Menampilkan daftar file dan folder dalam direktori aktif. |
| `cd`                 | Mengubah direktori aktif.                                 |
| `copy`               | Menyalin file ke lokasi lain.                             |
| `move`               | Memindahkan file ke lokasi lain.                          |
| `del`                | Menghapus file tertentu.                                  |
| `mkdir` atau `md`    | Membuat folder/direktori baru.                            |
| `rmdir` atau `rd`    | Menghapus folder/direktori kosong.                        |
| `ipconfig`           | Menampilkan konfigurasi jaringan.                        |
| `ping`               | Mengecek koneksi ke alamat IP tertentu.                  |
| `cls`                | Membersihkan layar Command Prompt.                       |


{% hint style="info" %}
## Tips Menggunakan Command Prompt

1. **Gunakan Tab untuk Auto-Complete**  
   Saat mengetik nama file atau folder, tekan `Tab` untuk melengkapi nama secara otomatis.

2. **Periksa Bantuan Perintah**  
   Tambahkan `/help` setelah perintah untuk melihat cara penggunaannya. Contoh:
   ```bash
   dir /help
   ```
   atau kalian bisa gunakan `/?`
{% endhint %}


# Windows Registry

Windows Registry adalah database hierarki yang digunakan oleh sistem operasi Windows untuk menyimpan pengaturan sistem, informasi konfigurasi perangkat keras, aplikasi, dan akun pengguna. Registry memegang peranan penting dalam menjaga stabilitas dan performa sistem.

![regedit](/.gitbook/assets/regedit.png)

## Struktur Registry

Registry terdiri dari lima root keys utama, masing-masing dengan fungsi tertentu:

1. **HKEY_CLASSES_ROOT (HKCR)**  
   Menyimpan informasi tentang file type associations, seperti aplikasi default untuk membuka file berdasarkan ekstensi.

2. **HKEY_CURRENT_USER (HKCU)**  
   Menyimpan pengaturan konfigurasi pengguna yang sedang aktif, termasuk preferensi desktop, printer, dan pengaturan aplikasi.

3. **HKEY_LOCAL_MACHINE (HKLM)**  
   Menyimpan pengaturan dan konfigurasi perangkat keras serta perangkat lunak yang berlaku untuk seluruh pengguna sistem.

4. **HKEY_USERS (HKU)**  
   Menyimpan informasi tentang semua pengguna yang pernah login ke komputer.

5. **HKEY_CURRENT_CONFIG (HKCC)**  
   Menyimpan informasi tentang konfigurasi perangkat keras yang sedang digunakan, seperti driver aktif.


## Fungsi Windows Registry

- **Menyimpan Pengaturan Sistem:**  
  Registry digunakan oleh sistem untuk menyimpan informasi seperti pengaturan jaringan, driver, dan konfigurasi perangkat keras.

- **Konfigurasi Aplikasi:**  
  Aplikasi menggunakan registry untuk menyimpan preferensi pengguna dan pengaturan aplikasi.

- **Memecahkan Masalah Sistem:**  
  Administrator sering memodifikasi registry untuk memperbaiki kesalahan sistem atau mengubah pengaturan tersembunyi.


## Cara Mengakses Registry

1. **Membuka Registry Editor:**
   - Tekan `Win + R`, ketik `regedit`, dan tekan `Enter`.

2. **Menavigasi Registry:**
   - Gunakan tampilan hierarki untuk menjelajahi root keys dan subkeys.

3. **Membuat atau Menghapus Key:**
   - Klik kanan pada key yang diinginkan, lalu pilih **New** untuk membuat key baru atau **Delete** untuk menghapus.


## Tips Bekerja dengan Registry

1. **Selalu Backup Registry:**  
   Sebelum melakukan perubahan, pastikan untuk membuat cadangan registry:
   - Di Registry Editor, pilih **File > Export**, lalu simpan file cadangan.

2. **Gunakan Search:**  
   Gunakan fitur **Find** (`Ctrl + F`) untuk mencari key atau value tertentu.

3. **Hati-Hati dengan Perubahan:**  
   Kesalahan dalam memodifikasi registry dapat menyebabkan sistem menjadi tidak stabil atau bahkan gagal booting.


## Contoh Modifikasi Registry

### 1. Mengubah Nama Registered Owner
1. Buka Registry Editor.
2. Navigasikan ke: `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion`
3. Temukan key `RegisteredOwner` dan ubah nilainya.

### 2. Mengatur Startup Delay
1. Navigasikan ke: `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\Serialize`
2. Tambahkan key DWORD baru dengan nama `StartupDelayInMSec` dan setel nilainya ke `0` untuk menonaktifkan delay.


## Perintah CMD untuk Registry

| Command                           | Description                                  |
|-----------------------------------|----------------------------------------------|
| `reg query <key>`                 | Melihat informasi di registry tertentu.     |
| `reg add <key>`                   | Menambahkan key atau value baru.            |
| `reg delete <key>`                | Menghapus key atau value tertentu.          |
| `reg export <file.reg>`           | Mengekspor registry ke file cadangan.       |
| `reg import <file.reg>`           | Mengimpor registry dari file cadangan.      |

Contoh penggunaan:
```bash
reg query HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft
```
