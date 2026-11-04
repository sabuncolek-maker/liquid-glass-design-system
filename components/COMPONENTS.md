# Komponen — LAPIS Design System 2.5D & 3D

Semua komponen mengikuti: palet di `tokens/`, sudut membulat halus, satu cahaya dari kiri atas, dan tingkat kedalaman L0–L3. Setiap komponen punya state Default, Active, dan Transition (spring melenting halus).

## 1. Layered Panel
Panel dasar tempat informasi tinggal. Permukaan Panel Deep atau Silver gelap di tingkat L1–L2, bayangan sesuai tingkat, radius 18px. Isi berjarak kelipatan 8px dari tepi.

## 2. Depth Card
Kartu dengan sisi tebal: permukaan atas terang, sisi bawah lebih gelap setebal 6–10px, memberi kesan papan 2.5D yang terangkat di L2. Radius 18px.

## 3. Primary Button
Biru Elektrik penuh, teks putih Inter 600, radius 14px, bayangan L2. State Active: turun 2px dan bayangan mengecil, seperti tombol fisik yang ditekan. Satu tombol utama per layar.

## 4. Secondary Button
Permukaan Silver gelap (Panel Deep dengan teks Light Silver), radius 14px, bayangan L1–L2. Mendampingi tombol utama, tidak pernah lebih menonjol darinya.

## 5. Navigation Bar
Bar horizontal di L2 melayang di atas latar: logo sederhana di kiri, 3–5 tautan teks, satu aksi utama di kanan. Tanpa pil melayang, tanpa kaca.

## 6. Icon Button
Tombol persegi membulat 14px berisi satu ikon garis sederhana (cari, lonceng, pengguna, panah). Permukaan Panel Deep, bayangan L1.

## 7. Toggle Switch
Pil penuh: rel Silver gelap saat mati, Biru Elektrik saat menyala. Knob lingkaran Light Silver bergeser dengan spring dan sedikit melenting di ujung. Label selalu di luar pil.

## 8. Progress Indicator
Batang berlapis: rel Panel Deep, isian Biru → Cyan dengan sisi atas lebih terang 1px. Ujung membulat. Angka persen memakai Space Grotesk di kanan batang.

## 9. Floating Dialog
Modal di L3: panel membulat 28px, bayangan paling besar dan lembut, latar di belakangnya digelapkan (bukan diburamkan). Masuk dengan spring dari bawah + skala 0,96 → 1.

## 10. Information Panel
Panel data: judul Space Grotesk, satu angka kunci besar, lalu baris label (Silver) dan nilai (Light Silver) tanpa garis pembatas tipis — jarak antar baris yang memisahkan.

## Elemen Set 3D

- **Properti low-poly**: bangunan, pohon, gunung, kendaraan dari bangun dasar; facet datar; sisi atas paling terang, sisi kanan paling gelap.
- **Karakter sederhana**: bentuk dasar terbaca dari jauh; satu warna aksen per karakter.
- **Penampang berlapis**: potongan tanah/lapisan yang memperlihatkan isi di bawah permukaan, jurus khas untuk menjelaskan proses dan kedalaman.
- **Duplikasi massal**: properti yang sama digandakan teratur untuk menunjukkan skala dan jumlah.
