# Web
* Cek dengan web browser.

* Lihat apa yang ditampilkan.

* Baca seluruh halaman untuk mendapatkan informasi.
  * Mencari nama, email, info pengguna.
  * apakah ada potensi kerentanan di dalamnya? bisa dicek dengan Local File Inclusion (LFI), Remote FIle Inclusion (RFI), Directory Traversal, SQL Injection, Upload Vulnerability.
  
* Lihat menggunakan `robots.txt`.
	- [Where are the robots](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#4-where-are-the-robots)

* Mengganti cookie.
	- [Logon](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#3-logon)
	- [Open to admins](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#6-open-to-admins)
	
* Menggunakan user agent
	- [Picobrowser](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#7-picobrowser)
	
* Lihat source code.
  * Lihatlah hidden values
  * Code yang asing
	- [Insp3ct0r](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#1-inpe3tor)
	- [Dont-use-client-side](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#2-dont-use-client-side)
	- [Client-side-again](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#5-client-side-again)
  * Passwords
  
* Bug web framework
	- [Empire 1](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#11-empire-1)
	- [Empire 2](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#12-empire-2)
	- [Empire 3](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#13-empire-3)

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
	- [Irish-Name-Repo 1](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#8-irish-name-repo-1)
	- [Irish-Name-Repo 2](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#9-irish-name-repo-2)
	- [irish-name-repo-3](https://github.com/ahm4ddm/Writeups-picoCTF2019/blob/master/Web.md#10-irish-name-repo-3)
  * XSS dapat digunakan untuk mendapatkan admin cookie.
  
* Halaman upload
  * Upload shell untuk reverse shell.
  * Bypass file upload filtering
  * Mengganti file (shell.php --> shell.php.png).
  * Jika blacklist bypass, ganti ektensi
    * php --> .php, php3, php4, php5, php6, .inc, pht, phpt, phtml.
    * asp --> .aspx, asp.
    * perl --> .pl, pm, cgi, .lib.
