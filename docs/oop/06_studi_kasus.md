# Studi Kasus: Bengkel Kendaraan

Mari kita praktikkan gabungan konsep Class, Properties, Method, Constructor, dan Inheritance ke dalam sebuah program simulasi bengkel kendaraan yang rapi.

## Skenario

Sebuah bengkel mendata kendaraan pelanggan secara umum berdasarkan **merek** dan **tahun pembuatannya**. Semua kendaraan memiliki fitur standar untuk **menyalakan mesin**. 

Namun, bengkel ini juga menerima spesifikasi khusus untuk **Mobil** dan **Motor** yang punya ciri khas masing-masing:
- Mobil memiliki properti khusus yaitu `jumlahPintu` dan fungsi `bukaPintu()`.
- Motor memiliki fungsi khusus yaitu `standarSamping()`.

## Kode Program

Salin dan jalankan kode berikut di [DartPad](https://dartpad.dev).

```dart
// 1. Parent Class (Cetakan Utama)
class Kendaraan {
  String merek;
  int tahun;
  
  // Constructor Utama
  Kendaraan({required this.merek, required this.tahun});
  
  // Method umum
  void nyalakanMesin() {
    print('Mesin $merek keluaran tahun $tahun menyala: Vrooom!');
  }
}

// 2. Child Class 1: Mobil
class Mobil extends Kendaraan {
  int jumlahPintu;
  
  // Menggunakan sintaks modern super.merek dan super.tahun untuk melempar data ke Parent Class
  Mobil({required super.merek, required super.tahun, required this.jumlahPintu});
    
  void bukaPintu() {
    print('$merek membuka salah satu dari $jumlahPintu pintunya.');
  }
}

// 3. Child Class 2: Motor
class Motor extends Kendaraan {
  bool adaGigi;
  
  Motor({required super.merek, required super.tahun, required this.adaGigi});
    
  void standarSamping() {
    print('Menurunkan standar samping motor $merek.');
  }
}

void main() {
  // Menggunakan Cascade Notation (..) untuk mengeksekusi banyak perintah secara instan
  var mobilPelanggan = Mobil(merek: 'Toyota', tahun: 2022, jumlahPintu: 4)
    ..nyalakanMesin()
    ..bukaPintu();
    
  print('---');
  
  var motorPelanggan = Motor(merek: 'Honda', tahun: 2021, adaGigi: false)
    ..standarSamping()
    ..nyalakanMesin();
}
```

## Penjelasan Singkat

1. `Kendaraan` adalah cetak biru utama yang menyimpan informasi umum.
2. `Mobil` dan `Motor` mewarisi `Kendaraan` (`extends Kendaraan`). Berkat pewarisan ini, kita tidak perlu lagi repot-repot menulis ulang properti `merek` dan `tahun` di dalam cetakan Mobil dan Motor dari awal.
3. Saat membuat objek Mobil, kita memberikan nilai *merek* dan *tahun* kepada instruksi `super(...)` agar data tersebut dilempar dan disimpan di brankas Parent Class.
