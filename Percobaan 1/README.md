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
const int ledPin = 6;     // Menentukan pin digital yang digunakan untuk LED
int timeDelay = 1000;     // Waktu delay awal (dalam milidetik)

void setup() {
  pinMode(ledPin, OUTPUT);  // Mengatur pin LED sebagai output
}

void loop() {
  // Menyalakan LED (HIGH = ON)
  digitalWrite(ledPin, HIGH);
  delay(timeDelay);         // Tunggu sesuai waktu delay

  // Mematikan LED (LOW = OFF)
  digitalWrite(ledPin, LOW);
  delay(timeDelay);         // Tunggu lagi sesuai waktu delay

  // Setelah satu siklus nyala-mati, ubah kecepatan kedip LED
  if (timeDelay <= 100) {
    // Jika delay sudah sangat cepat (<= 100 ms)
    delay(3000);            // Beri jeda 3 detik sebelum mengulang
    timeDelay = 1000;       // Reset delay ke nilai awal (lambat lagi)
  } else {
    // Jika belum mencapai batas minimum
    timeDelay -= 100;       // Kurangi delay 100 ms agar LED berkedip lebih cepat
  }
}
```
3. Simpan sketch dengan nama file modul1_percabangan
4. Konfigurasi Rangkaian
5. Berikutnya compile dan upload program ke dalam Arduino board. Perhatikan dan berikan analisi pada hasil yang terjadi, apakah sesuai dengan spesifikasi atau tidak. Tuliskan di Buku Catatan Praktikum

https://github.com/user-attachments/assets/173b2f90-c611-4f0a-a696-b3776e8a02c9

## 💡 Pertanyaan Praktikum
1)	Gambarkan schematic diagramnya!
2)	Pada kondisi apa program masuk ke blok if?
3)	Pada kondisi apa program masuk ke blok else?
4)	Jika program yang dibuat memiliki alur mati -> lambat -> cepat -> reset (mati), ubah menjadi LED tidak langsung reset → tetapi berubah dari cepat → sedang → mati dan berikan penjelasan disetiap baris kode nya dalam bentuk README.md!

<h2></h2>

<br>

[![banner](https://github.com/user-attachments/assets/f1f03032-41c0-4121-94e3-df1d513b42e5)](https://github.com/reslabunsoed/modul1_perulangan_percabangan)
