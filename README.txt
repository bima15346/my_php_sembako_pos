SEMBAKO POS - PROTOTIPE AWAL

FITUR
- Login satu akun pemilik
- Dashboard ringkasan penjualan dan stok rendah
- Kasir grid produk, pencarian, kategori, keranjang, pembayaran tunai/QRIS/transfer
- Pengelolaan produk, harga modal/jual, stok dan batas minimum
- Riwayat 100 transaksi terbaru
- Laporan ringkas laba kotor dan pencatatan pengeluaran
- Ganti password
- Layout responsive desktop, tablet, dan HP

CARA MENJALANKAN DI XAMPP
1. Ekstrak folder sembako_pos ke C:\xampp\htdocs\sembako_pos
2. Buka XAMPP Control Panel, nyalakan Apache dan MySQL.
3. Buka http://localhost/sembako_pos/setup.php
4. Jika setup berhasil, buka http://localhost/sembako_pos/index.php
5. Login awal:
   Username: pemilik
   Password: GantiSaya123!
6. Segera ganti password dari menu Pengaturan.
7. Setelah setup berhasil, hapus setup.php atau ubah nama file tersebut.

PENGATURAN DATABASE
Default XAMPP: host localhost, database sembako_pos, user root, password kosong.
Jika konfigurasi MySQL berbeda, ubah variabel koneksi di bagian atas setup.php dan index.php.

CATATAN PENTING
Ini adalah MVP/prototipe yang dapat dijalankan, bukan sistem produksi yang sudah diaudit.
- QRIS dan transfer belum terintegrasi dengan penyedia pembayaran; status dicatat manual oleh operator.
- Belum ada retur, hutang pelanggan/supplier, pembelian supplier, konversi satuan kemasan, dan ekspor laporan.
- Belum ada token CSRF pada seluruh form, pembatasan percobaan login, pencatatan audit penuh, serta mekanisme backup otomatis.
- Sebelum diunggah ke internet, implementasikan perlindungan keamanan tambahan, HTTPS, password database kuat, backup rutin, dan uji keamanan.
- Bootstrap dimuat dari CDN sehingga koneksi internet dibutuhkan untuk tampilan styling.
