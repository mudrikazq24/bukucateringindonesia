# BukuCatering — landing page

Redesain berdasarkan PRD_FLUTTER_ANDROID.md v1.5 dan DESIGN_ANDROID.md.

## Preview tanpa instalasi

Ekstrak seluruh ZIP, lalu buka `preview.html`. Biarkan folder `public/` berada di sebelah file tersebut agar screenshot dan ikon terbaca.

## Pengembangan

Gunakan Node.js 22.12+ atau 24 LTS.

```sh
npm ci
npm run dev
```

## Build

```sh
npm run build
npm run preview
```

Folder `dist/` siap untuk hosting statis pada root domain.

## Desain dan interaksi

- Hijau #245C43, krem #F8F7F2, sage #EDF2E8, amber #FFF0D8.
- Screenshot asli; demo pemilihan tanggal terpisah dan berlabel ilustrasi.
- Reveal sekali saat scroll, transisi screenshot 250–300 ms, hover tombol ringan.
- Tanpa autoplay, parallax, atau gerakan dekoratif berulang.
- Pengaturan `prefers-reduced-motion` menonaktifkan animasi; konten tetap terlihat.
- Tab mendukung tombol panah, Home/End; tombol tanggal memakai aria-pressed.

## Cakupan konten

Menekankan tanggal kirim eksplisit, slot makan, menu per jadwal, status kirim terpisah dari pembayaran, satu DP/pelunasan, invoice teks dan QRIS terpisah, ekspor Excel, pelanggan dan master menu, serta akun dan langganan lewat admin. Pencarian nama/nomor pesanan dan filter pembayaran kini terlihat pada screenshot terbaru. Tidak mengiklankan pembayaran otomatis maupun sinkronisasi WhatsApp otomatis. Harga langganan dan kontak admin belum tersedia di dokumen.

Tautan APK, versi 1.0.0, perkiraan ukuran dan screenshot tetap menggunakan materi landing page awal. Tautan rilis belum diperiksa ke server.

## Verifikasi

Build produksi berhasil. Pemeriksaan render awal mencakup bagian halaman, target navigasi, aset gambar, lima tab, enam FAQ dan demo yang memilih 21 serta 23 September tanpa menambahkan tanggal 22. Review visual dan pengujian interaksi di browser/perangkat belum selesai karena browser uji tidak tersedia di lingkungan eksekusi.

## Revisi konten terbaru

Teks kecil “Yang perlu disiapkan, langsung terlihat.” di visual utama dihapus. Promosi pengingat harian dihilangkan sementara menunggu rincian fitur terbaru; bagian fitur diganti dengan pelanggan dan master menu yang sudah dijelaskan dalam dokumen.

Favicon tab browser menggunakan logo BukuCatering, disematkan langsung agar tampil pada hosting dan saat preview.html dibuka dari file lokal.

## Screenshot terbaru

Kelima tampilan diperbarui menggunakan upload terbaru. File upload Beranda.jpg dan Detail Pesanan.jpg tertukar namanya; aset dipetakan menurut isi gambar. Tab Pengaturan ditambahkan.

Trial 14 hari ditambahkan berdasarkan konfirmasi pemilik, pada informasi unduh, cara mulai, FAQ dan ajakan penutup. Tidak menetapkan tanggal mulai trial atau syarat pembayaran yang belum dikonfirmasi.

Kelima screenshot diganti lagi dengan unggahan terbaru berakhiran (1). Pemetaan Beranda/Detail tetap mengikuti isi gambar, bukan nama unggahannya. Informasi trial 14 hari tetap disertakan.

Screenshot diperbarui dengan unggahan (2) tanggal 5 Oktober 2026. Seluruh nama file pada unggahan ini sudah cocok dengan isi layar; tidak memakai pemetaan tertukar dari unggahan sebelumnya.

Perbaikan mobile: override hero desktop yang menyebabkan dua kolom pada HP diperbaiki. Hero menggunakan satu kolom di bawah 760px, gambar memakai tinggi otomatis dan tidak menyusut di flex, serta metadata dapat membungkus. Build berhasil; verifikasi visual browser tetap diperlukan.

## Komposisi HP

Layout satu kolom hingga 760px; ukuran judul mengikuti lebar layar. Tombol unduh melebar, tab dua kolom, fitur satu kolom, dan screenshot mempertahankan rasio. Pada HP, catatan dekoratif dipindahkan di bawah screenshot agar tidak menutupi aplikasi. Jarak dan ukuran teks ditingkatkan; aturan tambahan menangani lebar 320–360px. Build berhasil. Verifikasi visual browser/perangkat belum dilakukan.

Kelima screenshot diperbarui dengan unggahan (3) tanggal 7 Oktober 2026. Istilah pada teks pendamping mengikuti tampilan terbaru: master paket catering dan rekap paket.
