# Windows Update

Windows Update adalah fitur bawaan di sistem operasi Windows yang digunakan untuk mengunduh dan menginstal pembaruan perangkat lunak, termasuk patch keamanan, peningkatan fitur, dan driver perangkat keras terbaru. Pembaruan ini penting untuk menjaga keamanan dan kinerja sistem.

![windows update](/.gitbook/assets/windows-update2.png)

## Fungsi Windows Update

1. **Keamanan:**  
   Membantu melindungi komputer dari ancaman terbaru seperti malware, ransomware, dan eksploitasi lainnya dengan menerapkan patch keamanan.

2. **Peningkatan Fitur:**  
   Menambahkan fitur baru atau menyempurnakan fitur yang sudah ada untuk meningkatkan pengalaman pengguna.

3. **Stabilitas Sistem:**  
   Memperbaiki bug atau masalah kompatibilitas yang dapat menyebabkan crash atau kinerja sistem yang tidak optimal.

4. **Driver Terbaru:**  
   Memastikan perangkat keras Anda bekerja dengan versi driver terbaru yang kompatibel dengan sistem operasi.


## Cara Mengakses Windows Update

1. **Melalui Pengaturan:**
   - Tekan `Win + I` untuk membuka **Settings**.
   - Navigasikan ke **Update & Security > Windows Update**.
   - Klik **Check for updates** untuk memeriksa pembaruan terbaru.

2. **Menggunakan Command Prompt atau PowerShell:**
   - Perintah `wuauclt /detectnow` atau `usoclient StartScan` dapat digunakan untuk memulai pemeriksaan pembaruan.


## Jenis Pembaruan

1. **Quality Updates:**  
   Pembaruan bulanan yang mencakup perbaikan bug, peningkatan keamanan, dan stabilitas.

2. **Feature Updates:**  
   Pembaruan besar yang biasanya dirilis dua kali setahun, membawa fitur dan perubahan antarmuka baru.

3. **Driver Updates:**  
   Pembaruan untuk perangkat keras seperti kartu grafis, printer, atau motherboard.

4. **Optional Updates:**  
   Pembaruan tambahan yang tidak diperlukan, seperti pembaruan driver opsional atau fitur minor.


## Tips Menggunakan Windows Update

1. **Periksa Pembaruan Secara Berkala:**  
   Lakukan pemeriksaan manual pembaruan untuk memastikan sistem Anda selalu mendapatkan patch keamanan terbaru.

2. **Atur Jadwal Pembaruan:**  
   Gunakan opsi **Active Hours** untuk mencegah pembaruan mengganggu saat Anda bekerja.

3. **Backup Sebelum Pembaruan Besar:**  
   Sebelum menginstal pembaruan fitur besar, lakukan backup data untuk menghindari kehilangan file jika terjadi masalah.


## Cara Menonaktifkan atau Menunda Pembaruan

1. **Melalui Pengaturan:**
   - Pergi ke **Update & Security > Advanced options**.
   - Atur penundaan pembaruan hingga maksimal 35 hari.

2. **Menggunakan Group Policy Editor (Pro dan Enterprise):**
   - Tekan `Win + R`, ketik `gpedit.msc`, lalu navigasikan ke:
     ```
     Computer Configuration > Administrative Templates > Windows Components > Windows Update
     ```
   - Konfigurasi kebijakan **Configure Automatic Updates**.


## Mengatasi Masalah Windows Update

1. **Gunakan Troubleshooter:**
   - Pergi ke **Settings > Update & Security > Troubleshoot > Windows Update**.
   - Jalankan troubleshooter untuk memperbaiki masalah umum.

2. **Reset Komponen Windows Update:**
   - Jalankan perintah berikut di Command Prompt:
     ```bash
     net stop wuauserv
     net stop bits
     net start wuauserv
     net start bits
     ```

3. **Hapus Cache Pembaruan:**
   - Hapus isi folder `C:\Windows\SoftwareDistribution` untuk membersihkan cache pembaruan yang korup.



# Windows Security

