# Quiz OOP Dasar

Uji pemahamanmu tentang pembuatan cetakan dan objek di Dart. Pilih jawaban yang paling tepat, lalu klik cek jawaban!

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>1. Dalam analogi pembuatan rumah, jika "Class" adalah gambar denah rumahnya, maka "Object" adalah?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="a"> a) Tukang bangunannya</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="b"> b) Bahan semen dan batanya</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="c"> c) Rumah fisik yang sudah jadi dan bisa ditinggali</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="d"> d) Izin mendirikan bangunannya</label></div>
  <button type="button" onclick="cekJawaban('q1')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q1" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>2. Variabel yang dibuat khusus di dalam sebuah Class untuk menyimpan data (seperti nama, warna, umur) disebut sebagai?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="a"> a) Properties</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="b"> b) Method</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="c"> c) Cascade</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="d"> d) Instansiasi</label></div>
  <button type="button" onclick="cekJawaban('q2')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q2" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>3. Apa ciri utama dari sebuah Constructor?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="a"> a) Selalu harus mengembalikan nilai angka.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="b"> b) Namanya bebas asal menggunakan awalan kata "get".</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="c"> c) Otomatis berjalan terakhir kali sebelum program ditutup.</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="d"> d) Namanya wajib sama persis dengan nama Class-nya.</label></div>
  <button type="button" onclick="cekJawaban('q3')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q3" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>4. Simbol apa yang digunakan untuk fitur Cascade Notation (memanggil banyak aksi secara beruntun tanpa mengulang nama objek)?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="a"> a) .</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="b"> b) ..</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="c"> c) -></label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="d"> d) ::</label></div>
  <button type="button" onclick="cekJawaban('q4')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q4" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>5. Jika class "Anjing" mewarisi class "Hewan", kata kunci apa yang wajib disematkan pada nama class Anjing?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="a"> a) class Anjing inherits Hewan</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="b"> b) class Anjing implements Hewan</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="c"> c) class Anjing extends Hewan</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="d"> d) class Anjing super Hewan</label></div>
  <button type="button" onclick="cekJawaban('q5')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q5" style="margin-top: 15px;"></div>
</div>

<script>
const quizData = {
  q1: {
    correct: 'c',
    explanations: {
      a: 'Pilihan ini salah. Tukang bangunan lebih mirip seperti fungsi utama (main) yang merangkai program.',
      b: 'Pilihan ini salah. Bahan material lebih mirip seperti tipe data dasar (int, String, bool).',
      c: '<strong>Tepat sekali!</strong> Object adalah hasil perwujudan fisik yang nyata dan sudah jadi (hidup di memori), yang dibuat berdasarkan panduan dari Class.',
      d: 'Pilihan ini salah. Izin bangunan tidak ada hubungannya dengan wujud nyata objek dalam pemrograman.'
    }
  },
  q2: {
    correct: 'a',
    explanations: {
      a: '<strong>Tepat sekali!</strong> Properties (atau atribut) adalah tempat kita mendeskripsikan sifat-sifat benda tersebut.',
      b: 'Pilihan <strong>Method</strong> salah. Method bukanlah penyimpan data, melainkan aksi/tindakan (fungsi) yang bisa dilakukan.',
      c: 'Pilihan <strong>Cascade</strong> salah. Itu adalah fitur penulisan titik ganda.',
      d: 'Pilihan <strong>Instansiasi</strong> salah. Itu adalah nama proses saat kita mencetak Object dari Class.'
    }
  },
  q3: {
    correct: 'd',
    explanations: {
      a: 'Pilihan ini salah. Constructor justru tidak boleh menggunakan kata kunci kembalian seperti int atau void.',
      b: 'Pilihan ini salah. Itu adalah aturan untuk fungsi (method) biasa.',
      c: 'Pilihan ini salah. Constructor berjalan di detik <strong>pertama</strong> objek dicetak, bukan terakhir.',
      d: '<strong>Tepat sekali!</strong> Aturan mutlak dari Constructor adalah namanya wajib persis sama dengan nama Class tempat ia berada.'
    }
  },
  q4: {
    correct: 'b',
    explanations: {
      a: 'Simbol <strong>.</strong> (titik tunggal) digunakan untuk memanggil satu aksi saja.',
      b: '<strong>Tepat sekali!</strong> Simbol <strong>..</strong> (titik ganda) digunakan untuk Cascade Notation agar kita bisa merangkai banyak aksi berturut-turut tanpa mengetik ulang nama objek.',
      c: 'Simbol <strong>-></strong> digunakan di bahasa C++ atau PHP, bukan di Dart.',
      d: 'Simbol <strong>::</strong> biasa dipakai di bahasa C++, bukan untuk fitur Cascade Dart.'
    }
  },
  q5: {
    correct: 'c',
    explanations: {
      a: 'Kata kunci <strong>inherits</strong> tidak ada dalam sintaks bahasa Dart.',
      b: 'Kata kunci <strong>implements</strong> memiliki arti berbeda, yaitu untuk menyalin kerangka kosong (Interface), bukan mewarisi sifat orang tua secara langsung.',
      c: '<strong>Tepat sekali!</strong> Kata kunci <strong>extends</strong> adalah sintaks resmi di Dart untuk mendefinisikan pewarisan sifat dari Parent Class ke Child Class.',
      d: 'Kata kunci <strong>super</strong> memang digunakan, tapi posisinya di dalam pemanggilan fungsi, bukan saat mendeklarasikan nama class.'
    }
  }
};

function cekJawaban(questionId) {
  const options = document.getElementsByName(questionId);
  let selectedValue = '';
  for (let i = 0; i < options.length; i++) {
    if (options[i].checked) { selectedValue = options[i].value; break; }
  }
  const feedbackDiv = document.getElementById('feedback-' + questionId);
  if (selectedValue === '') {
    feedbackDiv.innerHTML = '<span style="color: #e67e22; font-weight: bold;">Pilih jawaban terlebih dahulu.</span>';
    return;
  }
  const qData = quizData[questionId];
  const isCorrect = selectedValue === qData.correct;
  const penjelasanSpesifik = qData.explanations[selectedValue];
  let resultText = isCorrect ? '<span style="color: #27ae60; font-weight: bold; font-size: 1.1em;">Benar.</span><br>' : '<span style="color: #c0392b; font-weight: bold; font-size: 1.1em;">Salah.</span><br>';
  const explanationBox = '<div style="margin-top: 15px; padding: 15px; background-color: rgba(128, 128, 128, 0.1); border-left: 5px solid #2980b9; font-size: 0.95em; line-height: 1.5; color: inherit;">' + penjelasanSpesifik + '</div>';
  feedbackDiv.innerHTML = resultText + explanationBox;
}
</script>
