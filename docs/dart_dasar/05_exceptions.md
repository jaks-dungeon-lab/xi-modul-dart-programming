# Exceptions (Penanganan Error)

Saat program berjalan, terkadang ada kesalahan (error) fatal yang tidak terduga, misalnya mencoba membagi angka dengan nol atau mengambil data yang tidak ada. Jika dibiarkan, program akan *crash* (berhenti paksa dan keluar sendiri).

**Analogi:** Bayangkan kamu sedang mengendarai motor dan tiba-tiba ban bocor. Jika kamu tidak punya rencana cadangan (bawa alat penambal atau tahu nomor bengkel), perjalananmu akan berhenti total (*crash*). `try-catch` adalah alat penambal tersebut.

## Menggunakan Try-Catch

Gunakan blok `try` untuk menaruh kode yang berisiko error, dan blok `catch` untuk menangkap dan menangani errornya tanpa membuat aplikasi tertutup.

```dart
void main() {
  try {
    int angka = 10;
    int hasil = angka ~/ 0; // Error! Tidak bisa membagi dengan 0
    print(hasil);
  } catch (e) {
    // Kalau ada error di dalam blok try, kode ini yang dijalankan
    print('Terjadi kesalahan: Angka tidak bisa dibagi dengan nol.');
  } finally {
    // Blok ini akan SELALU dieksekusi, entah itu sukses atau error
    print('Operasi perhitungan selesai.');
  }
}
```

### Kapan Menggunakan `finally`?
Blok `finally` sangat berguna ketika kita ingin menjalankan kode pembersihan (*cleanup*), seperti mematikan ikon *loading* di layar, menutup koneksi database, atau menghapus *file* sementara. Baik programnya berhasil maupun berujung *error*, kita tetap ingin ikon *loading* tersebut berhenti berputar!
