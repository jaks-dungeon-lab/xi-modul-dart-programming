# Quiz Collections

Uji pemahaman logikamu seputar pembagian kategori jenis wadah penyimpanan *Collections* Dart di bawah ini. Pilih dan pastikan jawaban yang paling sesuai!

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>1. Jika kita memiliki data berupa senarai nama siswa dan kita ingin mencarinya berdasarkan nomor urutan masuk pendaftaran, koleksi apakah yang mutlak paling tepat untuk kita gunakan?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="a"> a) Map</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="b"> b) List</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="c"> c) Set</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q1" value="d"> d) Object</label></div>
  <button type="button" onclick="cekJawaban('q1')" style="padding: 8px 16px; background-color: rgba(41, 128, 185, 0.8); color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q1" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>2. Manakah sifat hukum alam di bawah ini yang paling benar mengenai penggunaan wadah Map?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="a"> a) Dapat memanggil isinya berdasarkan nomor angka urut dari 0.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="b"> b) Terdiri dari rentetan nilai himpunan tunggal di dalam kurung siku.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="c"> c) Label Key tidak boleh ada yang ganda duplikat kembar di dalam satu wilayah yang sama.</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q2" value="d"> d) Value (Isi) tidak boleh memiliki nilai angka atau tulisan teks ganda.</label></div>
  <button type="button" onclick="cekJawaban('q2')" style="padding: 8px 16px; background-color: rgba(41, 128, 185, 0.8); color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q2" style="margin-top: 15px;"></div>
</div>

<div class="question-block" style="margin-bottom: 25px; padding: 20px; border: 1px solid rgba(128, 128, 128, 0.3); border-radius: 8px;">
  <p style="margin-bottom: 15px; font-size: 1.05em;"><strong>3. Apa yang mutlak akan terjadi jika kita memaksakan menginput data berbunyi "Semangka" ke dalam sebuah Set yang sebelumnya ternyata sudah memiliki isi "Semangka"?</strong></p>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="a"> a) Mesin akan meneriaki kode error merah dan mematikan sistem program kita.</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="b"> b) Set akan membiarkannya lolos masuk dan menghasilkan himpunan berisi dua "Semangka".</label></div>
  <div style="margin-bottom: 8px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="c"> c) Set akan mengabaikan menelan musnahkan data "Semangka" yang kedua tersebut tanpa menghasilkan notifikasi peringatan apa pun.</label></div>
  <div style="margin-bottom: 15px;"><label style="cursor: pointer;"><input type="radio" name="q3" value="d"> d) Komputer akan mengubah tulisan "Semangka" menjadi angka nomor seri acak demi membedakannya.</label></div>
  <button type="button" onclick="cekJawaban('q3')" style="padding: 8px 16px; background-color: rgba(41, 128, 185, 0.8); color: white; border: none; border-radius: 4px; cursor: pointer;">Cek Jawaban</button>
  <div id="feedback-q3" style="margin-top: 15px;"></div>
</div>

<script>
const quizData = {
  q1: {
    correct: 'b',
    explanations: {
      a: '<strong>Map</strong> justru membuang pengurutan angka dan lebih mengandalkan label penamaan teks bebas.',
      b: '<strong>Tepat sekali!</strong> <strong>List</strong> adalah barisan laci berderet yang paling handal sangat superior jika tujuan kita adalah mengambil data secara baku murni berdasarkan nomor urutan laci angka.',
      c: '<strong>Set</strong> tidak dianjurkan untuk mengambil data berdasarkan nomor urut karena desain intinya berfokus acak pada pembuangan filter memori kembar.',
      d: '<strong>Object</strong> bukan jenis tipe himpunan wadah koleksi, melainkan kasta turunan tertinggi induk dasar dari semua jenis nilai Dart.'
    }
  },
  q2: {
    correct: 'c',
    explanations: {
      a: 'Pengambilan laci data menggunakan angka index 0 adalah hukum milik saudara sepupunya yakni himpunan jenis <strong>List</strong>.',
      b: 'Menggunakan rentetan wujud tunggal tanpa pasangan di dalam ruang kurung siku `[]` adalah wujud desain perakitan <strong>List</strong>.',
      c: '<strong>Tepat sekali!</strong> Dalam kamus sistem hukum loker penyimpanan <strong>Map</strong>, dilarang keras menempeli menimpa dua loker dengan label pintu stiker nama kunci *Key* yang sama mutlak.',
      d: 'Hukum larangan data kembar mutlak di dalam sistem *Map* itu hanya diimplementasikan diterapkan kuat untuk *Key* saja, sedangkan *Value* (isi nilai dalam loker) dibebaskan sebebas-bebasnya bernilai kembar berulang.'
    }
  },
  q3: {
    correct: 'c',
    explanations: {
      a: 'Mesin eksekutor Dart sama sekali tidak memedulikan pemicu aktivitas itu sebagai tindak pelanggaran, ia tidak akan memutus mati sistem.',
      b: 'Tindakan membiarkan mendiamkan terjadinya data dobel kembar bertumpuk adalah ciri lemah kelalaian milik ruang tipe <strong>List</strong>, bukan *Set*.',
      c: '<strong>Tepat sekali!</strong> Hukum tabiat mutlak utama himpunan kelas murni penjaga perbatasan <strong>Set</strong> adalah ia selalu mutlak tanpa banyak basa-basi akan segera otomatis menelan mementahkan dan menghanguskan isi data asing apa pun yang diusahakan disuntikkan masuk jika rupanya ada wujud yang mirip atau sama di dalam ruangannya.',
      d: 'Pemaksaan pengubahan mesin kompilator *hash* data semangka menjadi nomor digit acak hanya akan merusak validitas pencetakan laporan teks aslinya.'
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
    feedbackDiv.innerHTML = '<span style="color: rgba(230, 126, 34, 1); font-weight: bold;">Tentukan salah satu opsi pilihan jawaban terlebih dahulu!</span>';
    return;
  }
  
  const qData = quizData[questionId];
  const isCorrect = selectedValue === qData.correct;
  const penjelasanSpesifik = qData.explanations[selectedValue];
  
  let resultText = '';
  if (isCorrect) {
    resultText = '<span style="color: rgba(39, 174, 96, 1); font-weight: bold; font-size: 1.1em;">Benar.</span><br>';
  } else {
    resultText = '<span style="color: rgba(192, 57, 43, 1); font-weight: bold; font-size: 1.1em;">Salah.</span><br>';
  }
  
  const explanationBox = '<div style="margin-top: 15px; padding: 15px; background-color: rgba(128, 128, 128, 0.1); border-left: 5px solid rgba(41, 128, 185, 0.8); font-size: 0.95em; line-height: 1.5; color: inherit;">' + penjelasanSpesifik + '</div>';
  
  feedbackDiv.innerHTML = resultText + explanationBox;
}
</script>
