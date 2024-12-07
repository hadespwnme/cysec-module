# Komponen utama

Sebelumnya kita sudah membahas beberapa komponen utama secara singkat,disini kita akan bahas lebih dalam sedikit beberapa komponen nya.


## Graphical User Interface (GUI) in Windows

Graphical User Interface (GUI) adalah elemen visual yang memungkinkan pengguna berinteraksi dengan sistem operasi Windows melalui klik, drag, dan navigasi yang intuitif. GUI Windows dirancang untuk mempermudah pengguna dalam mengelola aplikasi, file, dan pengaturan tanpa harus menggunakan perintah berbasis teks.


### Komponen Utama GUI Windows

1. **Desktop:**
   - **Deskripsi:** Area kerja utama tempat ikon aplikasi, file, dan folder ditampilkan. 
   - **Fungsi:** Memudahkan akses cepat ke item yang sering digunakan.
   - **Contoh:** Ikon "Recycle Bin" atau file shortcut.

2. **Taskbar:**
   - **Deskripsi:** Bilah horizontal yang biasanya terletak di bagian bawah layar.
   - **Fungsi:**
     - Menampilkan aplikasi yang sedang berjalan.
     - Memberikan akses cepat ke aplikasi yang di-pin.
     - Menampilkan informasi seperti waktu, jaringan, dan notifikasi.
   - **Elemen Penting:**
     - **Start Menu:** Tempat mencari dan meluncurkan aplikasi.
     - **Search Bar:** Untuk mencari file, aplikasi, atau pengaturan.
     - **System Tray:** Menampilkan ikon status, seperti volume dan koneksi internet.

3. **Windows:**
   - **Deskripsi:** Setiap aplikasi atau folder dibuka dalam jendela tersendiri.
   - **Fungsi:**
     - Menyediakan antarmuka kerja untuk aplikasi atau file.
     - Memungkinkan multitasking dengan fitur seperti *Snap Assist*.
   - **Fitur Utama:**
     - **Minimize, Maximize, Close Buttons:** Untuk mengatur tampilan jendela.
     - **Resizable Borders:** Memungkinkan ukuran jendela diubah.

4. **Start Menu:**
   - **Deskripsi:** Menu utama untuk mengakses aplikasi, file, dan pengaturan.
   - **Fungsi:**
     - Memungkinkan pencarian cepat aplikasi atau dokumen.
     - Mengorganisir aplikasi ke dalam kategori untuk akses yang lebih mudah.
   - **Tips:** Gunakan tombol Windows pada keyboard untuk membuka Start Menu dengan cepat.

5. **File Explorer:**
   - **Deskripsi:** Aplikasi GUI untuk mengelola file dan folder di sistem.
   - **Fungsi:**
     - Membuka, memindahkan, menyalin, atau menghapus file.
     - Menavigasi drive lokal, jaringan, atau perangkat eksternal.
   - **Tips:** Gunakan shortcut `Windows + E` untuk membuka File Explorer.

6. **Notifications Center:**
   - **Deskripsi:** Panel di mana notifikasi sistem dan aplikasi ditampilkan.
   - **Fungsi:**
     - Memberikan informasi penting, seperti pembaruan sistem.
     - Memungkinkan akses cepat ke pengaturan seperti mode *Focus Assist*.


### Fitur Kustomisasi GUI

1. **Wallpaper dan Tema:**
   - Ubah tampilan desktop dengan memilih gambar latar belakang (wallpaper) atau tema.

2. **Taskbar Settings:**
   - Sesuaikan ikon yang muncul di taskbar, lokasi taskbar, atau atur ikon yang tersembunyi.

3. **Window Layout:**
   - Gunakan fitur seperti *Snap Layout* untuk mengatur jendela secara efisien dalam mode layar terpisah.


## File System in Windows

File system adalah struktur yang digunakan oleh sistem operasi Windows untuk menyimpan, mengatur, dan mengakses file di perangkat penyimpanan seperti hard drive, SSD, dan perangkat eksternal. Windows mendukung beberapa jenis file system, dengan **NTFS (New Technology File System)** menjadi yang paling umum digunakan.


### Jenis File System yang Didukung Windows

1. **NTFS (New Technology File System):**
   - **Deskripsi:** File system modern yang mendukung fitur seperti keamanan, enkripsi, dan kompresi.
   - **Keunggulan:**
     - Mendukung file besar dan partisi besar.
     - Memiliki fitur journaling untuk mencegah kerusakan data.
     - Mendukung izin file tingkat lanjut.
   - **Penggunaan:** Default pada sistem operasi Windows.

