# LAPIS — Design System 2.5D & 3D v1.0

Silver × Black × Electric Blue — Layered 2.5D + Low-Poly 3D — Space Grotesk + Inter

Sistem desain milik Erlangga untuk video motion graphics dan UI. Gayanya gambar berlapis yang terasa punya kedalaman (2.5D) dan set 3D low-poly sederhana. Sifat wajibnya dua: **hidup** dan **nyaman di mata**.

---

## 1. Prinsip

1. **Kedalaman dari lapisan, bukan dari kaca.** Panel bertumpuk dengan bayangan lembut. Tidak ada material kaca, tidak ada blur tembus pandang sebagai identitas.
2. **Hidup.** Tidak ada elemen yang mati diam. Semua bergerak halus: melayang, bernapas, atau menyambut dengan pegas. Tapi gerak tidak pernah ribut.
3. **Nyaman di mata.** Desain pakai rem, bukan gas. Kalau elemen bisa dibuang tanpa mengurangi pesan, buang. Satu aksen dominan per momen.
4. **Konsistensi di atas dekorasi.** Sistem yang sama di semua scene lebih penting daripada efek sesaat.

## 2. Warna

| Token | Hex | Peran |
| --- | --- | --- |
| Electric Blue | #0D6EFD | Aksen utama: CTA, sorotan, fokus |
| Silver | #C0C4CC | Permukaan panel, teks sekunder, sisi terang |
| Deep Black | #0B0B0D | Latar utama |
| Dark Navy | #080E1B | Latar gradasi, langit scene 3D |
| Panel Deep | #18243A | Isi panel tingkat dasar |
| Light Silver | #E2E7F0 | Teks utama di atas gelap, sisi paling terang |
| White | #FFFFFF | Teks judul |
| Cyan Glow | #00CFFF | Cahaya aksen saja, tidak untuk isi |

Distribusi: **50% hitam/navy · 25% silver · 15% biru · 10% putih/cyan.** Jangan tampilkan semua warna dengan intensitas sama.

## 3. Kedalaman (inti 2.5D)

Empat tingkat lapisan:

| Tingkat | Isi | Bayangan (offset-y / blur / opacity) | Faktor parallax |
| --- | --- | --- | --- |
| L0 Latar | gradasi, blob cahaya, set jauh | tanpa bayangan | 0,2 |
| L1 Permukaan | panel dasar, tanah, panggung | 10px / 24px / 25% | 0,5 |
| L2 Terangkat | kartu, tombol, panel info | 18px / 36px / 30% | 0,8 |
| L3 Melayang | dialog, elemen hero, karakter | 28px / 54px / 35% | 1,0 |

Aturan kedalaman:

- Bayangan selalu jatuh ke bawah, lembut, satu arah. Tidak ada bayangan keras.
- Saat kamera bergerak, lapisan jauh bergerak lebih lambat (parallax sesuai faktor di atas).
- Set 3D memakai sudut isometric ±30°.
- Satu sumber cahaya: dari kiri atas. Sisi atas benda paling terang, sisi kiri sedang, sisi kanan paling gelap. Berlaku untuk semua facet low-poly.

## 4. Geometri

- Sudut **membulat halus**: radius kecil 10px, sedang 18px, besar 28px. Pil penuh hanya untuk toggle dan chip bulat.
- Dilarang: sudut potong angular/chamfer, tepi kaca, garis outline tipis bercahaya.
- Bentuk 3D dari bangun dasar (kotak, prisma, kerucut, tabung) dengan facet datar low-poly.

## 5. Tipografi

- Heading: **Space Grotesk** (700/600/500).
- Body: **Inter** (400/500/600).
- Maksimal dua keluarga font. Hindari kapital penuh untuk semua teks; kapital hanya untuk label pendek.

## 6. Komponen

Sepuluh komponen reusable, dirinci di `components/COMPONENTS.md`:

1. Layered Panel — panel berlapis L1/L2
2. Depth Card — kartu dengan sisi tebal 2.5D
3. Primary Button — biru penuh, terangkat
4. Secondary Button — permukaan silver gelap, terangkat
5. Navigation Bar — bar L2 melayang di atas latar
6. Icon Button — tombol ikon membulat
7. Toggle Switch — pil dengan knob bergeser pegas
8. Progress Indicator — batang berlapis dengan sisi terang
9. Floating Dialog — modal L3, bayangan besar lembut
10. Information Panel — panel data dengan baris label/nilai

Elemen set 3D: properti low-poly (bangunan, pohon, gunung, kendaraan sederhana), karakter sederhana, dan penampang berlapis (potongan tanah/lapisan bumi) sebagai jurus khas menjelaskan isi.

## 7. Motion — bahasa gerak hidup

- **Pegas melenting halus**: elemen masuk dengan spring redaman rendah, berhenti dengan sedikit overshoot, bukan berhenti mati.
- **Melayang & bernapas**: elemen hero melayang ±4–8px dengan siklus 3–5 detik; cahaya latar berdenyut pelan.
- **Parallax**: setiap gerakan kamera menggerakkan lapisan sesuai faktornya.
- **Transisi melebur antar lapisan**: scene berganti lewat geseran lapisan dan parallax, bukan potongan fade polos.
- Durasi: micro 150–250ms · transisi UI 300–500ms · panel reveal 500–800ms · transisi scene 600–1000ms.
- Dilarang: easing linear, gerak patah-patah, fade tanpa gerak, efek berlebihan yang mengorbankan keterbacaan.

## 8. Komposisi scene

Opening (latar masuk bertingkat dari L0 ke L3, cahaya menyala pelan) → Main Content (satu fokus per scene) → Visual Transition (geser lapisan/parallax) → Closing (komposisi memusat, satu kalimat penutup, cahaya meredup bersih).

## 9. Konsistensi

Wajib dipertahankan: palet, font, tingkat lapisan, arah cahaya, bahasa gerak, komponen reusable.
Dilarang: mengganti warna utama, font dekoratif, gradasi acak, material kaca, sudut angular, glow berlebihan, elemen dekoratif tanpa fungsi, desain berbeda di tiap scene.

## 10. Urutan kerja agent

Baca design system ini → ambil design tokens → pakai komponen reusable → storyboard → animatic/preview → final → cek konsistensi (warna, font, lapisan, cahaya, gerak).
