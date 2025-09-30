# Tugas Pemrograman Web Pertemuan 3
### 1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.

![image](ss/4aa.png)
![image](ss/4.png)
<p align="center">gambar 1.1 sebelum menambah kode CSS</p>
<br>

![image](ss/4aaa.png)
![image](ss/4a.png)
<p align="center">gambar 1.2 sesudah menambah kode CSS</p>
<br>

### 2. Apa perbedaan pendeklarasian CSS elemen `h1` `{...}` dengan `#intro` `h1` `{...}`? berikan penjelasannya!
`h1 {...}`, disebut type selector. Berlaku untuk semua tag `<h1>` di seluruh dokumen HTML.

![image](ss/4b.png)

<br>

`intro h1 {...}`, disebut descendant selector, artinya hanya `<h1>` yang berada di dalam elemen dengan ID intro yang kena aturan ini.

![image](ss/4c.png)

Jadi, `<h1>Hello World</h1>` yang ada di dalam `<div id="intro">...</div>` akan berwarna putih, bukan biru.

<br>

### 3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!

Jika semua dipakai pada elemen yang sama: <br>

A. Inline CSS → prioritas tertinggi. <br>
   (ditulis langsung di atribut `style=""` pada elemen HTML).

B. Internal CSS → prioritas di bawah inline <br>
   (ditulis di `<style>` di dalam file HTML).

C. Eksternal CSS → prioritas paling rendah <br>
   (ditulis di file `.css` yang di-link).

![image](ss/4bb.png)
Eksternal (`style_eksternal.css`) misalnya mendefinisikan `h1 { color: blue; }`. <br>
Internal mendefinisikan `h1 { color: green; }`. <br>
Inline mendefinisikan `style="color:red;"`. <br>
<br>
![image](ss/4ba.png)
Hasil di browser = merah, karena inline CSS selalu meng-override yang lain. <br>

<br>

### 4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ( `<p id="paragraf-1"` `class="text-paragraf">` )

![image](ss/4dd.png)
![image](ss/4d.png)
![image](ss/4ddd.png)
Jika elemen memiliki ID dan Class sekaligus, maka ID lebih kuat dibanding class, sehingga gaya CSS dari ID yang akan tampil.
