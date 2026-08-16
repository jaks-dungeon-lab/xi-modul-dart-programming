# Quiz Dart Dasar

Uji pemahamanmu sebelum melanjutkan ke materi Flutter! Pilih jawaban yang paling tepat, lalu klik tombol cek di bawah setiap pertanyaan. Kamu bisa mengubah jawaban jika mau.

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>1. Apa kata kunci yang digunakan jika kita ingin membuat variabel yang nilainya tidak boleh diubah selamanya?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="a"> a) var</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="b"> b) final</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="c"> c) String</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="d"> d) let</label></div>
  <button type="button" onclick="cekJawaban('q1')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q1" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>2. Manakah tipe data yang paling tepat untuk menyimpan bilangan pecahan atau desimal?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="a"> a) int</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="b"> b) bool</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="c"> c) double</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="d"> d) String</label></div>
  <button type="button" onclick="cekJawaban('q2')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q2" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>3. Simbol apa yang digunakan untuk memeriksa apakah dua buah angka sama nilainya?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="a"> a) =</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="b"> b) ==</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="c"> c) !=</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="d"> d) +</label></div>
  <button type="button" onclick="cekJawaban('q3')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q3" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>4. Jika kita ingin variabel `umur` diizinkan kosong (boleh bernilai `null`), bagaimana cara menuliskannya?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="a"> a) int null umur;</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="b"> b) int? umur;</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="c"> c) int! umur;</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="d"> d) int umur = null;</label></div>
  <button type="button" onclick="cekJawaban('q4')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q4" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>5. Apa kegunaan utama dari blok `try-catch`?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="a"> a) Untuk mengulang baris kode berkali-kali.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="b"> b) Untuk menampung banyak data ke dalam satu variabel.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="c"> c) Untuk menangkap error berbahaya agar program tidak mati mendadak.</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="d"> d) Untuk mendeklarasikan fungsi baru.</label></div>
  <button type="button" onclick="cekJawaban('q5')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q5" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>6. Simbol apa yang digunakan untuk membuat catatan satu baris yang akan diabaikan oleh komputer?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q6" value="a"> a) /*</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q6" value="b"> b) &lt;!--</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q6" value="c"> c) //</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q6" value="d"> d) **</label></div>
  <button type="button" onclick="cekJawaban('q6')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q6" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>7. Data masukan yang diberikan ke dalam sebuah fungsi agar bisa diproses disebut sebagai?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q7" value="a"> a) Return</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q7" value="b"> b) Parameter</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q7" value="c"> c) Scope</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q7" value="d"> d) Operator</label></div>
  <button type="button" onclick="cekJawaban('q7')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q7" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid #ddd; border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>8. Variabel yang dideklarasikan di dalam kurung kurawal sebuah fungsi disebut sebagai?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q8" value="a"> a) Variabel Global</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q8" value="b"> b) Variabel Lokal</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q8" value="c"> c) Variabel Tetap</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q8" value="d"> d) Variabel Kosong</label></div>
  <button type="button" onclick="cekJawaban('q8')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q8" style="margin-top: 15px;"></div>
</div>

