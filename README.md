# 📺 QE3 IPTV Indonesia

## ⚠️ DISCLAIMER
Repository ini **HANYA untuk tujuan EDUKASI & penggunaan PRIBADI**.

- ❌ **DILARANG KERAS memperjualbelikan playlist ini**
- ❌ **DILARANG digunakan untuk layanan komersial**
- ❌ **TIDAK ADA JAMINAN KESTABILAN STREAM**

Pemilik repository **TIDAK menyimpan, meng-host, atau mengontrol konten siaran**.
Semua sumber berasal dari **URL publik di internet**.

---

## 🧠 Tentang QE3
**QE3 (Quality Enforcement Engine)** adalah sistem kurasi IPTV yang:

- ✅ Menguji stream **langsung via ffmpeg Jellyfin**
- ✅ Menolak stream yang:
  - Decode error
  - 0 ms playback
  - Segment rusak
  - PPS / reference overflow
- ✅ Menghapus duplicate
- ✅ Hanya menyimpan **REAL JELLYFIN-PLAYABLE**

---

## 🛠️ Metode Validasi
QE3 menggunakan:

- `docker exec jellyfin ffmpeg`
- Decode test (video stream)
- Segment read test
- Timeout & error pattern detection

Stream yang **tidak benar-benar bisa ditonton di Jellyfin akan DIBUANG**.

---

## 📥 Cara Pakai
Gunakan URL RAW berikut di Jellyfin / VLC / IPTV client:

```
https://raw.githubusercontent.com/Sincan2/qe3-iptv-indonesia/main/qe3.m3u
```

---

## 🔁 Update Otomatis
- Playlist diperbarui secara manual oleh QE3 engine
- Stream mati / rusak akan dihapus
- Stream valid akan dipertahankan

---

## 👤 Author
**BY Sincan2 – 2026**

> Gunakan dengan bijak. Hormati penyedia konten.
