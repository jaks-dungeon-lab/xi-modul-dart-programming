# Effective Dart

Setiap bahasa pemrograman di dunia ini tentu memiliki budayanya, adatnya, atau gaya penulisannya sendiri. Sebuah baris program memang bisa saja berjalan lancar tanpa mengalami masalah error di mesin, namun bentuk tulisan kodenya mungkin akan terlihat "kacau" atau aneh bagi sesama mata programmer di ekosistem tersebut.

Untuk mencegah kekacauan ini, Google selaku pencipta Dart telah merilis sebuah panduan suci bernama **Effective Dart**. Panduan ini merangkum kumpulan aturan emas (*Best Practices*) agar kode Dart yang kamu tulis tidak hanya sanggup berjalan sukses, tapi juga sedap dipandang mata, rapi, bersih, dan sangat mudah untuk dilanjutkan oleh teman satu timmu di masa depan.

Berikut adalah beberapa petuah aturan paling mendasar yang mutlak wajib kamu jadikan pondasi:

## 1. Aturan Suci Penamaan (Naming Conventions)

Kesepakatan ini tidak boleh dilanggar agar kode yang ditulis banyak orang tetap terlihat seragam.

- **`PascalCase` (Setiap Huruf Depan Kata Wajib Kapital)**: Gunakan HANYA untuk penamaan **Class**, **Enum**, **Typedef**, dan **Extension**.
  > Benar: `class KucingLiar {}`
  > Salah: `class kucing_liar {}`

- **`camelCase` (Huruf Punggung Unta)**: Gunakan KHUSUS untuk penamaan **Variabel**, **Parameter Inputan**, dan **Method/Fungsi**. Kata pertama harus huruf kecil, tapi huruf depan kata kedua dan seterusnya harus besar.
  > Benar: `int jumlahRodaBelakang;`
  > Salah: `int JumlahRodaBelakang;`

- **`snake_case` (Ular Garis Bawah)**: Gunakan SANGAT SPESIFIK untuk penamaan **Nama File** di dalam file explorer sistem Windows/Mac (dan nama folder). Mesin Dart sangat membenci nama file yang dieja menggunakan spasi atau huruf besar.
  > Benar: `06-effective-dart.md`, `login_screen.dart`
  > Salah: `06 Effective Dart.md`, `LoginScreen.dart`

## 2. Bijak Menggunakan `var`, `final`, dan `const`

Jangan pernah sombong menggunakan penulisan tipe data eksplisit (seperti pemanggilan kata `String` atau `int`) jika tipe datanya sendiri sudah sangat jelas terlihat oleh mata manusia di baris kode saat itu juga. Biarkan mesin mengambil alih (*Type Inference*).

> Benar: `var sapaanNama = 'Budi';`
> Dihindari: `String sapaanNama = 'Budi';` (Tindakan membuang waktu karena bertele-tele)

Lebih dari hal tersebut, utamakanlah "mengunci" datamu sedini mungkin jika logikanya tidak perlu diubah lagi!
- Utamakan penggunaan **`final`** dibandingkan `var` jika nilai variabel tersebut baru didapat setelah suatu rumus diproses, dan ia tidak berencana akan diganti isinya lagi.
- Ubah menjadi status **`const`** jika nilai matematis variabel tersebut sudah abadi dan sudah bisa dinalar nilainya secara pasti (misalnya menetapkan angka konstanta gravitasi bumi, atau konfigurasi nomor warna layar) bahkan sebelum program dijalankan.

## 3. Tinggalkan Masa Lalu: String Interpolation (`$`)

Segera tinggalkan cara kuno (yang populer di bahasa Java tua) untuk merangkai dan menyambung teks menggunakan simbol operator tambah (`+`). Di Dart, kamu diperintahkan untuk menggunakan tanda dolar ajaib (`$`) yang disisipkan secara langsung menembus ke dalam teks.

> Benar: `print('Namaku $nama, umurku $umur');`
> Dihindari: `print('Namaku ' + nama + ', umurku ' + umur.toString());`

Menanamkan dan menerapkan budaya-budaya kode berkelas di atas sejak bangku sekolah akan menghindarkan dirimu dari kebiasaan buruk yang akan sangat memalukan sekaligus sulit diperbaiki saat kelak kamu terjun berkarir secara profesional di industri teknologi global!