Windows Security adalah fitur bawaan dalam sistem operasi Windows yang dirancang untuk melindungi komputer Anda dari ancaman keamanan seperti malware, virus, ransomware, dan serangan jaringan. Fitur ini menyediakan perlindungan menyeluruh dengan integrasi berbagai alat keamanan yang bekerja secara real-time.

![windows security](/.gitbook/assets/windows-security.png)

## Fitur Utama Windows Security

### 1. **Virus & Threat Protection**
   - Menyediakan perlindungan terhadap malware, spyware, dan virus.
   - Secara otomatis memindai file yang masuk ke sistem dan memberi peringatan jika ada ancaman.
   - Termasuk **Microsoft Defender Antivirus** sebagai solusi antivirus bawaan.

### 2. **Account Protection**
   - Memastikan keamanan akun pengguna, termasuk perlindungan terhadap akses tidak sah.
   - Mendorong penggunaan otentikasi multi-faktor (MFA) dan Windows Hello untuk login yang lebih aman.

### 3. **Firewall & Network Protection**
   - Mengatur dan memantau koneksi jaringan untuk mencegah akses yang tidak sah.
   - Memblokir koneksi berbahaya yang mencoba masuk ke sistem.

### 4. **App & Browser Control**
   - Menyediakan perlindungan terhadap aplikasi berbahaya dan unduhan file dari internet.
   - Menawarkan **Exploit Protection** untuk melindungi sistem dari kerentanan perangkat lunak.

### 5. **Device Security**
   - Melindungi perangkat dengan fitur keamanan berbasis perangkat keras seperti TPM (Trusted Platform Module) dan Secure Boot.
   - Memastikan perangkat aman dari rootkit dan ancaman sistem rendah lainnya.

### 6. **Device Performance & Health**
   - Memberikan laporan tentang kondisi perangkat seperti pembaruan, penyimpanan, driver, dan status baterai.

### 7. **Family Options**
   - Membantu orang tua mengelola aktivitas online anak-anak mereka.
   - Menyediakan kontrol terhadap akses konten dan penggunaan perangkat.


## Mengakses Windows Security

1. Tekan `Win + I` untuk membuka **Settings**.
2. Pilih **Update & Security > Windows Security**.
3. Klik **Open Windows Security** untuk membuka dasbor utama.


## Tips untuk Menggunakan Windows Security

1. **Perbarui Windows Secara Berkala:**
   - Pastikan sistem Anda selalu menggunakan patch keamanan terbaru dari Windows Update.

2. **Aktifkan Real-Time Protection:**
   - Pastikan fitur real-time protection diaktifkan untuk mendeteksi ancaman secara otomatis.

3. **Gunakan Firewall:**
   - Jangan menonaktifkan Windows Firewall kecuali Anda memiliki solusi firewall pihak ketiga yang handal.

4. **Gunakan Proteksi Ransomware:**
   - Aktifkan **Controlled Folder Access** untuk melindungi folder penting dari ransomware.


## Mengatasi Masalah dengan Windows Security

1. **Masalah Antivirus Tidak Berfungsi:**
   - Periksa apakah ada software antivirus pihak ketiga yang bertentangan dengan Windows Security.
   - Nonaktifkan antivirus pihak ketiga untuk mengembalikan kontrol ke Microsoft Defender.

2. **Windows Security Tidak Dapat Dibuka:**
   - Jalankan perintah berikut di Command Prompt:
     ```bash
     sfc /scannow
     ```
     untuk memperbaiki file sistem yang rusak.

3. **Ancaman Tidak Dapat Dihapus:**
   - Jalankan pemindaian offline menggunakan **Microsoft Defender Offline Scan**.


## Keuntungan Menggunakan Windows Security

- **Bebas Biaya:** Tidak memerlukan langganan atau pembelian tambahan.
- **Integrasi Kuat:** Terintegrasi langsung dengan sistem operasi Windows untuk kinerja optimal.
- **Keamanan Real-Time:** Perlindungan otomatis terhadap ancaman yang terus berkembang.


# Virus & Threat Protection

**Virus & Threat Protection** adalah salah satu fitur utama dalam Windows Security yang dirancang untuk melindungi perangkat Anda dari virus, malware, spyware, ransomware, dan berbagai jenis ancaman lainnya. Fitur ini bekerja secara real-time dengan pemindaian otomatis dan manual, memberikan lapisan perlindungan yang kuat untuk menjaga keamanan sistem Anda.

