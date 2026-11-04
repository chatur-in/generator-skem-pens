# Generator Formulir SKEM PENS

Aplikasi web untuk membantu mahasiswa **Politeknik Elektronika Negeri Surabaya (PENS)** membuat, mempratinjau, dan mengunduh **Formulir Kegiatan SKEM** (Satuan Kredit Kegiatan Mahasiswa) langsung sebagai PDF siap cetak berukuran A4.

🔗 **Website:** [https://skem-pens.vercel.app](https://skem-pens.vercel.app)

---

## ✨ Fitur

**Pengisian formulir**
- **Pratinjau langsung** – setiap perubahan data langsung tampil pada tata letak kertas formulir resmi.
- **Pilihan siap pakai** – program studi (D3 dan Sarjana Terapan) dan departemen tersedia sebagai pilihan, dengan opsi **Lainnya** untuk diketik manual.
- **Data tersimpan otomatis** di browser, jadi tidak perlu mengetik ulang saat membuka lagi.
- **Kosongkan tanggal** untuk surat yang tanggalnya akan diisi tangan.

**Lampiran bukti kegiatan**
- Unggah banyak foto sekaligus. Format yang didukung: JPG, PNG, WebP, GIF, BMP, AVIF, SVG, HEIC/HEIF, dan PDF.
- **Putar foto** 90° ke kiri atau kanan.
- **Tata letak halaman otomatis:** foto potret 1 per halaman, foto lanskap 2 per halaman.

**Tanda tangan digital**
- Unggah tanda tangan **mahasiswa** dan **verifikator** (opsional).
- **Hapus latar putih otomatis** dan pemotongan ruang kosong di sekeliling tanda tangan.

**Unduh PDF**
- **Tiga pilihan kualitas** dengan perkiraan ukuran file: Hemat, Standar, dan Tajam.
- Garis tabel dan logo dirender rapi dan seragam.
- Tersedia juga tombol **Cetak** langsung dari browser.

**Privasi**
- Berjalan sepenuhnya di sisi klien (*client-side*). Tidak ada backend dan tidak ada data yang dikirim ke server. Data hanya tersimpan di browser perangkat Anda.

---

## 📖 Cara Pakai

1. Buka [skem-pens.vercel.app](https://skem-pens.vercel.app).
2. Isi **Identitas mahasiswa** dan **Informasi kegiatan**.
3. Unggah **lampiran bukti** (sertifikat atau foto dokumentasi). Putar foto jika orientasinya belum pas.
4. Isi bagian **Verifikasi** dan **Pernyataan**, lalu unggah tanda tangan digital jika ada.
5. Periksa hasilnya pada pratinjau.
6. Klik **Unduh PDF**, pilih kualitas (Hemat, Standar, atau Tajam), lalu simpan file.

---

## 🛠️ Teknologi

Proyek ini hanya terdiri dari satu file HTML dengan CSS dan JavaScript murni (*vanilla*), tanpa proses *build*.

| Kebutuhan | Pustaka |
|---|---|
| Menangkap halaman menjadi gambar | [html2canvas](https://html2canvas.hertzen.com/) 1.4.1 |
| Membuat dokumen PDF | [jsPDF](https://github.com/parallax/jsPDF) 2.5.1 |
| Membaca lampiran PDF | [PDF.js](https://mozilla.github.io/pdf.js/) 3.11.174 |
| Membaca foto HEIC/HEIF | [heic2any](https://github.com/alexcorvi/heic2any) 0.0.4 |

Pustaka dimuat dari CDN, sehingga koneksi internet dibutuhkan saat pertama kali membuka halaman.

---

## 💻 Menjalankan Secara Lokal

```bash
git clone <url-repositori>
cd <nama-folder>
```

Buka `index.html` langsung di browser, atau jalankan server lokal sederhana:

```bash
npx serve .
# atau
python3 -m http.server 8000
```

---

## 🚀 Deploy

Proyek ini dapat di-*deploy* ke layanan hosting apa pun, seperti Vercel, Netlify, atau GitHub Pages. Tidak ada konfigurasi build yang diperlukan.

---

## 👤 Pengembang

| | |
|---|---|
| **Nama** | Febrian Catur Wahyu Fibisono |
| **NRP** | 3125600035 |
| **Program Studi** | S.Tr. Teknik Informatika |
| **Institusi** | Politeknik Elektronika Negeri Surabaya (PENS) |
| **Email** | [cathur@outlook.co.id](mailto:cathur@outlook.co.id) |

---

> Proyek ini dibuat sebagai alat bantu dan tidak dikelola secara resmi oleh PENS. Pastikan format formulir masih sesuai dengan pedoman SKEM yang berlaku sebelum diserahkan.
