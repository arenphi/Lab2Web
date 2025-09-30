# Tugas Pemrograman Web Pertemuan 3
### 1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.

`#intro h1 {
    text-align: center;
    border: 0;
    color: #fff;
}`
![image](ss/4.png)
<p align="center">gambar 1.1 sebelum menambah kode CSS</p>
<br>

![image](ss/4a.png)
<p align="center">gambar 1.2 sesudah menambah kode CSS</p>
<br>

### 2. Apa perbedaan pendeklarasian CSS elemen `h1` `{...}` dengan `#intro` `h1` `{...}`? berikan penjelasannya!
`h1 {...}`
<br>
selector type (tag). Semua elemen `<h1>` di halaman akan mengikuti aturan ini.
![image](ss/4b.png)

`intro h1 {...}`
<br>
selector descendant (spesifik pada `<h1>` yang ada di dalam elemen dengan ID intro). Jadi hanya `<h1>` di dalam `<div id="intro">...</div>` yang terkena.
![image](ss/4c.png)

### 3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!

Jika semua dipakai pada elemen yang sama:

A. Inline CSS → prioritas tertinggi.
   (ditulis langsung di atribut style="" pada elemen HTML).

B. Internal CSS → prioritas di bawah inline (ditulis di <style> di dalam file HTML).

C. Eksternal CSS → prioritas paling rendah (ditulis di file .css yang di-link).

### 4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ( `<p id="paragraf-1"` `class="text-paragraf">` )
