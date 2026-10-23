# BUILD-NOTE.md — Demo Kuningan Mega Bangunan

## Sumber data (publik, dari brief parent)
Semua data di bawah ini diteruskan dari parent agent dan diperlakukan sebagai data sumber publik; TIDAK ada yang ditambahkan/dikarang di sini.
- Nama, tagline, alamat (Jl. RE. Martadinata Dusun Puhun RT.016/RW.003, Ancaran, Kuningan 45514), jam (Senin–Minggu 08.00–20.00)
- Nomor/WA +62 812-1438-3951 dan link wa.me beserta teks pra-isi — disalin persis dari brief
- Kategori produk: Besi & baja (beton, siku, hollow, pipa, kanal); Semen; Pasir & split; Cat — dealer resmi Mowilex; Keramik & sanitair
- Profil: berdiri sejak 2010, lahan 2.000 m², 30+ staf, wilayah Cirebon–Indramayu–Majalengka–Kuningan
- Rating 4,7/5 Google Maps (312 ulasan) — ditampilkan dengan label sumber persis "312 ulasan di Google Maps"
- TikTok: @kuninganmegabangunan
- Link Google Maps search: https://www.google.com/maps/search/?api=1&query=Kuningan+Mega+Bangunan+Ancaran+Kuningan

## Yang TIDAK dimasukkan + alasan
- **Harga produk** — brief menandai [ISI MANUAL]; tidak dikarang. Semua posisi harga diganti dengan "Minta penawaran via WhatsApp" (R7: dilarang mengarang harga).
- **Testimoni/ulasan pelanggan** — tidak dibuat (R8: dilarang testimoni/ulasan karangan). Yang tampil hanya rating agregat 4,7/5 dengan label sumber "312 ulasan di Google Maps" — terverifikasi dan tidak diedit bentuknya.
- **Klaim promo/diskon/janji pengiriman** — tidak ada sumbernya; tidak dimasukkan.
- **Foto/gambar bisnis** — sengaja nol aset visual: seluruh visual dibangun dari gradasi CSS agar file 100% self-contained (persyaratan teknis).

## Catatan teknis
- Satu file `index.html` (10,9 KB), 100% self-contained: NOL request eksternal. Font = system stack, visual = gradasi CSS + repeating-linear-gradient (motif garis hazard industrial di hero), TANPA `<img>`, TANPA CDN/JS eksternal.
- Satu-satunya URL luar: `https://wa.me/6281214383951?...` (aksi WA, muncul 5x) dan `https://www.google.com/maps/search/?api=1&query=Kuningan+Mega+Bangunan+Ancaran+Kuningan` (maps, muncul 3x).
- Mobile-first, max-width 640px, konten centered. Sticky header (border bawah kuning safety) + tombol WA; sticky CTA bawah (WA + tombol maps) dengan `body{padding-bottom}` anti-tumpang.
- Hero: rating badge tampil di atas fold di antara tagline dan CTA; tombol "Tanya Stok & Harga" + "Lihat Lokasi" di atas fold.
- Palet: `--kuning:#ffc400` (safety yellow), `--hitam:#161616` (charcoal), putih — industrial, tegas, maskulin sesuai brief.
- Ikon: glyph unicode geometris (◆ ◷ ▶ ✉), BUKAN emoji (brief melarang emoji sebagai logo; logo = blok "KM" kuning solid).
- Footer jujur persis template waja-kopi: atribusi "Contoh website dibuat oleh Zenn — web designer Kuningan" + disclaimer "bukan situs resmi usaha".

## Belum diverifikasi / perlu cek parent
- Kebenaran isi data bisnis (nomor, jam, produk, rating) — hanya disalin dari brief, belum di-cross-check independen ke Maps/sumber publik oleh subagent ini.
- TIDAK di-deploy (instruksi: parent yang deploy).
