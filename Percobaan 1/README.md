# Percobaan 1: Percabangan

## 🎯 Tujuan
Memahami dan mengimplementasikan konsep percabangan (if-else) dalam pemrograman mikrokontroler untuk mengontrol perilaku sistem secara dinamis.

## 💡 Spesifikasi yang Diharapkan
- LED menunjukkan fase mati --> lambat --> cepat --> lambat --> mati (reset)
- Rangkaian sesuai tanpa adanya error.

## ♻️ Langkah Percobaan
1. Persiapkan alat dan bahan

- Lakukan seperti halnya tugas pendahuluan poin 1
- Pastikan Arduino Uno terhubung dengan komputer

2. Program Percobaan
```cpp
#include <Arduino.h> // library dasar Arduino

// ===================== KONFIGURASI PIN =====================
// Tentukan pin digital yang digunakan untuk LED
const int ledPin = ;   // isi dengan nomor pin (contoh: 6)

// ===================== VARIABEL DELAY =====================
// Variabel untuk mengatur kecepatan kedip LED (dalam milidetik)
int timeDelay = ;  // isi nilai awal delay (contoh: 1000 ms)

void setup() {

  // ===================== MODE PIN =====================
  // Atur pin LED sebagai OUTPUT agar bisa mengirim sinyal
  pinMode(ledPin, );

}

void loop() {

  // ===================== LED MENYALA =====================
  // Kirim logika HIGH untuk menyalakan LED
  digitalWrite(ledPin, );

  // Beri jeda sesuai nilai timeDelay
  delay(); // isi dengan variabel delay

  // ===================== LED MATI =====================
  // Kirim logika LOW untuk mematikan LED
  digitalWrite(ledPin, );

  // Beri jeda lagi agar terlihat efek kedip
  delay(); // isi dengan variabel delay

  // ===================== PERUBAHAN KECEPATAN =====================
  // Setelah satu siklus nyala-mati, ubah kecepatan kedip LED

  if (timeDelay <= ) { 
    // Tentukan batas minimum delay (contoh: 100 ms)

    delay();        // beri jeda sebelum reset (contoh: 3000 ms)

    timeDelay = ;   // reset delay ke nilai awal (contoh: 1000 ms)

  } else {

    timeDelay -= ;  // kurangi delay secara bertahap (contoh: 100 ms)
  }

}
```
3. Simpan sketch dengan nama file modul1_percabangan
4. Konfigurasi Rangkaian
5. Berikutnya compile dan upload program ke dalam Arduino board. Perhatikan dan berikan analisi pada hasil yang terjadi, apakah sesuai dengan spesifikasi atau tidak. Tuliskan di Buku Catatan Praktikum

## 💡 Pertanyaan Praktikum
1)	Gambarkan schematic diagramnya!
2)	Pada kondisi apa program masuk ke blok if?
3)	Pada kondisi apa program masuk ke blok else?
4)	Jika program yang dibuat memiliki alur mati -> lambat -> cepat -> reset (mati), ubah menjadi LED tidak langsung reset → tetapi berubah dari cepat → sedang → mati dan berikan penjelasan disetiap baris kode nya dalam bentuk README.md!

<h2></h2>

<br>

[![banner](https://github.com/user-attachments/assets/f1f03032-41c0-4121-94e3-df1d513b42e5)](https://github.com/reslabunsoed/modul1_perulangan_percabangan)
