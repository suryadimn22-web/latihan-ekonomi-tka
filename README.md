# Latihan & Ujian TKA — Bank Soal Multi-Mapel

Aplikasi latihan dan simulasi ujian TKA untuk MAN 2 Kota Pekanbaru.

## Isi repositori

- `index.html` — aplikasi latihan dan ujian (satu halaman, semua mapel)
- `bank_soal.json` — bank soal TKA Ekonomi (1.030 soal, 11 sub-elemen)
- `bank_soal_biologi.json` — Biologi (1.000 soal)
- `bank_soal_fisika.json` — Fisika (1.000 soal)
- `bank_soal_geografi.json` — Geografi (1.000 soal)
- `bank_soal_kimia.json` — Kimia (1.000 soal)
- `bank_soal_sosiologi.json` — Sosiologi (1.000 soal)
- `bank_soal_ppkn.json` — PPKn (1.000 soal)
- `bank_soal_sejarah.json` — Sejarah (1.000 soal)
- `bank_soal_bahasa_arab.json` — Bahasa Arab (1.000 soal)
- `bank_soal_bahasa_inggris_lanjut.json` — Bahasa Inggris Tingkat Lanjut (1.000 soal)
- `gambar/` — aset visual stimulus, dikelompokkan per mapel (`gambar/kim/`, `gambar/bio/`, dst.)
- `CNAME` — konfigurasi domain kustom

## Domain

Domain yang digunakan:

**https://tka.man2kotapekanbaru.sch.id**

DNS subdomain perlu diarahkan dengan CNAME ke:

`suryadimn22-web.github.io`

## Fitur

- Dropdown **Mata Pelajaran** di layar awal — bank soal mapel yang dipilih dimuat sesuai kebutuhan (tidak semua bank soal diunduh sekaligus)
- Mode latihan dan ujian
- Pilihan ganda, pilihan ganda kompleks (jawaban lebih dari satu), dan pilihan ganda kompleks kategori (Benar/Salah per pernyataan)
- Timer, navigasi soal, serta penandaan jawaban
- Pemeriksaan nilai dan pembahasan
- Stimulus dengan gambar/diagram/tabel (SVG) untuk soal yang membutuhkannya
- Tampilan responsif untuk HP dan komputer

## Menambah mapel baru

1. Siapkan `bank_soal_<mapel>.json` dengan struktur yang sama (`subElemen` + `soal`).
2. Taruh gambar pendukungnya di `gambar/<kode-mapel>/`.
3. Tambahkan satu baris di array `MAPEL_LIST` pada `index.html`.

> Bank soal 9 mapel baru (Biologi, Fisika, Geografi, Kimia, Sosiologi, PPKn, Sejarah, Bahasa Arab, Bahasa Inggris Tingkat Lanjut) sudah lulus audit struktur otomatis (kunci, pembahasan, dan distribusi soal lengkap), tetapi **belum melalui validasi akademik oleh guru mapel masing-masing**. Tinjau dulu sebelum dipakai untuk ujian resmi.
