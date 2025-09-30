# Lab2Web
## Nama : Althaf Afif Faiz
## NIM : 312410404
## Kelas : TI.24.A.3

# Praktikum Pemrograman Web #

```
Pertanyaan dan Tugas
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
penjelasannya!
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
penjelasan dan contohnya!
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )
```
## Jawaban dari pertanyaan dan tugas
1. melakukan eksperimen merubah kode css dari modul seperti pada kode program berikut:
 ```
  nav {
  background: #20a759;
  color: #fff;
  padding: 10px;
}
nav a {
  color: #fff;
  text-decoration: none;
  padding: 10px 20px;
}
nav .active,
nav a:hover {
  background: #0b6b3a;
}

#intro {
  background: #418fb1;
  border: 1px solid #099249;
  min-height: 100px;
  padding: 10px;
}
#intro h1 {
  text-align: left;
  border: 0;
  color: #fff;
}
.button {
  padding: 15px 20px;
  color: #fff;
  display: inline-block;
  margin: 10px;
  text-decoration: none;
}
.btn-primary {
  background: #ff0000;
}
.btn-primary {
  background: #ff0000;
}
.btn-primary:hover {
  background: #cc0000;
}
.btn-primary:active {
  background: #949292;
}
.btn-primary:focus {
  outline: none;
  background: rgb(177, 177, 176);
}
.logo {
  position: absolute;
  top: 30px;
  left: 10px;
  width: 50px;
  height: auto;
}
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px 20px;
}
header h1 {
  flex: 1;
  text-align: center;
}
.logo {
  background-color: white;
  border-radius: 8px; /* biar sudutnya agak halus */
  padding: 5px;
}
header {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px 20px;
}
.logo {
  width: 80px;
  height: auto;
  margin-right: 15px;
}
```
Menambahkan class logo untuk dapat ditampilkan pada web dan juga membuat saat tombol di pencet warnanya berubah.

2. Perbedaan h1 {…} dengan #intro h1 {…}   
h1 {…}   
Mengatur semua elemen (h1) di seluruh halaman.   
#intro h1 {…}   
Hanya mengatur (h1) yang ada di dalam elemen dengan id="intro".   

