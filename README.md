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
3. Prioritas Internal, Eksternal, dan Inline CSS   
Urutan prioritas CSS (specificity + cascade):   
   1. Inline CSS (langsung di elemen → pakai style="")   
   2. Internal CSS (di <style>)   
   3. Eksternal CSS (file .css)

Contoh :   
```
<h1 style="color: blue;">Halo Dunia</h1>
```     
Jika eksternal CSS: h1 { color: red; }   
Jika internal CSS: h1 { color: green; }   
Hasilnya tetap blue, karena inline CSS menang.   

4. Jika terdapat id dan Class manakah yang ditampilkan pada browser, maka id lebih kuat dibandingkan class.
Contoh :
```
html
<p id="paragraf-1" class="text-paragraf">Teks Contoh</p>
```
```
#paragraf-1 {
  color: blue;
}

.text-paragraf {
  color: red;
}
```

## Menampilkan program yang berbeda dan menjelaskan setiap programnya  

### Code Program HTML :

<img width="998" height="565" alt="Screenshot 2025-10-01 071526" src="https://github.com/user-attachments/assets/a8052ea6-b8cf-4c43-a9d0-a22ff5cd25d7" />

```
<!DOCTYPE html>: Menyatakan bahwa dokumen ini adalah HTML5.   
<html lang="en">: Menandakan bahwa bahasa utama dokumen adalah Inggris.   
<meta charset="UTF-8" />: Mengatur encoding karakter ke UTF-8.   
<meta name="viewport"...>: Membuat tampilan halaman menjadi responsif pada perangkat mobile.   
<title>CSS Dasar</title>: Judul halaman yang akan tampil di tab browser.  
<link rel="stylesheet"...>: Menghubungkan file CSS eksternal.   
```

<img width="379" height="53" alt="image" src="https://github.com/user-attachments/assets/dcd3fa22-51a8-4948-8822-afbfaa5d7c62" />

```
Header Website
Elemen <header> digunakan sebagai bagian kepala halaman.     
<h1> berisi judul besar: "CSS Internal dan Inline CSS".   
Tag <i> digunakan untuk membuat teks italic (miring) pada kata "Inline CSS".
```

<img width="444" height="93" alt="image" src="https://github.com/user-attachments/assets/72cd48a7-87e2-45d4-96e2-bfde0945338e" />

```
Navigasi Website
Tag <nav> adalah container untuk tautan navigasi.
Tiga buah link (<a>) menuju halaman lain:
lab2_css_dasar.html   
lab2_css_eksternal.html   
lab1_tag_dasar.html   
Ini digunakan untuk berpindah antar halaman tutorial.
```

<img width="601" height="191" alt="image" src="https://github.com/user-attachments/assets/0008e879-ca86-4a29-b09b-ef7b7b958f37" />

```
<div id="intro">: Container dengan ID "intro", bisa untuk styling atau navigasi.   
<img> menampilkan gambar dengan nama logo.png.   
alt="Logo": Teks alternatif jika gambar gagal dimuat.   
class="logo": Untuk styling CSS (mungkin didefinisikan di lab2.css).
```
<img width="581" height="23" alt="image" src="https://github.com/user-attachments/assets/a21a0cf4-d35f-48cc-ad67-a397844b1335" />

```
Tautan berbentuk tombol (styling kemungkinan dari class="button btn-primary").   
href="#intro" artinya saat diklik, halaman akan scroll ke bagian dengan id="intro".
```

### Code Program CSS :

<img width="254" height="91" alt="image" src="https://github.com/user-attachments/assets/d37e05d1-97b6-4c83-9f26-e015072c1576" />

```
background: #20a759; → memberi warna latar belakang hijau pada elemen <nav>.     
color: #fff; → warna teks di dalam <nav> menjadi putih.   
padding: 10px; → memberi jarak dalam (spasi) sebesar 10px dari tepi elemen ke konten.
```

<img width="205" height="98" alt="image" src="https://github.com/user-attachments/assets/a620d7ba-b5f5-411f-9184-0f47bc1972b8" />

```
color: #fff; → teks link <a> di dalam <nav> berwarna putih.   
text-decoration: none; → menghilangkan garis bawah pada link.   
padding: 10px 20px; → memberi jarak dalam 10px atas–bawah, 20px kiri–kanan pada link.
```

<img width="205" height="80" alt="image" src="https://github.com/user-attachments/assets/0ff1832e-2f42-4ffe-8a0b-33711282653b" />

```
Selektor ini berlaku untuk link yang sedang aktif (.active) dan ketika pointer mouse diarahkan ke link (a:hover).   
background: #0b6b3a; → memberi warna latar hijau gelap.   
```
<img width="270" height="119" alt="image" src="https://github.com/user-attachments/assets/fb89939c-2775-44d3-bb35-1faf5ebc78a0" />

```
background: #418fb1; → latar belakang biru pada elemen dengan id intro.   
border: 1px solid #099249; → garis tepi 1px, berwarna hijau, model solid.   
min-height: 100px; → tinggi minimal kotak adalah 100px (bisa lebih tinggi jika konten banyak).   
padding: 10px; → jarak dalam 10px.   
```

