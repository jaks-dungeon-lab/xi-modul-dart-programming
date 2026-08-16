# Quiz Futures

Uji pemahamanmu tentang materi Asynchronous Programming sebelum melanjutkan ke dunia Flutter! Pilih jawaban yang paling tepat, lalu klik tombol cek di bawah setiap pertanyaan.

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>1. Apa kelemahan utama jika aplikasimu berjalan murni secara Synchronous saat mengunduh file besar?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="a"> a) Kecepatan internet Wi-Fi menjadi jauh lebih lambat.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="b"> b) Layar aplikasi akan macet total (freeze) dan tidak bisa disentuh.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="c"> c) File yang diunduh pasti mengalami kerusakan data (corrupt).</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="d"> d) Program akan otomatis tertutup sendiri.</label></div>
  <button type="button" onclick="cekJawaban('q1')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q1" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>2. Tipe data mutlak apa yang SELALU dikembalikan oleh sebuah fungsi asynchronous di Dart?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="a"> a) Tipe data String</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="b"> b) Tipe data dynamic</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="c"> c) Objek bertipe List</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="d"> d) Objek bertipe Future</label></div>
  <button type="button" onclick="cekJawaban('q2')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q2" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>3. Fase status apa yang otomatis disematkan pada objek Future pada detik pertama saat kamu BARU SAJA memanggil fungsinya?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="a"> a) Completed with Data</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="b"> b) Uncompleted</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="c"> c) Completed with Error</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="d"> d) Loading</label></div>
  <button type="button" onclick="cekJawaban('q3')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q3" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>4. Apa fungsi utama yang diemban oleh kata kunci sakti 'await'?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="a"> a) Membuat fungsi berjalan 2x lipat lebih cepat dari sebelumnya.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="b"> b) Membatalkan proses unduhan data yang saat itu sedang berjalan.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="c"> c) Berfungsi sebagai rem yang membekukan baris kode untuk menunggu hasil objek Future.</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="d"> d) Memberitahu Dart bahwa fungsi tersebut tidak memerlukan internet.</label></div>
  <button type="button" onclick="cekJawaban('q4')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q4" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>5. Saat menulis kode dengan kombinasi gaya async/await, taktik apa yang paling tepat untuk menangkap pesan error jika tiba-tiba server mati?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="a"> a) Menggunakan .catchError()</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="b"> b) Menggunakan statement if-else</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="c"> c) Menggunakan benteng try-catch konvensional</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="d"> d) Menggunakan perulangan while</label></div>
  <button type="button" onclick="cekJawaban('q5')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q5" style="margin-top: 15px;"></div>
</div>

<script>
const quizData = {
  q1: {
    correct: 'b',
    explanations: {
      a: 'Synchronous tidak memiliki kemampuan untuk memengaruhi sinyal asli Wi-Fi.',
      b: '<strong>Tepat sekali!</strong> Program Synchronous membekukan baris antrean di bawahnya, menyebabkan UI layar terblokir dan macet total sampai unduhan selesai.',
      c: 'Pengunduhan murni tidak membuat data rusak hanya karena metodenya.',
      d: 'Program tidak langsung tertutup, melainkan macet tidak bisa disentuh (hang).'
    }
  },
  q2: {
    correct: 'd',
    explanations: {
      a: 'Fungsi asinkron tidak bisa memunculkan String instan sebelum waktunya tiba.',
      b: 'Penggunaan dynamic adalah kebiasaan buruk, dan bukan standar asinkron.',
      c: 'List adalah tipe data kumpulan, bukan tanda asinkron.',
      d: '<strong>Tepat sekali!</strong> Fungsi asynchronous mutlak akan selalu mengembalikan objek berjenis <strong>Future</strong> sebagai bukti janji akan adanya data.'
    }
  },
  q3: {
    correct: 'b',
    explanations: {
      a: 'Fase kemenangan ini baru terjadi nanti setelah data selesai diunduh 100%.',
      b: '<strong>Tepat sekali!</strong> Pada detik pertama tombol ditekan, proses masih berjalan sibuk, sehingga status mutlaknya adalah <strong>Uncompleted</strong> (Belum Selesai).',
      c: 'Fase menyedihkan ini hanya akan terjadi apabila ternyata prosesnya gagal di tengah jalan.',
      d: 'Loading bukan nama fase teknis resmi di dalam objek Future Dart.'
    }
  },
  q4: {
    correct: 'c',
    explanations: {
      a: 'Kata await tidak memiliki kekuatan gaib untuk mempercepat kecepatan sistem mesin.',
      b: 'Untuk membatalkan proses, kamu tidak menggunakan kata await.',
      c: '<strong>Tepat sekali!</strong> await murni bertindak seperti sebuah tuas rem yang memaksa mesin program patuh menunggu sampai Future selesai membuahkan hasil.',
      d: 'Kata kunci await sama sekali tidak mendeteksi status internet.'
    }
  },
  q5: {
    correct: 'c',
    explanations: {
      a: 'Fungsi .catchError() adalah cara jadul yang hanya dipakai bersama .then().',
      b: 'Meskipun if-else kuat, ia tidak efektif untuk menampung lemparan error liar dari Future.',
      c: '<strong>Tepat sekali!</strong> Karena gaya async/await memaksa kode berjalan tegak lurus, kita kembali memanfaatkan benteng <strong>try-catch</strong> standar.',
      d: 'Perulangan while digunakan untuk me-looping kode, bukan menangkap error.'
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