![virus](/.gitbook/assets/windows-security3.png)

## Fitur Utama Virus & Threat Protection

### 1. **Real-Time Protection**
   - Memindai file dan aplikasi yang sedang digunakan untuk mendeteksi ancaman secara langsung.
   - Mengidentifikasi aktivitas mencurigakan sebelum dapat merusak sistem.

### 2. **Quick Scan dan Full Scan**
   - **Quick Scan**: Memindai area penting pada perangkat dengan cepat untuk mendeteksi ancaman.
   - **Full Scan**: Memeriksa seluruh file dan aplikasi di perangkat untuk ancaman yang lebih dalam.

### 3. **Microsoft Defender Antivirus**
   - Antivirus bawaan yang dirancang untuk memberikan perlindungan mendalam terhadap berbagai jenis ancaman.
   - Secara otomatis menerima pembaruan definisi virus melalui Windows Update.

### 4. **Cloud-Delivered Protection**
   - Menggunakan layanan berbasis cloud untuk mengidentifikasi ancaman baru dan memberikan perlindungan yang lebih cepat.

### 5. **Ransomware Protection**
   - Fitur **Controlled Folder Access** melindungi file dan folder penting dari serangan ransomware.
   - Memungkinkan pengguna menentukan folder mana yang ingin dilindungi.

### 6. **History dan Notifications**
   - Menyimpan riwayat pemindaian dan memberikan notifikasi jika ada ancaman yang ditemukan atau diblokir.


## Cara Menggunakan Virus & Threat Protection

### 1. Membuka Virus & Threat Protection:
   1. Tekan `Win + I` untuk membuka **Settings**.
   2. Pilih **Update & Security > Windows Security > Virus & Threat Protection**.

### 2. Melakukan Pemindaian Manual:
   - Di dasbor **Virus & Threat Protection**, klik **Quick Scan** untuk pemindaian cepat.
   - Untuk pemindaian mendalam, pilih **Scan Options > Full Scan**, lalu klik **Scan Now**.

### 3. Mengaktifkan Proteksi Real-Time:
   - Pastikan **Real-Time Protection** aktif di pengaturan **Virus & Threat Protection** untuk perlindungan langsung.

### 4. Menambahkan Folder ke Controlled Folder Access:
   - Klik **Manage Ransomware Protection**.
   - Aktifkan **Controlled Folder Access**.
   - Tambahkan folder penting ke dalam daftar proteksi.


## Tips Mengoptimalkan Virus & Threat Protection

1. **Pastikan Windows Update Selalu Aktif**  
   Virus & Threat Protection bergantung pada definisi virus yang diperbarui secara rutin melalui Windows Update.

2. **Gunakan Full Scan Secara Berkala**  
   Lakukan pemindaian penuh seminggu sekali untuk mendeteksi ancaman tersembunyi.

3. **Jangan Menonaktifkan Real-Time Protection**  
   Jika Anda harus menonaktifkannya sementara, pastikan untuk segera mengaktifkannya kembali.

4. **Gunakan Cloud-Delivered Protection**  
   Aktifkan fitur ini untuk mendeteksi ancaman terbaru yang mungkin belum terdaftar di database lokal.


## Mengatasi Masalah Virus & Threat Protection

1. **Tidak Bisa Membuka Virus & Threat Protection:**
   - Jalankan perintah di Command Prompt:
     ```bash
     sfc /scannow
     ```
   - Restart perangkat untuk memperbaiki file sistem yang rusak.

2. **Ancaman Tidak Dapat Dihapus:**
   - Jalankan pemindaian offline dengan memilih **Microsoft Defender Offline Scan** di opsi pemindaian.


# Firewall & Network Protection

**Firewall & Network Protection** adalah fitur keamanan di Windows yang melindungi perangkat Anda dari ancaman eksternal dengan mengontrol lalu lintas jaringan masuk dan keluar. Fitur ini memblokir koneksi yang tidak sah dan memungkinkan aplikasi dan layanan yang terpercaya untuk berkomunikasi dengan aman.

