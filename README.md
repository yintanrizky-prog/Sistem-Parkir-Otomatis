# SISTEM PARKIR OTOMATIS BERBASIS ARDUINO UNO

---

## 👤 Identitas Mahasiswa
* **Nama:** Intan Rizky Yuniar
* **NIM:** 24090620034
* **Mata Kuliah:** Praktikum Mikrokontroler
* **Program Studi:** D4 Teknik Elektronika

---

## 📝 Deskripsi Proyek
Sistem ini dirancang untuk menggantikan pengelolaan parkir manual menjadi otomatis. Dengan memanfaatkan mikrokontroler Arduino Uno, sistem dapat mendeteksi ketersediaan slot, mengatur palang pintu, dan memberikan indikasi visual maupun informasi real-time kepada pengguna melalui layar LCD dan lampu indikator.

---

## 🛠️ Implementasi Materi Praktikum
Proyek ini mengintegrasikan berbagai konsep yang telah dipelajari selama praktikum, antara lain:
* **Input Analog:** Penggunaan Potensiometer untuk membaca data variabel (kapasitas).
* **Input Digital:** Penggunaan Push Button sebagai pemicu (interrupt) sistem.
* **Output PWM:** Penggunaan Motor Servo untuk penggerak palang pintu dengan sudut presisi.
* **Komunikasi Serial I2C:** Integrasi LCD 16x2 untuk efisiensi penggunaan pin Arduino.
* **Aktuator DC:** Penggunaan Motor DC sebagai simulasi sistem sirkulasi udara (Exhaust Fan).

---
  
* ## 🚀 Cara Kerja Sistem
1. **Monitoring Kapasitas:** Potensiometer bertindak sebagai simulator jumlah kendaraan. Data analog dari potensiometer diolah oleh Arduino dan hasilnya ditampilkan secara real-time pada **LCD 16x2**.
2. **Indikasi Status di LCD & LED:**
   - Jika slot tersedia, **LCD** menampilkan pesan "Slot Tersedia" beserta jumlah kuotanya, dan **LED Hijau/Kuning** menyala.
   - Jika kapasitas penuh, **LCD** akan berubah menampilkan pesan "Parkir Penuh", dan **LED Merah** akan menyala.
4. **Logika Palang Pintu (Servo):** - Pengendara menekan **Push Button** untuk masuk.
   - Mikrokontroler akan mengecek kondisi kuota. Jika masih ada slot, **Servo** akan bergerak memutar 90 derajat (membuka palang) selama beberapa detik, lalu kembali ke posisi 0 derajat (menutup).
   - Jika kondisi parkir penuh (berdasarkan data potensiometer), **Servo** akan tetap diam (0 derajat) meskipun tombol ditekan, untuk mencegah kendaraan masuk.
5. **Otomasi Sirkulasi:** **Motor DC** aktif secara otomatis sebagai simulasi sistem kipas untuk menjaga sirkulasi udara di dalam area parkir sesuai dengan kepadatan kendaraan.

---

## 🔌 Rangkaian (Wiring)
Berikut adalah konfigurasi pin yang digunakan dalam rangkaian:

| Komponen | Pin Arduino | Fungsi |
| :--- | :--- | :--- |
| **Push Button** | D2 | Input Tombol Buka Palang |
| **Motor Servo** | D9 | Output Penggerak Palang |
| **LCD 16x2 I2C** | A4 (SDA), A5 (SCL) | Display Informasi |
| **Potensiometer** | A0 | Input Simulasi Kapasitas |
| **LED Hijau** | D13 | Indikator Slot Tersedia |
| **LED Kuning** | D11 | Indikator Slot Hampir Penuh |
| **LED Merah** | D12 | Indikator Parkir Penuh |
| **Motor DC** | D3 | Output Kipas Sirkulasi |

---

## 📸 Dokumentasi & Demo

### Video Demonstrasi
Penjelasan detail komponen dan cara kerja alat dapat dilihat pada video berikut:

[![Video Demo Sistem Parkir](https://img.youtube.com/vi/AW9QHFLfN3U/0.jpg)](https://www.youtube.com/watch?v=AW9QHFLfN3U)

### Link Penting
* **Simulasi Tinkercad:** https://www.tinkercad.com/things/4OfHwppKm3U-cool-blorr/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard&sharecode=DKbZeGkXEC2trWeNreHmRA693tiOKtRsmGbn7QqQP0o
* **Video Demo (YouTube):** [https://youtu.be/AW9QHFLfN3U](https://youtu.be/AW9QHFLfN3U)
