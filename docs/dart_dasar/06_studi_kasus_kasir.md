# Studi Kasus: Aplikasi Kasir Sederhana

Mari kita gabungkan apa yang sudah kita pelajari (Variabel, Tipe Data, dan Operator) untuk membuat logika program mesin kasir sangat sederhana.

**Skenario:**
Seorang pelanggan membeli sepatu dan tas. Toko memberikan potongan harga (diskon). Kita harus menghitung total harga yang harus dibayar dan menentukan berapa kembalian yang harus diberikan oleh kasir.

```dart
void main() {
  // 1. Tentukan harga barang
  int hargaSepatu = 150000;
  int hargaTas = 200000;
  
  // 2. Hitung total belanja awal
  int totalBelanja = hargaSepatu + hargaTas;
  print('Total belanja: Rp $totalBelanja');
  
  // 3. Tentukan diskon tetap
  int diskon = 50000;
  print('Diskon hari ini: Rp $diskon');
  
  // 4. Hitung harga akhir yang harus dibayar pelanggan
  int hargaAkhir = totalBelanja - diskon;
  print('Harus dibayar: Rp $hargaAkhir');
  
  // 5. Pelanggan menyerahkan uang
  int uangPelanggan = 400000;
  print('Uang yang dibayarkan: Rp $uangPelanggan');
  
  // 6. Hitung kembalian
  int kembalian = uangPelanggan - hargaAkhir;
  print('Kembalian Anda: Rp $kembalian');
}
```

Cobalah salin kode di atas ke [DartPad](https://dartpad.dev) dan jalankan. Ubah harga barang atau besaran diskon untuk melihat langsung bagaimana operator bekerja memproses angka yang baru!
