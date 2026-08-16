# List (Daftar Urut)

**List** (atau di bahasa lain sering disebut *Array*) adalah jenis koleksi yang paling sering digunakan. Ia menyimpan sekumpulan data secara berurutan, layaknya sebuah antrean panjang.

**Analogi:** Bayangkan **List** sebagai **laci vertikal bersusun** di lemari kantor. Laci paling atas selalu diberi stiker nomor urut mutlak "Laci ke-0", laci di bawahnya "Laci ke-1", lalu "Laci ke-2", dan seterusnya. Setiap kali kamu memasukkan data baru, data itu otomatis diletakkan di laci urutan paling bawah yang masih kosong.

## Membuat List

Untuk membuat sebuah *List*, kita menggunakan tanda kurung siku `[]`.

```dart
// Membuat list berisi teks (String)
List<String> daftarSiswa = ['Budi', 'Ayu', 'Siti'];

// Membuat list berisi angka bulat (int)
List<int> daftarNilai = [80, 90, 75, 100];
```

## Memanggil dan Mengubah Data (Indeks)

Untuk memanggil isi suatu laci, panggil nama variabelnya diikuti nomor urut lacinya. 
Sangat penting untuk diingat: **Perhitungan laci komputer selalu dan mutlak dimulai dari angka 0, bukan 1.**

```dart
List<String> daftarSiswa = ['Budi', 'Ayu', 'Siti'];

// Memanggil data urutan pertama (Ayu)
print(daftarSiswa[1]); 

// Mengubah isi laci urutan pertama
daftarSiswa[1] = 'Joko';
print(daftarSiswa); // Hasilnya: [Budi, Joko, Siti]
```

## Menambah dan Menghapus Data

Dart menyediakan perintah-perintah bawaan canggih (*method*) untuk memanipulasi barisan data di dalam `List`.

- `add()`: Untuk menyuntikkan data baru secara paksa ke urutan ekor paling belakang.
- `remove()`: Untuk melacak dan menghapus langsung isi data yang disebutkan.
- `removeAt()`: Untuk memusnahkan laci beserta isinya berdasarkan nomor urut.

```dart
List<String> keranjangBelanja = ['Apel', 'Mangga'];

// Menambah data di belakang
keranjangBelanja.add('Pisang');

// Menghapus data spesifik
keranjangBelanja.remove('Mangga');

print(keranjangBelanja); // Hasil: [Apel, Pisang]
```
