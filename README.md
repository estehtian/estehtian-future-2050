# Esteh Tian Future 2050

Website statis multi-halaman untuk GitHub Pages. Tidak membutuhkan hosting berbayar, framework, build tools, atau database.

## Isi folder
- `index.html` — Beranda
- `produk.html` — Katalog dan demo keranjang
- `tentang.html` — Profil/cerita merek
- `kontak.html` — Kontak dan FAQ
- `assets/css/style.css` — Tampilan responsif, warna, animasi
- `assets/js/config.js` — **Edit produk, harga, WhatsApp, Instagram, dan alamat di sini**
- `assets/js/script.js` — Interaksi menu, filter, keranjang, dan persiapan pesan
- `assets/images/favicon.svg` — Ikon tab browser

## Cara memasang ke repositori GitHub
1. Unduh ZIP ini lalu ekstrak di komputer.
2. Buka repositori GitHub yang saat ini menerbitkan website.
3. Pastikan Anda berada pada branch dan folder publikasi yang benar (umumnya branch `main`, folder `/ (root)`; cek **Settings → Pages**).
4. Unggah semua file dan folder dari isi ZIP ke lokasi publikasi tersebut. Jangan mengunggah folder pembungkus `esteh-tian-future-2050` jika Pages menerbitkan dari root; unggah isi foldernya.
5. Jika `index.html` yang lama penting, simpan salinan lokal dahulu. Periksa perubahan sebelum melakukan commit.
6. Commit changes, tunggu workflow/deployment Pages selesai, lalu buka situs Anda dan uji setiap menu.
7. Jangan mengubah DNS yang sudah berhasil. Perubahan file website tidak memerlukan perubahan DNS.

## Atur data bisnis
Edit `assets/js/config.js`:
- `whatsapp`: isi nomor WhatsApp bisnis dengan kode negara 62, tanpa `+`, spasi, atau tanda hubung. Contoh format `6281234567890` hanyalah format contoh, bukan nomor untuk dipakai.
- `instagram`: nama akun tanpa `@`.
- `address`: alamat yang benar.
- `products`: ubah `name`, `category`, `price`, `description`, `badge`, `visual`, dan `emoji`. Harga dalam angka Rupiah, misalnya `10000`.

**Penting:** enam menu dan harganya masih contoh. Sesuaikan dengan menu, harga, dan foto produk yang benar sebelum menerima pesanan. Ilustrasi gelas dibuat menggunakan CSS; belum memakai foto produk asli.

## Pemesanan
Keranjang demo berjalan di browser. Setelah nomor WhatsApp diisi, tombol checkout membuka WhatsApp dengan daftar menu dan total sementara. Tidak ada pembayaran online, inventori, database, atau penyimpanan order otomatis. Pesanan baru dikirim jika pelanggan menekan tombol kirim di WhatsApp.

## Pengujian singkat
- Buka `index.html`, navigasi Menu/Tentang/Kontak.
- Di Menu, filter kategori, tambah/kurangi jumlah, cek total.
- Sebelum nomor WhatsApp diatur, checkout akan memberi pesan bahwa konfigurasi belum lengkap.
- Setelah nomor diatur, uji link WhatsApp menggunakan nomor bisnis Anda sendiri.
- Uji tampilan desktop dan mobile serta HTTPS.

## Catatan
- Website ini adalah frontend statis. Jangan menaruh kata sandi, token rahasia, atau data pelanggan dalam file JavaScript.
- Harga, menu, alamat, akun sosial, dan klaim bisnis harus diverifikasi pemilik.


## Halaman tambahan Future 2050

Paket ini juga menyertakan halaman: `promo.html`, `galeri.html`, `pemesanan.html`, `cerita.html`, `lokasi.html`, dan `faq.html`. Keenam halaman tersebut sudah ditautkan melalui menu dropdown **Lainnya** di seluruh halaman utama. Gaya dropdown dan komponen tambahan berada di akhir `assets/css/style.css`.

Sebelum dipublikasikan, ganti harga contoh, isi kontak/alamat yang benar pada `assets/js/config.js`, dan ganti ilustrasi galeri dengan foto produk yang Anda miliki hak penggunaannya. DNS dan pengaturan GitHub Pages tidak perlu diubah.
