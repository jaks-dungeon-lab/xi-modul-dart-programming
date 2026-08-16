# Cascade Notation

Di bahasa Dart, ada sebuah fitur unik dan sangat berguna bernama **Cascade Notation** yang disimbolkan dengan titik ganda (`..`).

Fitur ini memungkinkan kita melakukan banyak perintah pada satu object yang sama secara beruntun ke bawah tanpa harus mengetik ulang nama object-nya berkali-kali.

**Analogi:** Seperti menyuruh asisten rumah tangga melakukan banyak pekerjaan.

- **Tanpa Cascade**: "Budi, sapu lantai. Budi, cuci piring. Budi, matikan lampu." (Melelahkan karena harus menyebut nama "Budi" terus menerus).
- **Dengan Cascade**: "Budi, tolong: sapu lantai, cuci piring, dan matikan lampu." (Jauh lebih singkat dan hemat kata-kata).

## Contoh Tanpa Cascade

Perhatikan bagaimana kita harus mengetik kata `kucingku` berulang kali di setiap baris.

```dart
void main() {
  var kucingku = Kucing();
  kucingku.nama = 'Oyen';
  kucingku.warna = 'Oranye';
  kucingku.makan();
  kucingku.tidur();
}
```

## Contoh Dengan Cascade (`..`)

Dengan titik ganda, kita langsung merangkai perintahnya ke bawah dan menyambungkannya. 

> **Penting**: Titik koma (`;`) penutup kode hanya diletakkan satu buah saja di akhir rangkaian.

```dart
void main() {
  var kucingku = Kucing()
    ..nama = 'Oyen'
    ..warna = 'Oranye'
    ..makan()
    ..tidur();
}
```

Kode menjadi jauh lebih bersih, mudah dibaca, dan lebih cepat untuk diketik!