![firewall](/.gitbook/assets/windows-firewall.png)

## Fitur Utama Firewall & Network Protection

### 1. **Firewall Windows Defender**
   - Firewall bertugas untuk memonitor dan mengontrol lalu lintas jaringan yang masuk dan keluar dari perangkat.
   - Firewall Windows Defender memblokir koneksi yang tidak sah, baik dari internet atau jaringan lokal.
   - Memungkinkan aplikasi atau layanan tertentu untuk mengakses jaringan hanya jika diizinkan oleh pengguna.

### 2. **Network Profile**
   - Windows dapat mengonfigurasi firewall untuk tiga jenis profil jaringan: **Domain**, **Private**, dan **Public**.
     - **Domain Network**: Profil untuk perangkat yang terhubung ke domain perusahaan.
     - **Private Network**: Profil untuk jaringan yang digunakan di rumah atau tempat pribadi.
     - **Public Network**: Profil untuk jaringan publik (misalnya, Wi-Fi umum), dengan keamanan lebih ketat untuk melindungi perangkat dari ancaman luar.

### 3. **Advanced Settings**
   - **Inbound Rules**: Menentukan jenis koneksi yang dapat diterima perangkat Anda dari jaringan luar.
   - **Outbound Rules**: Menentukan jenis koneksi yang diperbolehkan keluar dari perangkat Anda.
   - **Connection Security Rules**: Mengonfigurasi aturan untuk koneksi yang lebih aman antara perangkat Anda dan perangkat lain.

### 4. **Blocking Unauthorized Apps and Services**
   - Windows dapat memblokir aplikasi yang tidak dikenal atau berpotensi berbahaya agar tidak mengakses jaringan tanpa izin.
   - Fitur ini bekerja dengan memverifikasi status aplikasi atau layanan dan membandingkannya dengan database keamanan Windows.


## Cara Mengakses Firewall & Network Protection

### 1. Membuka Firewall & Network Protection:
   1. Tekan `Win + I` untuk membuka **Settings**.
   2. Pilih **Update & Security > Windows Security > Firewall & Network Protection**.

### 2. Mengonfigurasi Firewall:
   - Di dasbor **Firewall & Network Protection**, Anda dapat melihat status firewall untuk berbagai profil jaringan (Domain, Private, Public).
   - Anda dapat memilih **Allow an app through firewall** untuk memberi izin pada aplikasi tertentu untuk mengakses jaringan.

### 3. Menambahkan atau Menghapus Aturan (Advanced Settings):
   - Di menu **Advanced Settings**, Anda dapat membuat **Inbound** atau **Outbound Rules** sesuai kebutuhan untuk aplikasi atau layanan tertentu.

### 4. Menonaktifkan atau Mengaktifkan Firewall:
   - Jika Anda perlu menonaktifkan firewall sementara (misalnya, untuk pemecahan masalah), klik **Turn Windows Defender Firewall on or off**. Namun, pastikan untuk mengaktifkannya kembali setelah selesai.


## Tips Mengoptimalkan Firewall & Network Protection

1. **Selalu Aktifkan Firewall**
   - Pastikan firewall selalu aktif, terutama pada profil **Public** dan **Private** untuk memastikan perlindungan optimal terhadap ancaman luar.

2. **Tinjau Aplikasi yang Diberikan Akses**
   - Sesekali, tinjau aplikasi yang diberi izin untuk mengakses jaringan Anda. Pastikan hanya aplikasi yang tepercaya yang mendapat akses.

3. **Gunakan Mode Public untuk Jaringan Tidak Dikenal**
   - Saat terhubung ke jaringan publik (misalnya, Wi-Fi umum), pastikan perangkat Anda menggunakan profil **Public** untuk membatasi akses ke perangkat Anda.

4. **Aktifkan Advanced Security Rules**
   - Untuk tingkat keamanan yang lebih tinggi, pertimbangkan untuk mengonfigurasi **Connection Security Rules** untuk mengamankan koneksi antar perangkat.


## Cara Memecahkan Masalah Firewall