<img width="155" height="98" alt="image" src="https://github.com/user-attachments/assets/e446e16a-b398-4984-81c0-4f0d8465d6b9" />

```
text-align: left; → teks heading <h1> di dalam #intro rata kiri.   
border: 0; → menghapus garis tepi (jika ada).   
color: #fff; → teks heading putih.   
```

<img width="200" height="132" alt="image" src="https://github.com/user-attachments/assets/bdc2221c-7ee4-4cce-b103-29e35fa61bdb" />

```
padding: 15px 20px; → jarak dalam 15px atas–bawah, 20px kiri–kanan.   
color: #fff; → teks tombol berwarna putih.   
display: inline-block; → membuat elemen tampil seperti inline tapi tetap bisa diberi ukuran, padding, margin.   
margin: 10px; → jarak luar 10px.   
text-decoration: none; → menghilangkan garis bawah pada teks (jika tombol berupa link <a>).
```

<img width="240" height="232" alt="image" src="https://github.com/user-attachments/assets/98fd776f-03b4-438e-92bb-9d685d3d4772" />

```
Elemen dengan class .btn-primary diberi warna latar merah terang (#ff0000).   
Saat mouse diarahkan ke tombol (hover), warna background berubah menjadi merah gelap (#cc0000).   
→ Efek ini memberi feedback interaktif.
Saat tombol ditekan (active), background berubah menjadi abu-abu (#949292).   
→ Menunjukkan tombol sedang diklik.
```

<img width="299" height="80" alt="image" src="https://github.com/user-attachments/assets/c26fa95f-5014-44ba-aee0-63455d2abdfb" />

```
Saat tombol mendapat fokus (misalnya setelah ditekan dengan keyboard), garis outline default dihilangkan.   
Background berubah ke abu-abu muda (rgb(177, 177, 176)).   
→ Memperbaiki tampilan agar konsisten dengan style custom.   
```


<img width="181" height="139" alt="image" src="https://github.com/user-attachments/assets/64f9c9e5-2015-42a4-9844-0a578db1dd7b" />

```
position: absolute; → posisi logo diatur bebas terhadap parent element yang memiliki posisi relatif.   
top: 30px; → jarak logo dari atas 30px.   
left: 10px; → jarak logo dari kiri 10px.    
width: 50px; → lebar logo diatur 50px.     
height: auto; → tinggi menyesuaikan proporsi aslinya (tidak terdistorsi).
```


<img width="285" height="120" alt="image" src="https://github.com/user-attachments/assets/97abd97b-5bd1-40cb-b447-f43fb41d44d0" />

```
display: flex; → membuat konten di dalam <header> menggunakan flexbox.   
align-items: center; → semua item di dalam header rata tengah secara vertikal.   
justify-content: space-between; → item di dalam header ditempatkan dengan jarak merata (yang pertama ke kiri, yang terakhir ke kanan).   
padding: 10px 20px; → memberi jarak dalam 10px atas–bawah, 20px kiri–kanan.   
```


<img width="200" height="79" alt="image" src="https://github.com/user-attachments/assets/6ff03c91-a7f8-482d-82c2-3e8cf3a8193f" />

```
flex: 1; → elemen <h1> di dalam header akan mengambil ruang kosong yang tersedia.   
text-align: center; → teks judul di dalam <h1> rata tengah.    
```

<img width="227" height="97" alt="image" src="https://github.com/user-attachments/assets/86872346-0d3d-4acc-bd6f-e75cbedef253" />

```
background-color: white; → memberi latar belakang putih pada elemen dengan class .logo.   
border-radius: 8px; → membuat sudut kotak menjadi melengkung (rounded) 8px.   
padding: 5px; → memberi jarak dalam sebesar 5px antara isi logo dengan tepi kotak.   
```

<img width="229" height="113" alt="image" src="https://github.com/user-attachments/assets/b82aa629-22c5-48e3-92e0-629599fab6e1" />

```
display: flex; → menjadikan header sebagai flex container.   
align-items: center; → isi di dalam header akan diratakan secara vertikal ke tengah.    
justify-content: center; → isi di dalam header diratakan ke tengah secara horizontal.   
padding: 10px 20px; → memberi jarak dalam 10px atas–bawah dan 20px kiri–kanan.
```

<img width="205" height="104" alt="image" src="https://github.com/user-attachments/assets/4e85d045-13f0-45c7-86d3-3e1904074466" />

```
width: 80px; → logo diberi lebar 80px.   
height: auto; → tinggi logo menyesuaikan proporsi aslinya (tidak terdistorsi).    
margin-right: 15px; → memberi jarak luar ke kanan sebesar 15px, supaya tidak terlalu menempel dengan teks/elemen lain di sampingnya.   
```

### Berikut ini tampilan code program pada HTML :


<img width="1542" height="2192" alt="code html" src="https://github.com/user-attachments/assets/620680e0-e7fa-4eb6-ac04-a00a75505940" />


### Berikut ini tampilan code program pada CSS :


<img width="838" height="3446" alt="code css ril" src="https://github.com/user-attachments/assets/a67bb753-4ca5-4f8b-85a6-52da4bd3e17c" />

### Output dari program dan tampilan pada browser :


<img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/f8d70a34-de70-4872-9709-6719c3fd0deb" />






