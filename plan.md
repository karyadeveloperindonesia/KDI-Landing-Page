# Rencana Implementasi — KDI Solusi Digital Bisnis

## Tujuan
Membangun landing page satu halaman berbahasa Indonesia untuk Karya Developer Indonesia (KDI) yang meniru struktur, tipografi, ritme ruang, warna, kartu metrik, dan isi screenshot referensi. Informasi yang terbaca dipertahankan; tidak membuat klaim/nomor kontak baru. Semua navigasi dan CTA mengarah ke bagian relevan di halaman sampai kontak nyata diberikan.

## Arah Desain (disetujui berdasarkan referensi)
- **Gerakan desain:** minimalisme editorial B2B dengan sentuhan Swiss/neo-grotesk modern.
- **Prinsip inti:** komposisi asimetris; teks dan angka menjadi fokus; kartu bersudut lembut dengan garis halus; aksen warna hanya membantu pemindaian informasi.
- **Filosofi warna:** hitam arang dan putih hangat membangun kesan tegas/tepercaya, hijau mint menandai keberhasilan dan status, biru sangat muda menghangatkan bagian solusi/CTA, krem pucat menyeimbangkan statistik.
- **Paradigma tata letak:** lebar konten terpusat tetapi bagian header, hero, pengantar section dan grid kartu menggunakan kolom editorial asimetris; komponen menumpuk alami di mobile.
- **Elemen khas:** gambar monogram KDI terlampir dipasangkan dengan wordmark; kartu dashboard/KPI dengan label kecil uppercase dan titik hijau; CTA besar berbentuk pil hitam di atas panel biru pucat.
- **Interaksi:** navigasi anchor yang jelas, menu mobile tombol buka/tutup, tautan CTA ke kontak/section terkait, FAQ native yang bisa dibuka dengan keyboard.
- **Animasi:** transisi hover halus pada tautan/kartu, tanpa animasi dekoratif besar; hormati `prefers-reduced-motion`.
- **Tipografi:** Plus Jakarta Sans sebagai sans utama untuk teks dan heading; hierarki heading berat, label tracking lebar, beberapa frasa italic ringan sebagaimana screenshot.
- **Esensi merek:** partner teknologi bisnis Indonesia yang mengubah kebutuhan operasional menjadi sistem yang langsung dipakai; profesional, lugas, meyakinkan.
- **Suara merek:** headline menekankan hasil dan kejelasan; CTA langsung namun tidak memaksa. Contoh: “Wujudkan aplikasi & sistem bisnis Anda, cepat, tepat, tanpa repot.” dan “Diskusikan kebutuhan aplikasi atau sistem perusahaan Anda langsung bersama tim spesialis kami hari ini secara gratis.”
- **Wordmark/logo:** gunakan gambar monogram KDI yang diberikan pengguna, dengan wordmark “KDI.” dan subnama “KARYA DEVELOPER INDONESIA” tetap menyertainya.
- **Warna merek khas:** hijau mint/teal lembut untuk status sukses, dipakai hemat sebagai penanda KDI.

## Struktur Produk
- Navigasi: Solusi Bisnis, Keunggulan Kami, Hasil Nyata, Tanya Jawab; CTA Konsultasi Gratis dan Mulai Proyek.
- Hero: pill garansi, pesan utama, deskripsi PT Karya Developer Indonesia, CTA dan dua jaminan; di kanan empat kartu operasional/99,8%/100%/+240%.
- Pita nama klien: ManERP Solutions, Tenda Membran ID, Mauiklan Media, Logistik Nusantara, Retail Smart Indonesia.
- Keunggulan/komitmen: lima kartu garansi, kemudahan staf, transparansi biaya, terima beres dan respon cepat.
- Solusi siap pakai: empat layanan (aplikasi mobile, sistem ERP/gudang/kasir, website profil, landing page penjualan) serta CTA kebutuhan khusus.
- Hasil nyata: tiga kisah implementasi ManERP, Tenda Membran Surabaya, dan Mauiklan dengan metrik yang tampak pada referensi serta strip jaminan.
- FAQ: lima pertanyaan dan jawaban sebagaimana referensi.
- CTA penutup: panel biru dengan konsultasi WhatsApp, jelajahi solusi, dan empat benefit.
- Footer: layanan, perusahaan, alamat operasional, identitas KDI, komunikasi WhatsApp, hak cipta dan tautan kebijakan.

## Implementasi
- Website statis satu halaman tanpa server data atau akun; HTML semantik, CSS responsif, dan JavaScript kecil untuk menu mobile.
- Direktorinya: `index.html` (konten dan penggunaan logo), `styles.css` (sistem desain/breakpoint), `script.js` (interaksi menu), `manus-routes.json` (deklarasi route statis), `/manus-storage/…` (gambar logo pengguna), dan `app.config.ts` (URL HTTPS metadata logo platform).
- Jalankan server statis pada port runtime 3000 sesuai konfigurasi proyek.
- Tidak menambahkan ilustrasi stok; elemen visual dashboard dibuat sebagai komponen HTML/CSS agar serupa dengan referensi.
- Mobile: header ringkas, satu kolom, kartu metrik dan layanan menumpuk, kartu narasi tidak overflow, CTA serta footer menjadi kolom.
- CTA WhatsApp diarahkan ke label kontak di footer; nomor WhatsApp langsung tidak ditambahkan karena tidak terlihat pada screenshot referensi.
- Tidak menerbitkan website secara publik tanpa permintaan eksplisit; serahkan URL Preview setelah server terverifikasi.
