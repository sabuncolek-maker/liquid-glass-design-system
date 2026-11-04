---
name: lapis-design-system
description: Design system 2.5D berlapis + 3D low-poly milik Erlangga (Silver × Hitam × Biru Elektrik, Space Grotesk + Inter). Pakai saat membuat video motion graphics, UI, atau visual apa pun yang diminta mengikuti sistem ini.
---

# LAPIS — Design System 2.5D & 3D

Sebelum bekerja, baca `DESIGN-SYSTEM.md` di repo ini sampai selesai. Itu hukumnya. Ringkasan yang mengikat:

- **Gaya**: 2.5D berlapis (panel bertumpuk, bayangan lembut, parallax) dan set 3D low-poly dari bangun dasar. Bukan kaca, bukan blur tembus pandang, bukan sudut angular.
- **Warna**: Electric Blue #0D6EFD, Silver #C0C4CC, Deep Black #0B0B0D; pendukung Dark Navy #080E1B, Panel Deep #18243A, Light Silver #E2E7F0, Cyan Glow #00CFFF (cahaya aksen saja). Distribusi 50% hitam/navy, 25% silver, 15% biru, 10% putih/cyan.
- **Kedalaman**: empat tingkat L0–L3 dengan bayangan dan faktor parallax sesuai tabel di DESIGN-SYSTEM.md. Satu sumber cahaya dari kiri atas: sisi atas paling terang, sisi kanan paling gelap.
- **Geometri**: sudut membulat halus (radius 10/18/28px). Pil penuh hanya untuk toggle dan chip bulat.
- **Font**: Space Grotesk untuk heading, Inter untuk body. Maksimal dua keluarga.
- **Komponen**: pakai 10 komponen reusable dari `components/COMPONENTS.md`; jangan mengarang komponen baru tanpa kebutuhan nyata.
- **Motion**: spring melenting halus, elemen melayang dan bernapas, parallax saat kamera bergerak, transisi lewat geseran lapisan. Dilarang easing linear dan fade polos tanpa gerak.
- **Komposisi**: Opening bertingkat → Main Content satu fokus → Transisi lapisan → Closing memusat.

Urutan kerja wajib: baca design system → ambil tokens → pakai komponen → storyboard → animatic/preview → final → cek konsistensi (warna, font, lapisan, cahaya, gerak). Konsistensi lebih penting daripada dekorasi; jangan mengorbankan keterbacaan.
