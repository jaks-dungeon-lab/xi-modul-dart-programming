# Rangkuman Collections

Kamu telah menyelami ketiga bentuk perabot penyimpan data massal (*Collections*) utama di dalam bahasa Dart. Penggunaan ketiganya harus disesuaikan mutlak dengan jenis masalah yang sedang kamu selesaikan.

## Intisari Materi

Berikut adalah rumus cepat untuk membantu otakmu memilih wadah koleksi yang tepat saat merancang arsitektur kode di masa depan:

- **Collections**: Secara umum adalah istilah sebutan keranjang bagi sistem penyimpanan sekumpulan kelompok data menjadi satu kesatuan *variabel* wadah bernaung.
- **List**: Gunakan ini jika urutan sangat penting. Cocok dipakai ketika datamu diurutkan secara berderet seperti antrean loket kasir dan diakses berdasar nomor urut (`indeks`). Ia diizinkan menyimpan data kembar. Dibuat menggunakan kurung siku `[]`.
- **Map**: Gunakan ini jika kamu butuh memanggil data menggunakan pelabelan nama yang jelas (struktur pasangan Kunci-Nilai). Cocok digunakan sebagai struktur buku telepon, nomor identitas berpasangan dengan nama, dsb. Kunci (*Key*) tidak boleh ganda, namun Nilai (*Value*) boleh berulang. Dibuat menggunakan kurung kurawal berpasangan `{Kunci: Nilai}`.
- **Set**: Gunakan ini jika kamu menginginkan data mentah yang sangat bersih dari duplikat. Cocok dipakai untuk menampung riwayat data absensi acak di mana satu siswa tidak boleh dihitung hadir ganda. Dibuat menggunakan kurung kurawal nilai tunggal `{}`.
