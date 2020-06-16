# Enumerasi (tahapan mendapatkan informasi)
* Cek dengan web browser.

* Lihat apa yang ditampilkan.

* Baca seluruh halaman untuk mendapatkan informasi.
  * Mencari nama, email, info pengguna.
  * apakah ada potensi kerentanan di dalamnya? bisa dicek dengan Local File Inclusion (LFI), Remote FIle Inclusion (RFI), Directory Traversal, SQL Injection, Upload Vulnerability.
  
* Lihat menggunakan `robots.txt`.

* Lihat source code.
  * Lihatlah hidden values
  * Code yang asing
  * Passwords
  
* Menggunakan web application scanner (Burp suite, Nikto, dll).

* Jika https (menurut saya jarang lomba ctf ada https, kebanyakan pakai ip-address dan port)
  * Scan dengan `heartbleed`.
  * Baca sertikikat web
  
* Menggunakan `curl`

* Mencari directory dan files
  * `dirbuster`
  * `dirb`
  * `nikto`
  
* Halaman login
  * Melihat source code
  * Login menggunakan default password (admin admin, admin  , admin password, dll)
  * Brute force directory (terkadang login tidak dibutuhkan untuk pwn sebuah mesin).
  * Menggunakan `curl`.
  * Menggunakan query SQL Injection. [klik ini untuk menampilkan query SQL Injection](https://github.com/ahm4ddm/Best-Practice-101/blob/master/query%20sql%20injection.txt)
  * XSS dapat digunakan untuk mendapatkan admin cookie.
  
* Halaman upload
  * Upload shell untuk reverse shell.
  * Bypass file upload filtering
  * Mengganti file (shell.php --> shell.php.png).
  * Jika blacklist bypass, ganti ektensi
    * php --> .php, php3, php4, php5, php6, .inc, pht, phpt, phtml.
    * asp --> .aspx, asp.
    * perl --> .pl, pm, cgi, .lib.
