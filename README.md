<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<title>Project — Bumi & Antariksa</title>
<style>
body{
  margin:0;
  font-family:Verdana,sans-serif;
  color:white;
  background: url("background.jpg") no-repeat center center fixed;
  background-size: cover;
}
header{
  padding:30px;
  text-align:center;
  font-size:2.3em;
  font-weight:bold;
  background:rgba(0,0,0,0.7);
}
nav{
  display:flex;
  justify-content:center;
  flex-wrap:wrap;
  gap:10px;
  padding:15px;
}
nav button{
  padding:10px 16px;
  border:none;
  border-radius:10px;
  background:#00ffff;
  font-weight:bold;
  cursor:pointer;
}
.page{
  display:none;
  max-width:1100px;
  margin:30px auto;
  padding:40px;
  background:rgba(0,0,0,0.65);
  border-radius:25px;
}
.page.active{display:block;}
h2{color:#00ffff;}
footer{text-align:center;padding:30px;color:#ccc;}
.quiz button{
  margin:5px;
  padding:10px 15px;
  border:none;
  border-radius:8px;
  background:#00ffff;
}
iframe{width:100%;height:600px;border:none;border-radius:20px;}
</style>
</head>
<body>

<header>🚀 Project — Bumi & Antariksa</header>

<nav>
<button onclick="showPage(1)">Bab 1</button>
<button onclick="showPage(2)">Bab 2</button>
<button onclick="showPage(3)">Bab 3</button>
<button onclick="showPage(4)">Bab 4</button>
<button onclick="showPage(5)">Bab 5</button>
<button onclick="showPage(6)">Quiz</button>
<button onclick="showPage(7)">Simulasi</button>
</nav>

<div id="p1" class="page active">
<h2>Bab 1 — Pendahuluan</h2>
<p>Bumi dan antariksa merupakan bagian dari alam semesta yang saling berkaitan erat. Bumi adalah planet tempat kehidupan berkembang, sedangkan antariksa merupakan ruang luas yang mencakup semua benda langit di luar atmosfer Bumi. Dengan mempelajari antariksa, manusia dapat memahami posisi Bumi di tengah kosmos dan menyadari bahwa kehidupan di Bumi sangat bergantung pada kondisi di ruang angkasa.</p>
<p>Sejak zaman kuno, manusia telah mengamati pergerakan Matahari, Bulan, dan bintang untuk menentukan musim, arah, serta waktu. Kemajuan ilmu pengetahuan dan teknologi memungkinkan manusia membangun teleskop canggih dan mengirim wahana ke luar angkasa untuk mengamati planet dan galaksi secara langsung. Hal ini memperluas wawasan manusia tentang alam semesta.</p>
<p>Pembelajaran tentang Bumi dan antariksa penting agar manusia memahami lingkungan kosmiknya dan dapat menjaga keberlanjutan kehidupan di planet ini. Dengan pemahaman yang baik, manusia dapat menggunakan teknologi antariksa secara bijak dan bertanggung jawab.</p>
</div>

<div id="p2" class="page">
<h2>Bab 2 — Tata Surya</h2>
<p>Tata surya adalah sistem yang terdiri atas Matahari sebagai pusat dan semua benda langit yang mengelilinginya karena gaya gravitasi. Planet, satelit, asteroid, dan komet bergerak dalam lintasan yang teratur yang disebut orbit. Keseimbangan gaya inilah yang menjaga keteraturan tata surya.</p>
<p>Matahari merupakan sumber energi utama yang menyediakan cahaya dan panas bagi seluruh tata surya. Energi Matahari mengatur iklim Bumi, siklus air, serta mendukung kehidupan melalui fotosintesis tumbuhan. Tanpa Matahari, kehidupan di Bumi tidak akan mungkin terjadi.</p>
<p>Setiap planet memiliki karakteristik yang unik, baik dari segi ukuran, komposisi, maupun atmosfer. Keanekaragaman ini menjadikan tata surya sebagai laboratorium alam untuk memahami pembentukan dan evolusi sistem planet.</p>
</div>

<div id="p3" class="page">
<h2>Bab 3 — Planet, Bintang, dan Galaksi</h2>
<p>Planet adalah benda langit yang mengorbit bintang dan tidak memancarkan cahaya sendiri. Planet dapat berbentuk padat seperti Bumi atau berupa gas raksasa seperti Jupiter. Kondisi tiap planet sangat berbeda dan mencerminkan proses pembentukannya.</p>
<p>Bintang adalah bola gas panas yang memancarkan energi melalui reaksi nuklir di intinya. Cahaya dari bintang dapat menempuh jarak yang sangat jauh sehingga memungkinkan manusia mengamati galaksi lain di alam semesta.</p>
<p>Galaksi merupakan kumpulan miliaran bintang yang terikat oleh gravitasi. Galaksi Bima Sakti adalah rumah bagi tata surya kita dan merupakan bagian kecil dari alam semesta yang sangat luas.</p>
</div>

<div id="p4" class="page">
<h2>Bab 4 — Eksplorasi Antariksa</h2>
<p>Eksplorasi antariksa dilakukan melalui pengamatan teleskop dan pengiriman wahana ke luar angkasa. Sejak peluncuran satelit pertama, manusia terus mengembangkan teknologi untuk menjelajah lebih jauh.</p>
<p>Misi ke Bulan, Mars, dan planet lain menghasilkan data penting tentang kemungkinan kehidupan di luar Bumi dan kondisi ekstrem ruang angkasa.</p>
<p>Teknologi antariksa juga bermanfaat bagi kehidupan sehari-hari, seperti komunikasi satelit, navigasi GPS, dan pemantauan cuaca global.</p>
</div>

<div id="p5" class="page">
<h2>Bab 5 — Masa Depan Antariksa</h2>
<p>Manusia berencana membangun koloni di Bulan dan Mars untuk memperluas wilayah kehidupan. Hal ini memerlukan teknologi canggih dan kerja sama internasional.</p>
<p>Namun eksplorasi ini juga menimbulkan tantangan etika, risiko kesehatan astronaut, dan biaya besar yang harus dikelola dengan bijak.</p>
<p>Karena itu, masa depan antariksa harus diarahkan pada keberlanjutan dan kesejahteraan umat manusia secara global.</p>
</div>

<div id="p6" class="page quiz">
<h2>Quiz Astronaut</h2>
<p id="q"></p>
<div id="choices"></div>
<p id="score"></p>
</div>

<div id="p7" class="page">
<h2>Simulasi Tata Surya</h2>
<iframe src="https://eyes.nasa.gov/apps/solar-system/#/home"></iframe>
</div>

<footer>© 2026 Alvaro Digital</footer>

<script>
const quiz=[
 {q:"Planet terbesar di tata surya adalah...",c:["Mars","Jupiter","Bumi"],a:1},
 {q:"Pusat tata surya adalah...",c:["Matahari","Bulan","Mars"],a:0},
 {q:"Galaksi tempat kita berada adalah...",c:["Andromeda","Bima Sakti","Sombrero"],a:1}
];
let current=0,score=0;
function showPage(n){
 document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
 document.getElementById('p'+n).classList.add('active');
 if(n===6){current=0;score=0;showQuestion();}
}
function showQuestion(){
 let q=quiz[current];
 document.getElementById("q").innerText=q.q;
 document.getElementById("choices").innerHTML=q.c.map((c,i)=>`<button onclick="answer(${i})">${c}</button>`).join("");
 document.getElementById("score").innerText="";
}
function answer(i){
 if(i===quiz[current].a)score++;
 current++;
 if(current<quiz.length)showQuestion();
 else document.getElementById("score").innerText="Skor kamu: "+score+" / "+quiz.length;
}
</script>

</body>
</html>
