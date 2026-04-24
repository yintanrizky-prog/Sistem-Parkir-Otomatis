* Nama        = Intan Rizky Yuniar
* NIM         = 24090620034
* Mata Kuliah = UTS Mikrokontroller

# Sistem-Parkir-Otomatis
Proyek ini merupakan sistem purwarupa (prototype) manajemen parkir otomatis yang dirancang untuk mengoptimalkan kuota lahan parkir secara real-time. Sistem ini mengintegrasikan sensor input untuk memantau kapasitas dan aktuator untuk mengontrol akses kendaraan.

## 🛠️ Penjelasan Komponen
* **Arduino Uno:** Sebagai pusat kendali (otak) sistem.
* **Servo Motor:** Bertugas sebagai mekanisme palang pintu otomatis.
* **LCD 16x2 (I2C):** Menampilkan status ketersediaan slot parkir secara visual.
* **Potensiometer:** Simulasi sensor untuk membaca kapasitas kendaraan di dalam area parkir.
* **Push Button:** Pemicu (trigger) untuk membuka palang pintu masuk.
* **LED (Hijau, Kuning, Merah):** Indikator visual status kapasitas (Tersedia, Waspada, atau Penuh).
* **Motor DC:** Simulasi sistem sirkulasi udara (Exhaust Fan) otomatis.

# Daftar Pin Utama:
* **Servo (Palang):** Pin 9
* **Push Button:** Pin 2
* **Potensiometer:** Pin A0
* **LCD I2C:** SDA (A4), SCL (A5)
* **Motor DC:** Pin 3
* **LED Merah (Penuh):** Pin 12
* **LED Kuning (Waspada):** Pin 11
* **LED Hijau (Tersedia):** Pin 13

### 📺 Video Demonstrasi
Berikut adalah penjelasan komponen, konfigurasi pin, dan simulasi cara kerja alat:

{Sistem Parkir Otomatis(https://youtu.be/AW9QHFLfN3U ini link ytb)}
