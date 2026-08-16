# Enums (Enumeration)

**Enums** adalah tipe data khusus yang isinya berupa sekumpulan pilihan yang sudah kita tentukan secara pasti sejak awal. 

Kita menggunakannya saat kita punya daftar opsi yang nilainya tetap, mutlak, dan tidak akan pernah bertambah secara acak (misalnya: nama hari, arah mata angin, atau tingkat kesulitan).

**Analogi:** Seperti kamu sedang memilih ukuran baju di toko. Pilihannya hanya ada S, M, L, atau XL. Kamu tidak bisa tiba-tiba memesan ukuran baju yang bernama "Raksasa". Enums memastikan bahwa pilihan yang kamu masukkan ke dalam program tidak akan pernah melenceng keluar dari daftar resmi.

## Cara Menggunakan Enum

Gunakan kata kunci `enum` diikuti dengan nama tipenya, lalu tuliskan opsi-opsinya di dalam kurung kurawal.

```dart
// 1. Mendefinisikan Enum di luar fungsi main
enum TingkatKesulitan {
  mudah,
  normal,
  susah
}

void main() {
  // 2. Menggunakan Enum
  var kesulitanGame = TingkatKesulitan.normal;
  
  // Mengecek nilai enum menggunakan if
  if (kesulitanGame == TingkatKesulitan.susah) {
    print('Kamu memilih mode Susah. Bersiaplah!');
  } else {
    print('Mode santai, nikmati permainannya.');
  }
}
```

## Keuntungan Enum

Penggunaan enum akan sangat menekan risiko terjadinya *typo* (salah ketik *bug*) jika dibandingkan dengan menggunakan tipe teks (String) biasa untuk pengecekan kondisi (seperti `'Mudah'` huruf M besar berlawanan dengan `'mudah'` huruf kecil, yang seringkali menyebabkan program rusak secara tidak terduga).