<script>
const quizData = {
  q1: {
    correct: 'b',
    explanations: {
      a: '<strong>var</strong> digunakan untuk variabel biasa yang nilainya bisa diubah. Jadi pilihan ini kurang tepat.',
      b: '<strong>Tepat sekali!</strong> Kata kunci <strong>final</strong> (atau <strong>const</strong>) mengunci variabel agar nilainya tidak bisa diubah lagi.',
      c: '<strong>String</strong> adalah nama tipe data teks, bukan kata kunci untuk mengunci variabel.',
      d: '<strong>let</strong> adalah kata kunci di bahasa pemrograman lain (seperti JavaScript), bukan di Dart dasar.'
    }
  },
  q2: {
    correct: 'c',
    explanations: {
      a: '<strong>int</strong> hanya bisa menampung angka bulat tanpa koma.',
      b: '<strong>bool</strong> digunakan untuk nilai logika benar atau salah (true/false).',
      c: '<strong>Tepat sekali!</strong> Tipe data <strong>double</strong> dirancang khusus untuk menyimpan angka desimal atau pecahan.',
      d: '<strong>String</strong> digunakan khusus untuk teks atau kalimat, bukan untuk angka desimal.'
    }
  },
  q3: {
    correct: 'b',
    explanations: {
      a: 'Simbol <strong>=</strong> (sama dengan tunggal) adalah operator penugasan untuk memasukkan data ke variabel.',
      b: '<strong>Tepat sekali!</strong> Simbol <strong>==</strong> adalah operator perbandingan yang menghasilkan nilai benar jika angka di kiri dan kanan sama.',
      c: 'Simbol <strong>!=</strong> justru digunakan untuk memeriksa ketidaksamaan (tidak sama dengan).',
      d: 'Simbol <strong>+</strong> adalah operator aritmatika untuk menjumlahkan angka.'
    }
  },
  q4: {
    correct: 'b',
    explanations: {
      a: 'Penulisan tipe data <strong>null</strong> secara eksplisit di tengah tidak dikenali oleh Dart.',
      b: '<strong>Tepat sekali!</strong> Dalam sistem Null Safety Dart, tanda tanya (<strong>?</strong>) tepat di sebelah tipe data memberitahu program bahwa variabel tersebut diizinkan kosong (null).',
      c: 'Tanda seru (<strong>!</strong>) digunakan untuk memaksa program percaya bahwa nilainya pasti TIDAK kosong, bukan sebaliknya.',
      d: 'Menugaskan dengan <strong>= null</strong> secara langsung tanpa tanda tanya di tipe datanya akan ditolak keras oleh sistem Null Safety.'
    }
  },
  q5: {
    correct: 'c',
    explanations: {
      a: 'Untuk mengulang baris kode, kita menggunakan perulangan seperti <strong>for</strong> atau <strong>while</strong>.',
      b: 'Untuk menampung banyak data, kita menggunakan tipe data Collections seperti <strong>List</strong>.',
      c: '<strong>Tepat sekali!</strong> Blok try-catch bekerja seperti sabuk pengaman yang menangkap error agar program tidak tertutup paksa (crash).',
      d: 'Untuk mendeklarasikan fungsi baru, kita cukup menuliskan tipe kembalian, nama fungsi, dan kurung kurawal tanpa try-catch.'
    }
  },
  q6: {
    correct: 'c',
    explanations: {
      a: 'Simbol <strong>/*</strong> digunakan untuk memulai komentar banyak baris, bukan satu baris.',
      b: 'Simbol <strong>&lt;!--</strong> digunakan untuk membuat komentar di dalam bahasa HTML, bukan Dart.',
      c: '<strong>Tepat sekali!</strong> Simbol garis miring ganda (<strong>//</strong>) akan membuat seluruh sisa baris diabaikan oleh komputer.',
      d: 'Simbol <strong>**</strong> tidak memiliki fungsi komentar khusus di bahasa Dart.'
    }
  },
  q7: {
    correct: 'b',
    explanations: {
      a: '<strong>Return</strong> merujuk pada hasil akhir yang dikembalikan atau dikeluarkan oleh fungsi tersebut.',
      b: '<strong>Tepat sekali!</strong> Parameter adalah data mentah yang kita masukkan ke dalam kurung fungsi saat memanggilnya agar bisa diproses di dalam mesin fungsi.',
      c: '<strong>Scope</strong> (ruang lingkup) adalah batas wilayah di mana sebuah variabel bisa dibaca oleh program.',
      d: '<strong>Operator</strong> adalah simbol matematika atau logika (seperti +, -, ==).'
    }
  },
  q8: {
    correct: 'b',
    explanations: {
      a: 'Variabel Global adalah variabel yang dibuat di LUAR semua fungsi, sehingga bisa diakses secara bebas dari mana saja.',
      b: '<strong>Tepat sekali!</strong> Variabel di dalam kurung kurawal fungsi bersifat lokal, artinya ruang lingkupnya terbatas dan tidak bisa dikenali dari luar fungsi tersebut.',
      c: 'Variabel Tetap lebih cocok merujuk pada variabel yang menggunakan kata kunci final/const, bukan soal letaknya di dalam fungsi.',
      d: 'Variabel Kosong merujuk pada variabel yang bernilai null, tidak ada hubungannya dengan posisi pembuatan variabel di dalam fungsi.'
    }
  }
};

function cekJawaban(questionId) {
  const options = document.getElementsByName(questionId);
  let selectedValue = '';
  
  for (let i = 0; i < options.length; i++) {
    if (options[i].checked) {
      selectedValue = options[i].value;
      break;
    }
  }
  
  const feedbackDiv = document.getElementById('feedback-' + questionId);
  
  if (selectedValue === '') {
    feedbackDiv.innerHTML = '<span style="color: #e67e22; font-weight: bold;">Pilih jawaban terlebih dahulu.</span>';
    return;
  }
  
  const qData = quizData[questionId];
  const isCorrect = selectedValue === qData.correct;
  const penjelasanSpesifik = qData.explanations[selectedValue];
  
  let resultText = '';
  if (isCorrect) {
    resultText = '<span style="color: #27ae60; font-weight: bold; font-size: 1.1em;">Benar.</span><br>';
  } else {
    resultText = '<span style="color: #c0392b; font-weight: bold; font-size: 1.1em;">Salah.</span><br>';
  }
  
  const explanationBox = '<div style="margin-top: 15px; padding: 15px; background-color: rgba(128, 128, 128, 0.1); border-left: 5px solid #2980b9; font-size: 0.95em; line-height: 1.5; color: inherit;">' + penjelasanSpesifik + '</div>';
  
  feedbackDiv.innerHTML = resultText + explanationBox;
}
</script>
