# Studi Kasus Kasir dengan Control Flow

Mari kita tingkatkan aplikasi kasir kita dari bab sebelumnya dengan menambahkan **Control Flow** (`if-else`). Kali ini, program akan menjadi lebih cerdas karena bisa mengambil keputusan secara otomatis.

**Skenario:**
Jika total belanja pelanggan melebihi Rp 100.000, maka ia berhak mendapatkan diskon 10%. Selain itu, kasir juga akan secara otomatis memeriksa apakah uang tunai yang diserahkan pelanggan cukup, kurang, atau pas.

```dart
void main() {
  int totalBelanja = 120000;
  int uangPelanggan = 150000;
  
  // 1. Cek apakah pelanggan berhak mendapat diskon
  if (totalBelanja > 100000) {
    print('Selamat! Anda mendapatkan diskon 10%');
    
    // Simbol ~/ adalah pembagian dengan hasil bilangan bulat
    int jumlahDiskon = (totalBelanja * 10) ~/ 100;
    totalBelanja = totalBelanja - jumlahDiskon;
  }
  
  print('Total yang harus dibayar: Rp $totalBelanja');
  
  // 2. Cek apakah uang pembayaran cukup
  if (uangPelanggan > totalBelanja) {
    int kembalian = uangPelanggan - totalBelanja;
    print('Pembayaran sukses. Kembalian: Rp $kembalian');
  } else if (uangPelanggan == totalBelanja) {
    print('Pembayaran sukses. Uang pas.');
  } else {
    // Kondisi jika uangPelanggan < totalBelanja
    int uangKurang = totalBelanja - uangPelanggan;
    print('Maaf, uang Anda kurang Rp $uangKurang');
  }
}
```

Cobalah salin kode di atas ke [DartPad](https://dartpad.dev). Coba bereksperimen dengan mengubah nilai `totalBelanja` menjadi `50000` (agar tidak dapat diskon) atau mengubah `uangPelanggan` menjadi `100000` (agar muncul pesan uang kurang). Amati bagaimana program otomatis berbelok mengubah nasib sesuai dengan nilai variabel yang kamu berikan!