1. **Firewall Tidak Dapat Dinyalakan:**
   - Jalankan **Windows Security Troubleshooter**: 
     1. Tekan `Win + I` dan pilih **Update & Security > Troubleshoot**.
     2. Pilih **Windows Firewall**, lalu klik **Run the troubleshooter**.

2. **Aplikasi Tidak Dapat Terhubung ke Jaringan:**
   - Pastikan aplikasi telah diizinkan untuk mengakses jaringan. Periksa pengaturan **Allow an app through firewall** di menu **Firewall & Network Protection**.


# App & Browser Control

**App & Browser Control** adalah fitur keamanan di Windows yang membantu melindungi perangkat Anda dari aplikasi yang tidak dikenal, serta ancaman dari web. Fitur ini memungkinkan pengguna untuk mengelola dan mengonfigurasi pengaturan terkait aplikasi, browser, dan perlindungan konten untuk menjaga perangkat tetap aman.

![app](/.gitbook/assets/windows-app-control.png)

## Fitur Utama App and Browser Control

### 1. **Exploit Protection**
   - Exploit Protection melindungi aplikasi dan sistem operasi dari eksploitasi yang memanfaatkan kerentanannya. Fitur ini membantu memblokir teknik-teknik yang digunakan oleh peretas untuk mengeksploitasi bug atau kelemahan dalam aplikasi.
   - Windows 10 dan versi lebih baru secara otomatis mengaktifkan pengaturan perlindungan eksploitasi untuk aplikasi yang sering digunakan seperti browser dan aplikasi email.

### 2. **SmartScreen for Microsoft Edge**
   - **SmartScreen** adalah teknologi perlindungan yang digunakan di browser **Microsoft Edge** dan aplikasi Windows untuk melindungi perangkat Anda dari situs web berbahaya dan aplikasi yang tidak tepercaya.
   - SmartScreen menganalisis situs web dan aplikasi yang Anda coba buka, memberikan peringatan jika situs tersebut teridentifikasi sebagai phishing atau berpotensi berbahaya.

### 3. **SmartScreen for Microsoft Store Apps**
   - Fitur ini bekerja dengan aplikasi yang diunduh melalui **Microsoft Store**. SmartScreen memeriksa aplikasi untuk mendeteksi apakah aplikasi tersebut aman atau berbahaya.
   - Jika ada potensi ancaman atau aplikasi tidak tepercaya, SmartScreen akan memberi peringatan kepada pengguna sebelum mereka melanjutkan untuk menginstalnya.

### 4. **Potentially Unwanted App Blocker (PUA)**
   - PUA adalah aplikasi yang tidak berbahaya, tetapi dapat menyebabkan gangguan, seperti menambah iklan yang tidak diinginkan atau merubah pengaturan default di sistem.
   - Windows memungkinkan Anda untuk mengonfigurasi **PUA Blocker** untuk mencegah penginstalan aplikasi semacam itu.


## Cara Mengakses App and Browser Control

1. **Membuka App and Browser Control:**
   - Tekan `Win + I` untuk membuka **Settings**.
   - Pilih **Update & Security** > **Windows Security** > **App & Browser Control**.

2. **Menonaktifkan atau Mengaktifkan SmartScreen:**
   - Di bawah **Reputation-based protection**, Anda dapat menonaktifkan atau mengaktifkan SmartScreen untuk aplikasi dan browser.
   - Pilih **On** atau **Off** untuk menyesuaikan pengaturan sesuai kebutuhan.

3. **Mengelola Pengaturan Exploit Protection:**
   - Untuk mengonfigurasi perlindungan eksploitasi untuk aplikasi tertentu, pilih **Exploit Protection Settings** dan atur pengaturan sesuai kebutuhan.


## Tips Mengoptimalkan App and Browser Control

1. **Aktifkan SmartScreen untuk Perlindungan Optimal**
   - Untuk meningkatkan keamanan saat menjelajah web, pastikan SmartScreen diaktifkan untuk Microsoft Edge dan aplikasi lainnya. Ini akan melindungi Anda dari situs web berbahaya yang dapat mencuri data atau merusak sistem.

