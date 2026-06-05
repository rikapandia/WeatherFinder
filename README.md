# 🌤️ WeatherFinder

Aplikasi cuaca real-time yang menampilkan informasi cuaca berdasarkan nama kota menggunakan Open-Meteo API (gratis, tanpa API key).

---

## Fitur

**Level 1 (Core)**
- TextInput controlled untuk pencarian kota
- Debounce 500ms dengan setTimeout + clearTimeout
- useEffect dengan dependency array [searchInput]
- Fetch 2 langkah: Geocoding → Forecast (Open-Meteo)
- 4 kondisi UI: Kosong, Loading, Error, Sukses
- AbortController di cleanup function
- Mapping weathercode WMO → label + emoji

**Level 2 (Pengembangan) ⭐**
- ⭐ Riwayat Pencarian — 5 kota terakhir sebagai chip yang bisa di-tap
- ⭐ Indikator Siang/Malam — field `is_day` untuk tampilkan ☀️ / 🌙
- ⭐ Suhu Min/Maks Harian — parameter daily dari API
- ⭐ Tombol Refresh — fetch ulang tanpa mengetik ulang
- ⭐ Background Dinamis — warna latar berubah sesuai kondisi cuaca

---

## Screenshot

Screenshot
Kosong
<img width="360" alt="kosong" src="https://github.com/user-attachments/assets/00ea9b0f-e8ca-48d8-a580-b4567fc5bf9e" />

Loading
<img width="360" alt="loading" src="https://github.com/user-attachments/assets/6ab53705-4f19-47ba-ae25-7663ac67ae38" />

Sukses
<img width="360" alt="sukses" src="https://github.com/user-attachments/assets/929027c3-4a38-4665-80c3-9840467ebf37" />

Error
<img width="360" alt="error" src="https://github.com/user-attachments/assets/aa11d22c-6be9-4abe-991f-647a97581282" />

## Cara Menjalankan

**Prasyarat:** Node.js dan Expo Go di HP

```bash
git clone https://github.com/USERNAME/WeatherFinder.git
cd WeatherFinder
npx expo start
```

Scan QR code yang muncul menggunakan Expo Go. Pastikan HP dan laptop di WiFi yang sama.

---

## Tech Stack

- React Native + Expo SDK 51
- JavaScript (ES6+)
- Open-Meteo API (gratis, tanpa API key)

--

---

**Nama:** Nama Kamu | **NIM:** 123456789 | **Kelas:** TI-XX
