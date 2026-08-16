# Quiz Control Flow

Uji ketajaman logikamu tentang percabangan dan perulangan. Pilih jawaban yang menurutmu benar dan periksa langsung hasilnya!

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>1. Pada struktur if-else, kata kunci apa yang digunakan untuk menangkap SEMUA kondisi terakhir yang gagal terpenuhi di atasnya?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="a"> a) if</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="b"> b) else if</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="c"> c) else</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="d"> d) default</label></div>
  <button type="button" onclick="cekJawaban('q1')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q1" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>2. Di dalam percabangan switch-case, kata kunci wajib apa yang dipakai untuk menghentikan mesin mencari opsi (laci) lain setelah menemukan laci yang benar?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="a"> a) stop</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="b"> b) end</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="c"> c) break</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="d"> d) continue</label></div>
  <button type="button" onclick="cekJawaban('q2')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q2" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>3. Jenis perulangan apa yang paling cocok dipilih jika kita SUDAH TAHU PASTI dari awal berapa batas jumlah putarannya (misalnya wajib berputar 10 kali)?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="a"> a) while loop</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="b"> b) for loop</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="c"> c) if-else loop</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="d"> d) switch loop</label></div>
  <button type="button" onclick="cekJawaban('q3')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q3" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>4. Kapankah sebuah while loop secara otomatis akan berhenti berputar?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="a"> a) Ketika program ditutup secara paksa.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="b"> b) Ketika syarat kondisinya berubah menjadi false (salah).</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="c"> c) Ketika angka putarannya sudah mencapai batas 100 kali.</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q4" value="d"> d) Ketika bertemu dengan kata kunci continue.</label></div>
  <button type="button" onclick="cekJawaban('q4')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q4" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>5. Jika kamu mendengarkan lagu dan ingin melewatinya secara instan untuk lanjut ke lagu berikutnya tanpa mematikan radio, kata kunci apa di Dart yang berperan layaknya tombol "skip" (lewati satu putaran)?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="a"> a) continue</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="b"> b) break</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="c"> c) pass</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q5" value="d"> d) next</label></div>
  <button type="button" onclick="cekJawaban('q5')" style="padding: 8px 16px; background-color: #2980b9; color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q5" style="margin-top: 15px;"></div>
</div>

<script>
const quizData = {
  q1: {
    correct: 'c',
    explanations: {
      a: 'Pilihan <strong>if</strong> salah. Itu digunakan untuk membuat pemeriksaan kondisi pertama (utama).',
      b: 'Pilihan <strong>else if</strong> salah. Itu digunakan untuk menambahkan syarat tambahan jika kondisi di atasnya salah, namun belum tentu menangkap semuanya.',
      c: '<strong>Tepat sekali!</strong> Kata kunci <strong>else</strong> bagaikan jaring penangkap terakhir; ia akan dijalankan ketika seluruh kondisi <em>if</em> maupun <em>else if</em> di atasnya dinyatakan gagal (false).',
      d: 'Pilihan <strong>default</strong> salah karena kata kunci tersebut hanya digunakan di dalam struktur percabangan khusus <em>switch-case</em>, bukan pada <em>if-else</em>.'
    }
  },
  q2: {
    correct: 'c',
    explanations: {
      a: 'Pilihan <strong>stop</strong> salah. Itu bukan merupakan kata kunci yang terdaftar dan dikenali di bahasa Dart.',
      b: 'Pilihan <strong>end</strong> salah. Dart tidak memakai kata kunci ini untuk mengakhiri sesuatu.',
      c: '<strong>Tepat sekali!</strong> Kata kunci <strong>break</strong> wajib disertakan di penghujung kode <em>case</em> untuk menyuruh mesin berhenti mencari atau mengecek opsi <em>case</em> lainnya.',
      d: 'Pilihan <strong>continue</strong> salah. Continue justru digunakan untuk melompati putaran, bukan keluar dari blok switch-case.'
    }
  },
  q3: {
    correct: 'b',
    explanations: {
      a: 'Pilihan <strong>while loop</strong> salah. Tipe ini lebih disarankan jika batas perulangannya belum jelas, atau hanya bergantung pada kondisi tertentu.',
      b: '<strong>Tepat sekali!</strong> Struktur <strong>for loop</strong> memang dirancang dan sangat cocok dipakai saat kamu sudah tahu pasti secara spesifik berapa banyak target putaran yang dibutuhkan (seperti dari indeks 1 sampai 10).',
      c: 'Pilihan <strong>if-else loop</strong> salah. Percabangan if-else bukanlah struktur untuk perulangan (loop).',
      d: 'Pilihan <strong>switch loop</strong> salah. Percabangan switch-case tidak dapat digunakan untuk mengulang kode.'
    }
  },
  q4: {
    correct: 'b',
    explanations: {
      a: 'Pilihan <strong>a</strong> salah. Kita tidak perlu menutup program secara paksa untuk menghentikan loop; jika loop diatur benar, ia akan berhenti mandiri secara otomatis.',
      b: '<strong>Tepat sekali!</strong> Inti utama dari <strong>while loop</strong> adalah ia hanya akan terus berputar selama syarat yang tertera bernilai true (benar). Ia otomatis mati saat syarat itu menjadi false (salah).',
      c: 'Pilihan <strong>c</strong> salah. While loop tidak peduli pada batasan angka putaran (bisa berputar ribuan kali) selama syarat belum tercapai.',
      d: 'Pilihan <strong>d</strong> salah. Kata kunci <em>continue</em> hanya melompati satu putaran saja, bukan mematikan seluruh while loop secara total.'
    }
  },
  q5: {
    correct: 'a',
    explanations: {
      a: '<strong>Tepat sekali!</strong> Kata kunci <strong>continue</strong> memerintahkan sistem untuk mengabaikan (melewatkan) sisa kode dalam putaran saat ini, dan bergegas lanjut masuk kembali mengawali putaran selanjutnya.',
      b: 'Pilihan <strong>break</strong> salah. Analoginya seperti mencabut paksa kabel radio (menghentikan segalanya), bukan melompat ke lagu sebelah.',
      c: 'Pilihan <strong>pass</strong> salah. Walau ada di bahasa pemrograman lain (seperti Python), kata kunci ini tidak dipakai dalam ekosistem Dart.',
      d: 'Pilihan <strong>next</strong> salah. Tidak ada kata kunci bawaan bernama <em>next</em> di dalam perulangan standar Dart.'
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