2. **Periksa Aplikasi yang Diunduh dari Sumber Tidak Dikenal**
   - Hindari mengunduh aplikasi dari situs web yang tidak tepercaya. Gunakan **Microsoft Store** untuk mengunduh aplikasi agar lebih aman.

3. **Tinjau dan Atur Pengaturan PUA**
   - Secara rutin tinjau pengaturan **Potentially Unwanted App Blocker** dan pastikan aplikasi yang tidak diinginkan atau berpotensi mengganggu diblokir.

4. **Gunakan Exploit Protection untuk Aplikasi Pihak Ketiga**
   - Jika Anda menggunakan aplikasi pihak ketiga yang sering menjadi sasaran eksploitasi, aktifkan pengaturan **Exploit Protection** untuk aplikasi tersebut di pengaturan **App & Browser Control**.


## Cara Memecahkan Masalah App and Browser Control

1. **SmartScreen Memberikan Peringatan Salah:**
   - Jika SmartScreen memblokir situs atau aplikasi yang seharusnya aman, Anda dapat menonaktifkan sementara fitur ini atau menambahkan situs/aplikasi ke daftar pengecualian. Namun, disarankan untuk hanya melakukannya jika Anda yakin bahwa sumbernya tepercaya.

2. **Aplikasi Tidak Bisa Dibuka Karena Pengaturan SmartScreen:**
   - Pastikan pengaturan **SmartScreen** tidak memblokir aplikasi yang Anda coba buka. Anda bisa menonaktifkan pengaturan atau memilih untuk membuka aplikasi secara manual dengan mengonfirmasi bahwa Anda memahami risikonya.



# Device Security

**Device Security** adalah sekumpulan fitur yang dirancang untuk melindungi perangkat Windows dari ancaman yang dapat merusak perangkat keras dan perangkat lunak. Windows memiliki berbagai teknologi keamanan yang membantu mencegah akses tidak sah ke perangkat dan data yang tersimpan di dalamnya. Device Security bertujuan untuk menjaga keamanan fisik perangkat dan melindungi perangkat dari potensi ancaman berbasis perangkat keras serta perangkat lunak.

![devsec](/.gitbook/assets/windows-device-sec.png)

## Fitur Utama dalam Device Security

### 1. **Secure Boot**
   - **Secure Boot** adalah fitur yang memastikan perangkat hanya menjalankan perangkat lunak yang tepercaya saat booting. Fitur ini mencegah perangkat keras dan perangkat lunak yang tidak sah atau berbahaya (seperti rootkit) untuk dimuat pada saat sistem mulai.
   - Dengan **Secure Boot**, Windows hanya akan memuat sistem operasi yang telah diautentikasi oleh pembuat perangkat (OEM) atau Microsoft, mencegah ancaman yang bisa merusak atau mengambil alih perangkat.

### 2. **BitLocker**
   - **BitLocker** adalah alat enkripsi yang melindungi data di perangkat dengan mengenkripsi seluruh volume penyimpanan. Dengan BitLocker, meskipun perangkat dicuri atau diakses oleh orang yang tidak sah, data yang disimpan akan tetap terlindungi karena hanya bisa dibaca oleh orang yang memiliki kunci enkripsi yang sah.
   - BitLocker bekerja dengan mengenkripsi hard drive atau SSD dan menggunakan kata sandi atau kunci pemulihan untuk membuka akses ke data.

### 3. **Virtualization-Based Security (VBS)**
   - **Virtualization-Based Security (VBS)** menggunakan teknologi virtualisasi perangkat keras untuk melindungi bagian sensitif sistem operasi dari ancaman yang mencoba untuk mengaksesnya. VBS menciptakan lingkungan terisolasi di dalam sistem untuk melindungi memori dan data penting dari malware atau peretas.
   - VBS bekerja bersama dengan fitur-fitur seperti **Device Guard** dan **Credential Guard** untuk menjaga sistem tetap aman dengan mencegah eksekusi kode berbahaya.

### 4. **Windows Defender System Guard**
   - **Windows Defender System Guard** melindungi perangkat dari serangan berbasis kernel yang mencoba untuk memodifikasi atau mengakses memori perangkat. Fitur ini memperkuat perlindungan terhadap perangkat keras dan perangkat lunak dengan cara mendeteksi dan memitigasi eksploitasi kernel.
   - System Guard memanfaatkan teknologi virtualization-based security untuk melindungi berbagai komponen vital sistem.

