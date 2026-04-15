# Percobaan 2: Perulangan

## 🎯 Tujuan
Fokus percobaan adalah memahami penggunaan perulangan (for) untuk mengontrol LED berdasarkan kondisi tertentu.

## 💡 Spesifikasi yang Diharapkan
1)	Kongfigurasi pin sesuai dengan petunjuk praktikum pada bagian langkah percobaan
2)	LED menyala secara berurutan dari kiri ke kanan 
3)	Setelah LED terakhir, arah berubah ke kanan ke kiri 
4)	Pola berjalan terus menerus tanpa error 
5)	Tidak ada LED yang mati atau tidak sesuai urutan

## ♻️ Langkah Percobaan
1. Persiapkan alat dan bahan

- Lakukan seperti halnya tugas pendahuluan poin 1
- Pastikan Arduino Uno terhubung dengan komputer

2. Program percobaan

```cpp
int timer = 100;           // delay. Semakin tinggi angkanya, semakin lambat waktunya.
void setup() {
  // gunakan loop for untuk menginisialisasi setiap pin sebagai output:
  for (int ledPin = 2; ledPin < 8; ledPin++) {
    pinMode(ledPin, OUTPUT);
  }
}
void loop() {
  // looping dari pin rendah ke tinggi
  for (int ledPin = 2; ledPin < 8; ledPin++) {
    // hidupkan LED pin nya:
    digitalWrite(ledPin, HIGH);
    delay(timer);
    // matikan pin LED nya:
    digitalWrite(ledPin, LOW);
  }
  // looping dari pin yang tinggi ke yang rendah
  for (int ledPin = 7; ledPin >= 2; ledPin--) {
    // menghidupkan pin:
    digitalWrite(ledPin, HIGH);
    delay(timer);
    // mematikan pin:
    digitalWrite(ledPin, LOW);
  }
}
```
4. Simpan sketch dengan nama file modul1_perulangan
5. Konfigurasi Rangkaian

<img width="940" height="387" alt="image" src="https://github.com/user-attachments/assets/c303009e-7c48-41f4-932b-201f1b7d151e" />

Membuat rangkaian yang menghubungkan 5 buah LED dengan Pin digital menggunakan breadboard sesuai pada Gambar dengan konfigurasi pin sesuai pada Tabel berikut

| No | Komponen | Pin   |
|:--:|:---------|:-----:|
| 1  | LED 1    | Pin 2 |
| 2  | LED 2    | Pin 3 |
| 3  | LED 3    | Pin 4 |
| 4  | LED 4    | Pin 5 |
| 5  | LED 5    | Pin 6 |
| 6  | LED 6    | Pin 7 |
| 7  | GND      | GND   |

7. Berikutnya compile dan upload program ke dalam Arduino board. Perhatikan dan berikan analisi pada hasil yang terjadi, apakah sesuai dengan spesifikasi atau tidak. Tuliskan di Buku Catatan Praktikum

https://github.com/user-attachments/assets/3f404021-c567-4f6c-8abb-d7b18a7a3152

## 📄 Pertanyaan Praktikum
1)	Gambarkan rangkaian schematic 5 LED running yang digunakan pada percobaan!
2)	Jelaskan bagaimana program membuat efek LED berjalan dari kiri ke kanan!
3)	Jelaskan bagaimana program membuat LED kembali dari kanan ke kiri!
4)	Buatkan program agar LED menyala tiga LED kanan dan tiga LED kiri secara bergantian dan berikan penjelasan disetiap baris kode nya dalam bentuk README.md!

<h2></h2>

<br>

[![banner](https://github.com/user-attachments/assets/f1f03032-41c0-4121-94e3-df1d513b42e5)](https://github.com/reslabunsoed/modul1_perulangan_percabangan)
