# Pemilih Video Grafik

Alat satu halaman untuk hasilkan video motion graphic: pilih gaya, tulis skrip, tekan **Create Video**.

## Cara guna
1. Buka `index.html` dalam Google Chrome atau Microsoft Edge (klik dua kali pun boleh).
2. Tulis skrip — setiap baris = satu babak.
3. Pilih format, tema, font, animasi, latar, peralihan, kelajuan, muzik & kualiti.
4. Tekan **▶ Pratonton** untuk tengok dulu, atau **Create Video** untuk rakam dan muat turun (MP4 di Chrome terkini, WebM di pelayar lain).

> Biarkan tab terbuka semasa rakaman — video dirakam dalam masa nyata.

## Latar sendiri
Di bahagian **Sumber latar**:
- **Ikut tema** — guna warna tema yang dipilih.
- **Warna sendiri** — pilih 2 warna (gradien), atau tekan "Guna 1 warna sahaja" / pilih hiasan *Kosong* untuk warna padu. Warna teks dipilih automatik ikut kecerahan latar.
- **Gambar sendiri** — klik atau seret satu atau lebih gambar sekaligus.
  - Susun turutan dengan **seret** thumbnail, atau butang **‹ ›**. Butang **×** buang gambar.
  - **Tukar gambar**: *Setiap babak* (gambar 1 → babak 1, gambar 2 → babak 2, …, berulang) atau *Sama rata sepanjang video*.
  - Peralihan antara gambar guna crossfade; *Zum perlahan* bergerak masuk/keluar berselang-seli.
  - Lapisan Gelap (teks putih) atau Cerah (teks hitam), dan kekuatan lapisan.
- Gambar dan muzik sendiri disimpan dalam pelayar (IndexedDB) untuk kali seterusnya.

## Panjang video
Pilih **Auto** (ikut panjang skrip, maksimum 2 minit) atau tetapkan 15s, 30s, 45s, 1 min, 1.5 min atau 2 min. Semua babak diregang/dipendekkan supaya tepat dengan panjang yang dipilih.

## Muzik latar
Pilih *Chill*, *Upbeat* (dijana automatik) atau **Muzik sendiri** — klik/seret fail MP3, WAV, M4A atau OGG. Boleh atur kelantangan, ulang muzik jika lebih pendek daripada video, dan pilih saat mula. Muzik di-fade out pada hujung video.

Hiasan latar (Partikel, Grid, Bentuk) boleh digabungkan dengan warna atau gambar sendiri.

## Format skrip
| Tulis | Hasil |
|---|---|
| `# Tajuk` | Babak tajuk besar dengan garisan aksen |
| `- item` | Senarai; item muncul satu persatu (baris sebelum yang berakhir `:` jadi tajuk senarai) |
| `*perkataan*` | Perkataan ditonjolkan dengan warna aksen |
| Baris pendek dengan nombor (`60%`, `RM 5,000`, `33 juta`) | Nombor besar dikira naik secara animasi |
| Baris biasa | Babak teks |

Semua diproses dalam pelayar — tiada pelayan, tiada muat naik.
