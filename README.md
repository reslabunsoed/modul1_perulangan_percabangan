# Modul 1 : Percabangan dan Perulangan 

## 🎯 Tujuan Praktikum
Berikut ini adalah tujuan praktikum pada Modul Praktikum 1:
- Memahami konsep dasar percabangan (if, if-else) dalam pemrograman mikrokontroler.
- Memahami konsep perulangan (while, for) dalam pengendalian perangkat keras.
- Mengimplementasikan logika percabangan dan perulangan untuk mengontrol LED.

## 📄 Dasar Teori

Struktur kontrol sering dipakai dalam pemrograman untuk mengatur fungsi input-output atau memanipulasi data. Terdapat beberapa struktur kontrol yang dipakai dalam pemrograman Arduino yaitu percabangan dan perulangan. Pada kegiatan pembelajaran ini, kita akan mempelajari struktur kontrol percabangan if dan if – else serta perulangan while dan for, dan pemrograman logika. Untuk lebih mempermudah pemahaman digunakan nyala LED sebagai contoh aplikasi sederhana percabangan, perulangan dan logika.

Perintah ```if``` digunakan untuk menyeleksi suatu kondisi tunggal. Bila proses yang diseleksi terpenuhi atau bernilai benar, maka pernyataan yang ada di dalam blok “if” akan diproses dan dikerjakan, dan jika tidak maka program tidak menghasilkan apa-apa. Cara penulisan programnya adalah sebagai berikut:
```
if (kondisi) {
  // aksi
}
```

***Percabangan ```if else```***

Pada dasarnya IF-ELSE merupakan pengembangan dari IF. ELSE berarti kondisi yang tidak sesuai dengan kondisi dalam IF. Dengan kata lain, ELSE artinya “jika tidak”.
```
if (kondisi) {
  // aksi jika benar
} else {
  // aksi jika salah
}
```

Sedangkan perulangan ```for``` digunakan untuk mengulang-ulang kondisi didalam kurung kurawal selama kondisi persyaratan terpenuhi. Biasanya dipakai untuk penambahan atau pengurangan yang berulang-ulang selama kondisi/syarat perulangan terpenuhi.
```
for (inisialisasi kondisi awal; syarat perulangan; penambaan atau pengurangan) {
  // aksi
}
```

***Perulangan ```while```***
Perintah WHILE merupakan perintah untuk melakukan perulangan berdasarkan suatu kondisi, jadi banyaknya perulangan tidak bisa ditentukan dengan pasti. Dalam WHILE seakan ada pengecekan kondisi seperti perintah IF untuk melakukan perulangan.
```
while (kondisi) {
  // aksi
}
```
## 🚀 Tugas Pendahuluan

- Membuat semua program (source code) yang diperlukan untuk masing-masing percobaan (sertakan keterangan-keterangan penting pada source code menggunakan komentar); Jelaskan masing-masing baris atau bagian kode tersebut.
- Menyiapkan rangkaian hardware untuk percobaan (sudah dirangkai, sehingga saat percobaan langsung menjalankan program yang telah dibuat). Sertakan pada tugas pendahuluan dalam bentuk foto yang juga menampilkan wajah Anda. (Dilakukan untuk masing-masing percobaan; Sebelum praktikum, cukup siapkan untuk percobaan pertama saja jika space pada breadboard terbatas)

## ⚙️ Alat dan Bahan

Dalam percobaan sederhana ini, berikut alat dan bahan yang digunakan:

<div align="center">
<table border="1" cellpadding="10" cellspacing="0" width="100%">
  <tr>
    <th>Arduino</th>
    <th>Breadboard</th>
    <th>Resistor</th>
    <th>Jumper</th>
    <th>LED</th>
  </tr>

  <tr align="center">
    <td>
      <img width="192" height="136,1" alt="arduino_uno" src="https://github.com/user-attachments/assets/3e61e208-bb23-42aa-bbef-0ac539279ce0" /><br>
    </td>
    <td>
      <img width="500" height="326" alt="breadboard" src="https://github.com/user-attachments/assets/4c9fc9ea-116c-4bb7-b802-48314049936a" />
    </td>
    <td>
      <img width="224" height="65" alt="Resistor220_Fritzing" src="https://github.com/user-attachments/assets/ba91ea1b-bf55-45c1-acce-085e7308688c" />
    </td>
    <td>
      <img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/1ee4a681-73e4-4ed6-851c-e1bda5911d9c" />
    </td>
    <td>
      <img width="54" height="134" alt="RedLED_Fritzing" src="https://github.com/user-attachments/assets/80556570-c129-43fa-904b-39eac5677a2d" />
    </td>
  </tr>

  <tr align="center">
    <td>Arduino Uno, Leonardo, atau lainnya</td>
    <td>Breadboard Mini</td>
    <td>Resistor</td>
    <td>Jumper Male to Male</td>
    <td>LED Merah</td>
  </tr>
</table>
</div>

## 💻 Percobaan

<h3><a href="Percobaan 1">Percobaan 1A: Percabangan</a></h3>

Percabangan adalah struktur kontrol yang memungkinkan program mengambil keputusan dan memilih jalur eksekusi kode berdasarkan kondisi tertentu, seperti sensor yang bernilai true/false.

Pada percobaan perulangan, praktikan akan mengontrol LED dengan kondisi-kondisi tertentu

Selanjutnya dapat membuka bagian percobaan di [Percobaan 1A: Percabangan](https://github.com/reslabunsoed/modul1_perulangan_percabangan/tree/b182bc3db485fdbe19a6b11fa372b7d29c147894/Percobaan%201)

<h3><a href="Percobaan 2">Percobaan 2A: Perulangan</a></h3>

Perulangan pada Arduino digunakan untuk mengeksekusi blok kode berulang kali, menghemat penulisan kode, dan mengatur aliran program.

Pada percobaan percabangan praktikan akan mengontrol perilaku LED secara dinamis sesuai dengan nilai yang diberikan. 

Selanjutnya dapat membuka bagian percobaan di [Percobaan 2A: Perulangan](https://github.com/reslabunsoed/modul1_perulangan_percabangan/tree/b182bc3db485fdbe19a6b11fa372b7d29c147894/Percobaan%202)

## 📚 Pertanyaan Praktikum

## 🧰 Mengakhiri Percobaan

Berikut hal yang perlu dilakukan setelah selesai praktikum:
- Sebelum keluar dari ruang praktikum, pastikan meja dalam keadaan rapi.
- Jangan lupa untuk mendokumentasikan dalam bentuk foto dan video serta diunggah lewat google drive dan sertakan tautan dokumentasi tersebut di Buku Catatan Praktikum.
- Pastikan asisten telah menandatangani catatan percobaan kali ini pada Buku Catatan Praktikum Anda. Catatan percobaan yang tidak ditandatangani oleh asisten tidak akan dinilai.
- Kumpulkan kode program tugas tambahan pada setiap percobaan dalam repository github dengan format name repository “Kelas(value)_Modul(value)_Nama_NIM”


<h2></h2>

<br>

![banner](https://github.com/user-attachments/assets/f1f03032-41c0-4121-94e3-df1d513b42e5)