2. **FAT32 (File Allocation Table):**
   - **Deskripsi:** File system yang lebih tua dan sederhana, mendukung kompatibilitas lintas platform.
   - **Keunggulan:**
     - Kompatibel dengan hampir semua perangkat.
     - Cocok untuk perangkat penyimpanan kecil seperti flash drive.
   - **Batasan:**
     - Tidak mendukung file yang lebih besar dari 4 GB.
     - Kurang aman dibandingkan NTFS.

3. **exFAT (Extended File Allocation Table):**
   - **Deskripsi:** Versi modern dari FAT32 yang mendukung file dan partisi besar.
   - **Keunggulan:**
     - Kompatibel dengan banyak perangkat modern.
     - Cocok untuk flash drive dan SD card dengan kapasitas besar.
   - **Penggunaan:** Umumnya digunakan pada perangkat eksternal.



### Struktur Hierarki File System Windows

Windows menggunakan struktur hierarki untuk mengorganisir file dan folder, di mana drive seperti `C:\` adalah akar (root) dari file system. Berikut adalah elemen penting:

1. **Drive Letters:**
   - Setiap perangkat penyimpanan atau partisi diberi huruf, seperti `C:\` untuk drive utama.

2. **Directories (Folder):**
   - Struktur pohon tempat file dan folder lain disimpan. Contoh: `C:\Users\`.

3. **File:**
   - Objek data yang menyimpan informasi, misalnya dokumen, gambar, atau program.

4. **Paths:**
   - Lokasi file atau folder dalam file system.
   - **Contoh Path Absolut:** `C:\Users\Username\Documents\file.txt`.


### Tools dan Command untuk Interaksi dengan File System

Berikut adalah beberapa alat dan perintah penting untuk bekerja dengan file system di Windows:

1. **File Explorer:**
   - GUI utama untuk menjelajahi file dan folder.
   - **Shortcut:** Tekan `Windows + E`.

2. **Command Prompt (cmd):**
   - Perintah untuk berinteraksi dengan file system.
   - Contoh:
     - `dir`: Menampilkan daftar file dalam direktori.
     - `cd`: Berpindah ke direktori tertentu.
     - `del`: Menghapus file.

3. **PowerShell:**
   - Alat yang lebih canggih untuk skrip dan manajemen file.
   - Contoh:
     - `Get-ChildItem`: Menampilkan daftar file seperti `dir`.


### Fitur Penting File System di Windows

1. **Permissions:**
   - Atur akses file berdasarkan pengguna atau grup.
   - Contoh: Membatasi akses file sensitif ke pengguna tertentu.

2. **File Attributes:**
   - Properti seperti **read-only**, **hidden**, dan **system** yang dapat diatur menggunakan GUI atau perintah seperti `attrib`.

3. **Disk Management:**
   - GUI untuk membuat, menghapus, atau memformat partisi disk.
   - **Shortcut:** Tekan `Windows + X` lalu pilih *Disk Management*.


## Windows\System32 Folder

Folder `System32` adalah salah satu direktori paling penting dalam sistem operasi Windows. Lokasinya berada di dalam folder instalasi Windows, biasanya di `C:\Windows\System32`. Folder ini berisi file sistem kritis, pustaka, driver, dan alat penting yang dibutuhkan untuk menjalankan Windows secara normal.

### Isi dan Fungsi Utama Windows\System32

1. **File Eksekusi Penting (Executable Files):**
   - File dengan ekstensi `.exe` yang digunakan untuk menjalankan aplikasi atau alat bawaan Windows.
   - **Contoh:**
     - `cmd.exe`: Command Prompt.
     - `taskmgr.exe`: Task Manager.
     - `explorer.exe`: File Explorer.

2. **Dynamic Link Libraries (DLLs):**
   - File pustaka yang digunakan oleh berbagai aplikasi dan sistem Windows untuk berbagi fungsi.
   - **Contoh:**
     - `kernel32.dll`: Berisi fungsi inti sistem operasi.
     - `user32.dll`: Berisi fungsi untuk pengelolaan GUI.

3. **Device Drivers:**
   - File dengan ekstensi `.sys` yang memungkinkan Windows berkomunikasi dengan perangkat keras.
   - **Contoh:**
     - `disk.sys`: Driver untuk perangkat penyimpanan.
     - `usb.sys`: Driver untuk perangkat USB.

4. **Configuration Files:**
   - File dengan ekstensi `.ini` atau `.cfg` yang menyimpan pengaturan sistem.
   - **Contoh:** `win.ini`.

5. **Built-in Tools dan Utilities:**
   - Alat bawaan Windows untuk pengelolaan sistem.
   - **Contoh:**
     - `chkdsk.exe`: Memeriksa dan memperbaiki disk.
     - `sfc.exe`: Memeriksa dan memperbaiki file sistem.


### Pentingnya Windows\System32 Folder

- **Fungsi Inti Sistem Operasi:**
  Folder ini mendukung fungsi inti Windows. Jika file di dalamnya hilang atau rusak, sistem mungkin tidak dapat berjalan dengan baik.

- **Dependensi Aplikasi:**
  Banyak aplikasi pihak ketiga yang menggunakan pustaka atau alat yang ada di `System32`.

- **Keamanan Sistem:**
  File di folder ini sering menjadi target malware karena pentingnya peran mereka dalam sistem.

{% hint style="warning" %}
### Perhatian Penting

1. **Jangan Menghapus File Secara Sembarangan:**
   Menghapus atau mengubah file di folder ini dapat menyebabkan kerusakan serius pada sistem Windows, termasuk kegagalan untuk boot.

2. **Hati-hati dengan Malware:**
   Beberapa malware menyamar sebagai file di `System32`. Gunakan antivirus yang andal untuk melindungi sistem.

3. **Gunakan Hak Administrator:**
   Untuk mengakses atau memodifikasi file di folder ini, pengguna harus memiliki hak administratif.
{% endhint %}

### Cara Mengakses Folder System32

1. **Melalui File Explorer:**
   - Navigasi ke `C:\Windows\System32`.

2. **Melalui Command Prompt:**
   - Gunakan perintah:
     ```bash
     cd C:\Windows\System32
     ```

3. **Melalui PowerShell:**
   - Gunakan perintah:
     ```powershell
     Set-Location -Path C:\Windows\System32
     ```

## User Accounts, Permissions, and User Account Control in Windows

### 1. User Accounts in Windows

User accounts adalah identitas yang digunakan untuk mengakses komputer Windows. Windows mendukung berbagai jenis akun pengguna dengan tingkat akses berbeda. Akun pengguna membantu mengatur siapa yang dapat mengakses komputer, data, dan aplikasi.

#### Jenis Akun Pengguna:
- **Administrator:**
  - Memiliki kontrol penuh atas sistem.
  - Dapat menginstal aplikasi, mengubah pengaturan, dan mengelola akun pengguna lain.
- **Standard User:**
  - Memiliki akses terbatas.
  - Dapat menggunakan aplikasi dan mengubah pengaturan tertentu, tetapi tidak dapat membuat perubahan besar pada sistem.
- **Guest:**
  - Akun dengan akses paling terbatas.
  - Biasanya digunakan untuk pengguna sementara.
  
#### Cara Mengelola Akun Pengguna:
1. **Melalui Control Panel:**
   - Buka *Control Panel* > *User Accounts* > *Manage Accounts*.
2. **Melalui Settings (Windows 10/11):**
   - Buka *Settings* > *Accounts* > *Family & other users*.


### 2. Permissions in Windows

Permissions adalah aturan yang mengatur akses pengguna ke file, folder, atau aplikasi di Windows. Dengan permissions, sistem dapat melindungi data sensitif dari akses yang tidak sah.

#### Jenis Permissions:
- **Read:** Pengguna dapat melihat isi file atau folder.
- **Write:** Pengguna dapat memodifikasi file atau folder.
- **Execute:** Pengguna dapat menjalankan file atau aplikasi.
- **Full Control:** Pengguna memiliki kontrol penuh, termasuk mengubah izin lainnya.

#### Mengelola Permissions:
1. Klik kanan pada file/folder > Pilih *Properties*.
2. Buka tab *Security* > Klik *Edit* untuk mengubah permissions.
3. Tambahkan atau hapus pengguna, serta atur izin sesuai kebutuhan.


### 3. User Account Control (UAC)

User Account Control (UAC) adalah fitur keamanan Windows yang mencegah perubahan yang tidak sah pada sistem. UAC meminta izin pengguna atau kredensial administrator sebelum mengizinkan perubahan yang memengaruhi sistem.

#### Fungsi UAC:
- Melindungi sistem dari malware.
- Memastikan perubahan besar dilakukan dengan persetujuan pengguna.

#### Tingkat UAC:
1. **Always Notify:**
   - Memberi peringatan setiap kali aplikasi mencoba membuat perubahan atau pengguna mengubah pengaturan sistem.
2. **Notify Me Only When Apps Try to Make Changes:**
   - Default di Windows, memberi peringatan hanya ketika aplikasi mencoba membuat perubahan.
3. **Notify Me Only When Apps Try to Make Changes (No Dim Desktop):**
   - Sama seperti sebelumnya, tetapi desktop tidak dikunci saat pemberitahuan muncul.
4. **Never Notify:**
   - Menonaktifkan UAC (tidak disarankan).

#### Cara Mengatur UAC:
1. Buka *Control Panel* > *User Accounts* > *Change User Account Control settings*.
2. Gunakan slider untuk memilih tingkat UAC yang diinginkan.

---

### Pentingnya User Accounts, Permissions, dan UAC

1. **Keamanan Data:**
   - Membatasi akses ke data sensitif hanya untuk pengguna yang sah.
2. **Mencegah Malware:**
   - Permissions dan UAC membantu mencegah eksekusi malware atau perubahan tidak sah.
3. **Manajemen Sistem:**
   - Dengan akun pengguna yang terpisah, administrator dapat mengelola sistem lebih efisien.

{% hint style="warning" %}
### Tips:
- Gunakan akun administrator hanya untuk tugas yang memerlukan kontrol penuh.
- Selalu aktifkan UAC untuk melindungi sistem dari perubahan yang tidak sah.
- Atur permissions dengan bijak untuk menjaga keamanan data Anda.
{% endhint %}


## Task Manager di Windows
**Task Manager** adalah alat bawaan Windows yang memberikan informasi tentang proses, aplikasi, layanan yang berjalan, dan performa sistem. Alat ini memungkinkan pengguna untuk memantau dan mengelola aplikasi serta memecahkan masalah yang mungkin memengaruhi kinerja komputer.


### Cara Membuka Task Manager

1. **Melalui Kombinasi Tombol:**
   - Tekan `Ctrl + Shift + Esc`.
   - Tekan `Ctrl + Alt + Del`, lalu pilih *Task Manager*.

2. **Melalui Menu Start:**
   - Klik kanan pada *Taskbar* dan pilih *Task Manager*.

3. **Melalui Command Prompt atau Run:**
   - Ketik `taskmgr` di *Command Prompt* atau *Run Dialog Box* (`Win + R`).


### Tampilan dan Fungsionalitas Task Manager

1. **Tab Processes:**
   - Menampilkan daftar aplikasi dan proses yang berjalan.
   - Informasi yang ditampilkan meliputi:
     - **Nama proses**: Nama aplikasi atau layanan yang berjalan.
     - **CPU**: Persentase penggunaan prosesor oleh proses tersebut.
     - **Memory**: Jumlah RAM yang digunakan.
     - **Disk**: Aktivitas disk yang sedang digunakan.
     - **Network**: Aktivitas jaringan (jika ada).

   **Fungsi Utama:**
   - Mengakhiri proses dengan memilih proses dan klik *End Task*.
   - Memantau proses yang menggunakan terlalu banyak sumber daya.

2. **Tab Performance:**
   - Menampilkan performa CPU, RAM, disk, jaringan, dan GPU secara real-time.
   - Informasi penting:
     - Penggunaan CPU dalam persen.
     - Jumlah RAM yang digunakan dan tersedia.
     - Aktivitas disk baca/tulis.
     - Kecepatan jaringan.

3. **Tab App History:**
   - Memberikan informasi tentang penggunaan sumber daya oleh aplikasi dari akun pengguna tertentu.
   - Berguna untuk memantau aplikasi UWP (Universal Windows Platform).

4. **Tab Startup:**
   - Menampilkan aplikasi yang dijalankan saat startup.
   - Memungkinkan pengguna mengaktifkan atau menonaktifkan program startup untuk mempercepat booting.

5. **Tab Users:**
   - Menampilkan aktivitas pengguna aktif.
   - Memantau proses dan sumber daya yang digunakan oleh masing-masing pengguna.

6. **Tab Details:**
   - Menampilkan informasi mendetail tentang semua proses yang berjalan, seperti ID proses (PID) dan prioritas.
   - Berguna untuk pengguna tingkat lanjut atau administrator.

7. **Tab Services:**
   - Menampilkan layanan Windows yang berjalan atau berhenti.
   - Memungkinkan pengguna untuk memulai atau menghentikan layanan tertentu.


### Menggunakan Task Manager untuk Memecahkan Masalah

1. **Mengatasi Program Tidak Merespons:**
   - Pilih program yang tidak merespons di tab *Processes* dan klik *End Task*.

2. **Memantau Sumber Daya:**
   - Identifikasi proses yang menggunakan terlalu banyak CPU, RAM, atau disk.
   - Jika ada proses mencurigakan, lakukan analisis lebih lanjut.

3. **Mengelola Startup:**
   - Nonaktifkan program yang tidak diperlukan di tab *Startup* untuk mempercepat waktu booting.

4. **Melihat Detail Layanan:**
   - Gunakan tab *Services* untuk memulai ulang atau menghentikan layanan penting.


### Tips untuk Menggunakan Task Manager

1. Gunakan tab *Performance* untuk memantau kesehatan sistem secara real-time.
2. Nonaktifkan aplikasi startup yang tidak penting untuk meningkatkan performa.
3. Berhati-hatilah saat mengakhiri proses—proses sistem penting yang dihentikan dapat menyebabkan ketidakstabilan.
4. Gunakan informasi di tab *Details* untuk mendeteksi proses mencurigakan atau malware.