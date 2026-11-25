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

## Panjang video (pilihan paling atas)
Pilih **Auto** (ikut panjang skrip, maksimum 2 minit) atau tetapkan 15s, 30s, 45s, 1 min, 1.5 min atau 2 min. Semua babak diregang/dipendekkan supaya tepat dengan panjang yang dipilih.

## Muzik latar
Pilih *Chill*, *Upbeat* (dijana automatik) atau **Muzik sendiri** — klik/seret fail MP3, WAV, M4A atau OGG. Boleh atur kelantangan, ulang muzik jika lebih pendek daripada video, dan pilih saat mula. Muzik di-fade out pada hujung video.

Hiasan latar (Partikel, Grid, Bentuk) boleh digabungkan dengan warna atau gambar sendiri.

## Suara latar (voiceover)
- **Rakam suara sendiri** — setiap babak ada butang 🎙 Rakam. Baca teks babak, tekan ■ Henti. Babak dipanjangkan ikut suara; senyap di awal & hujung dipotong automatik. Boleh dengar (▶), rakam semula, atau buang.
- **Fail suara** — muat naik satu fail MP3/WAV/M4A untuk keseluruhan video (contoh suara AI dari ElevenLabs/CapCut). Tanda "Panjang video ikut panjang suara" supaya video sama panjang dengan suara.
- Muzik latar diperlahankan automatik bila ada suara.
- Suara robot terbina dalam pelayar tidak boleh dirakam ke dalam fail video, sebab itu ia tidak disediakan.

## Gambar dalam babak
Muat naik gambar, logo atau ikon di bahagian **Gambar dalam babak** (bawah skrip). Setiap gambar dapat nama (dari nama fail). Pilih animasi/posisi/saiz/gerakan, letak kursor dalam skrip, dan klik **+ Sisip** — atau taip sendiri:

```
[gambar: logo, lantun, kanan, besar, terapung, 1s]
```

| Jenis | Pilihan |
|---|---|
| Animasi masuk | `pop` `pudar` `zum` `dari-kiri` `dari-kanan` `dari-atas` `dari-bawah` `putar` `lantun` |
| Posisi | `tengah` `atas` `bawah` `kiri` `kanan` `penuh` (gambar penuh skrin di belakang teks) |
| Saiz | `kecil` `sederhana` `besar` |
| Gerakan berterusan | `terapung` `goyang` `pusing` |
| Masa | `1s`, `0.5s` … = muncul selepas sekian saat |

- Nama boleh juga nombor: `[gambar: 2]` = gambar kedua dalam senarai.
- Baris yang ada gambar sahaja → babak gambar besar.
- Beberapa arahan gambar dalam satu baris → gambar diletak bersebelahan.
- Dalam senarai, `- [gambar: ikon] Item` → ikon menggantikan bulatan.
- Skrin menegak (9:16): posisi `kiri`/`kanan` jadi `atas`/`bawah` secara automatik.

## Format skrip
| Tulis | Hasil |
|---|---|
| `# Tajuk` | Babak tajuk besar dengan garisan aksen |
| `- item` | Senarai; item muncul satu persatu (baris sebelum yang berakhir `:` jadi tajuk senarai) |
| `*perkataan*` | Perkataan ditonjolkan dengan warna aksen |
| Baris pendek dengan nombor (`60%`, `RM 5,000`, `33 juta`) | Nombor besar dikira naik secara animasi |
| Baris biasa | Babak teks |

Semua diproses dalam pelayar — tiada pelayan, tiada muat naik.
