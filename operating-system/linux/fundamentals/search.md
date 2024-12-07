# Searching of Files

Setelah kalian berinterakai dengan file system,kalian akan belajar bagaimana mencari file atau directory yang kalian inginkan tanpa tahu letak tepatnya dimana.

Daripada kalian harus mencari menggunakan `cd` atau `ls`, tidak efisien. kalian bisa gunakan tools yang namanya `find`. Mari kalian bedah.

## Using find

Tools Find ini sangat over power untuk mencari file, kalian hanya perlu memasukan sebaris perintah, dia akan mencarikan apa yang kalian inginkan.

Contoh disini kalian lihat menggunakan `ls`:

![List directory](/.gitbook/assets/find-ls.jpg)

Banyak sekali directory dan kalian tidak tahu dimana file mysecret.txt. Disini kalian gunakan `find` untuk memudahkan kalian mencarinya.

![Find mysecret.txt](/.gitbook/assets/find.jpg)

> **Penjelasan** : 
> - `find` tools find.
> - `.` folder saat ini.
> - `-name` mencari file dengan spesifikasi namanya.
> - `mysecret.txt` nama file yang dicari.

## Using grep

Atau jika kalian ingin mencari kata yang ada didalam sebuah file, atau kalian ingin melihat log system dengan spesifik seperti ip adress tertentu, kalian bisa menggunakan yang namanya `grep`

![grep](/.gitbook/assets/grep.jpg)