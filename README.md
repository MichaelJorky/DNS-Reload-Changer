# **DNS Reload & Changer**

## 📌 **Deskripsi**

**DNS Reload & Changer** adalah aplikasi Windows yang berfungsi untuk melakukan rotasi DNS, mengganti DNS secara otomatis, serta melakukan pengecekan (resolve) kecepatan DNS.
Aplikasi ini sangat berguna untuk pengguna yang ingin mencari DNS paling cepat secara otomatis atau mengganti DNS secara berkala tanpa perlu melakukan konfigurasi manual.

Aplikasi ini mendukung semua sistem operasi berikut:

* Windows 7 (32-bit & 64-bit)
* Windows 8 / 8.1 (32-bit & 64-bit)
* Windows 10 (32-bit & 64-bit)
* Windows 11 (32-bit & 64-bit)

---

## ✨ **Fitur Utama**

### ✅ **1. Rotasi DNS Otomatis**

Aplikasi dapat mengganti DNS secara otomatis berdasarkan interval waktu yang dipilih (misalnya setiap 1 menit).

### ✅ **2. Auto Load DNS List**

Daftar DNS otomatis dimuat dari file `dnslist.txt` saat aplikasi dijalankan.

### ✅ **3. Resolve dan Cek Latency DNS**

Setiap DNS dalam daftar akan diuji kecepatan resolve-nya (latency).
Hasilnya ditampilkan berwarna:

* **Hijau** → DNS cepat & dapat digunakan
* **Kuning** → DNS sedang di cek / digunakan untuk rotasi
* **Merah** → DNS tidak dapat digunakan / gagal resolve

### ✅ **4. User-Friendly**

Tampilan sederhana, ringan, dan mendukung semua adapter (Ethernet/WiFi).

### ✅ **5. Editable DNS List**

Pengguna dapat menambah, menghapus, atau mengedit daftar DNS langsung dari file `dnslist.txt`.

---

## 📁 **Format File dnslist.txt**

File daftar DNS menggunakan format **split**, diproses dengan:

```
Split([';', ',', '|', '='])
```

Artinya Anda dapat memisahkan data menggunakan:

* `;`
* `,`
* `|`
* `=`

### 📌 **Contoh Format DNS List**

```
1;Google Public DNS;8.8.8.8;8.8.4.4;...;Ipv4 Default
2;OpenDNS;208.67.222.222;208.67.220.220;...;Ipv4 Default
```

Setiap baris berisi:

1. Nomor
2. Nama DNS
3. Primary DNS
4. Secondary DNS
5. Field tambahan (opsional)
6. Jenis DNS (misalnya Ipv4 Default)

---

## 🖥️ **Tampilan Aplikasi**

Aplikasi menampilkan daftar DNS lengkap dengan:

* Nama DNS
* Primary / Secondary DNS
* Resolve Time (ms)
* Jenis DNS
* Warna status usability

---

## 🚀 **Cara Menggunakan**

1. Jalankan aplikasi **DNS Reload & Changer v1.0.0.1 (Beta Version)**
2. Aplikasi otomatis:

   * Memuat file `dnslist.txt`
   * Mengecek setiap DNS
   * Menampilkan kecepatan resolve
3. Pilih interface (misalnya **Ethernet** atau **WiFi**)
4. Pilih interval rotasi DNS
5. Klik **Start**
6. Aplikasi akan mengganti DNS otomatis berdasarkan DNS tercepat atau berdasarkan daftar rotasi Anda.

---

## 📝 **Edit Daftar DNS**

Untuk menambah DNS baru:

1. Buka file `dnslist.txt`
2. Tambahkan baris baru dengan format:

   ```
   nomor;nama_dns;primary_dns;secondary_dns;...;type
   ```
3. Simpan file
4. Restart aplikasi

---

## ⚠️ **Status**

**Beta Version** — beberapa fitur mungkin masih dalam pengembangan.

---
