# SISTEM PARKIR OTOMATIS BERBASIS ARDUINO UNO

Proyek ini adalah sistem manajemen parkir pintar yang dibuat sebagai implementasi praktikum Mikrokontroler. Sistem ini mensimulasikan kontrol akses kendaraan dan pemantauan kapasitas lahan parkir secara otomatis menggunakan platform Tinkercad.

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
1. **Monitoring:** Potensiometer bertindak sebagai simulator kapasitas. Jika diputar, nilai variabelnya akan dianggap sebagai jumlah mobil yang ada di dalam.
2. **Indikasi Status:** - **Lampu Hijau/Kuning:** Menyala jika slot masih tersedia, LCD menampilkan "TERSEDIA".
   - **Lampu Merah:** Menyala jika kapasitas penuh, LCD menampilkan "PENUH".
3. **Kontrol Akses:** Saat tombol (Push Button) ditekan, sistem mengecek kuota. Jika tersedia, Servo akan membuka palang (90°). Jika penuh, palang tetap tertutup.
4. **Otomasi Tambahan:** Motor DC aktif secara otomatis untuk menjaga sirkulasi udara di dalam gedung parkir.

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
* **Simulasi Tinkercad:** https://www.tinkercad.com/things/4OfHwppKm3U-cool-blorr/editel
* **Video Demo (YouTube):** [https://youtu.be/AW9QHFLfN3U](https://youtu.be/AW9QHFLfN3U)