### 5. **Core Isolation**
   - **Core Isolation** adalah teknologi yang menggunakan isolasi perangkat keras untuk melindungi komponen inti sistem dari serangan berbasis perangkat lunak. Fitur ini melindungi data dan proses yang berjalan di level kernel untuk mencegah kerusakan atau perubahan yang dilakukan oleh malware.
   - Fitur ini juga mencakup **Memory Integrity**, yang memastikan integritas memori yang digunakan oleh sistem operasi, mencegah manipulasi oleh malware atau kode berbahaya.


## Mengakses dan Mengonfigurasi Device Security

1. **Cara Memeriksa Status Device Security:**
   - Tekan `Win + I` untuk membuka **Settings**.
   - Pilih **Update & Security** > **Windows Security** > **Device Security**.
   - Di sini, Anda dapat memeriksa status berbagai fitur keamanan perangkat, seperti Secure Boot, BitLocker, dan Core Isolation.

2. **Mengaktifkan atau Menonaktifkan Fitur Device Security:**
   - Beberapa fitur, seperti BitLocker dan Core Isolation, dapat diaktifkan atau dinonaktifkan melalui pengaturan **Device Security**.
   - Jika perangkat mendukungnya, Anda dapat mengaktifkan **Secure Boot** melalui BIOS/UEFI.

3. **Mengonfigurasi BitLocker:**
   - Untuk mengonfigurasi **BitLocker**, buka **Control Panel** > **BitLocker Drive Encryption**, dan pilih volume yang ingin Anda enkripsi.
   - Anda akan diminta untuk membuat kata sandi dan memilih metode pemulihan untuk membuka akses jika terjadi masalah.


## Tips Mengoptimalkan Device Security

1. **Selalu Gunakan BitLocker untuk Enkripsi Data**
   - Jika Anda menyimpan data sensitif di perangkat, pastikan BitLocker diaktifkan untuk melindunginya. Dengan enkripsi, data Anda akan tetap aman meskipun perangkat dicuri.

2. **Aktifkan Secure Boot**
   - Pastikan **Secure Boot** diaktifkan di BIOS/UEFI untuk melindungi perangkat dari malware yang mencoba menginfeksi sistem operasi saat booting.

3. **Aktifkan Core Isolation dan Memory Integrity**
   - **Core Isolation** dan **Memory Integrity** adalah fitur penting untuk mencegah malware atau peretas mengakses memori sistem. Pastikan fitur ini diaktifkan untuk perlindungan maksimal.

4. **Jaga Firmware dan Driver Selalu Terbaru**
   - Selalu pastikan firmware perangkat keras dan driver Anda selalu diperbarui untuk menghindari potensi kerentanannya yang bisa dimanfaatkan oleh peretas.

5. **Gunakan Teknologi Virtualization-Based Security (VBS)**
   - Jika perangkat Anda mendukungnya, aktifkan **VBS** untuk menambah lapisan perlindungan terhadap eksploitasi berbasis perangkat keras dan perangkat lunak.


## Cara Memecahkan Masalah Device Security

1. **BitLocker Tidak Dapat Diaktifkan:**
   - Jika Anda tidak dapat mengaktifkan BitLocker, pastikan perangkat Anda memiliki TPM (Trusted Platform Module) versi 1.2 atau lebih tinggi, atau gunakan kata sandi untuk mengenkripsi perangkat.

2. **Core Isolation atau Memory Integrity Tidak Dapat Diaktifkan:**
   - Pastikan perangkat Anda memiliki dukungan untuk **Virtualization-Based Security (VBS)**. Anda mungkin perlu mengaktifkan fitur ini melalui BIOS/UEFI.

3. **Secure Boot Tidak Berfungsi:**
   - Jika **Secure Boot** tidak berfungsi, periksa pengaturan BIOS/UEFI dan pastikan fitur ini diaktifkan. Selain itu, pastikan perangkat keras Anda kompatibel dengan **Secure Boot**.

