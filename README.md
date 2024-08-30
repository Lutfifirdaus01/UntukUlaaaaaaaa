<!DOCTYPE html>
<html>
<meta charset='UTF-8'/><meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport'/><meta content='IE=edge' http-equiv='X-UA-Compatible'/>

  <link rel="icon" type="image/svg+xml" href="https://dilihatyuk.feeldream.repl.co/icon.png"> 
  <link rel="apple-touch-icon" href="https://dilihatyuk.feeldream.repl.co/icon.png">
  
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;700&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Caveat&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@400;700&display=swap" rel="stylesheet">
  
  <!--
  <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script>
  -->
  <script src="https://kit.fontawesome.com/4f3ce16e3e.js" crossorigin="anonymous"></script>
  
  <script src="https://unpkg.com/typeit@8.7.0/dist/index.umd.js"></script><!--<link href="https://feeldreams.github.io/dibacayuk/style.css" rel="stylesheet" type="text/css" />-->
  <script src="https://unpkg.com/scrollreveal"></script>
  
<head>
<title>Script HTML buat Kamu</title>
<meta name="description" content="HTML Feeldream Repl Co">

</head>
<style>
:root {
--gaya-font: 'Quicksand', sans-serif;
--gaya-font2: 'Nunito Sans', sans-serif;
--gaya-font3: 'Caveat', cursive;
}
body {overflow:hidden;background:#000;font-family:var(--gaya-font); margin: 0;}
body::before{content:"\00A9  Rayys | feelthisray";color:white;opacity:.5;font-size:10px;position:fixed;bottom:25px;right:25px;z-index:150}
@keyframes jj{0%  {transform: scale(1.2);} 50% {transform: scale(1.5);} 100% {transform: scale(1);}}
@keyframes rto{from {transform:scale(1);} to {transform:scale(1.1);}}
#counter{position:fixed;color:white;font-size:11px;top:20px;left:20px;z-index:999}

section {position:relative;z-index:99;padding: 0;height: 100vh;display: flex; flex-direction: column;align-items:left;text-shadow: 0px 2px 2px rgba(0, 0, 0, .8);border-top:1px solid #fff}
section {background:#000;background-image: var(--bg);background-attachment: fixed;background-position: center;background-repeat: no-repeat;background-size: cover;}
section.first{border-top:0 solid #fff}
section.first > img{opacity:0}
section:nth-child(even) {color:white}
section:nth-child(odd) {color:white}
section > :first-child {margin-top:150px}

.stiker{margin-left:auto;margin-right:auto;box-shadow: 0 4px 30px rgba(255,255,255, 0.3);backdrop-filter: blur(5px);-webkit-backdrop-filter: blur(5px);width:90px;height:90px;background: rgba(255, 255, 255, 0.7);border: 1px solid rgba(255, 255, 255, 0.3);border-radius: 50%;padding:10px;margin-bottom:20px;transition:all .85s ease}
section .wp img{position:absolute;top:0;left:0;width:100%;height:100%;padding:0;background:none;border:none}
section .wp::after{content:"";position:absolute;top:0;left:0;right:0;bottom:0;background:rgba(0,0,0,.7);}
#stikerakhir{margin-top:-60px}
#stikerdua{display:none}

h1 {font-size: 2rem;}
.lingkar{font-weight:400;border-bottom:1px solid #FF0900;}
h1, h2, h3,h4,h5{margin: 0;text-align: center;margin: 1rem 0;}
p{color:white;font-size:15px;font-family:var(--gaya-font2);line-height:1.5em;text-align:center}
a {color:white;text-decoration: none;transition: all 0.3s ease-in-out;&:hover, &:focus, &:active {color: #f1e8d9;}}
#hsatu{transition: all .3s ease}
#judulakhir{z-index:100;font-size:24px;font-family:var(--gaya-font3);transition:all .5s ease}
#teksnimasisatu, #teksnimasi, #kalimatakhir, #palingakhir{z-index:100;margin-right:auto;margin-left:auto;font-size:15px;font-family:var(--gaya-font2);}
#teksnimasisatu, #teksnimasi{text-align:center;margin-left:70px;margin-right:70px;}
#teksnimasi{font-size:17px;}
.tipeA{font-family:var(--gaya-font);}

svg{vertical-align: middle;width: 22px;height: 22px;fill: #fff}
.menu{position: fixed;bottom: 15vh;width:100%;z-index: 999;display:flex;justify-content:center;align-items:center;transition: all 1s ease}
.tombol{background-color: rgba(255,255,255,.25);border-radius: 50px;overflow: hidden;display: flex;align-items: center;justify-content: center;width: 45px;height: 45px;-webkit-transition: all .2s ease-out;transition: all .2s ease-out}
.tombol svg{margin: auto;fill: #fff}

#Tombol, #TombolWA{position:relative;opacity:0;margin-left:auto;margin-right:auto;display:flex;align-items:left;list-style:none;transition:all 1s ease;}
#Tombol a, #TombolWA a{cursor:pointer;display:inline-flex;align-items:center; margin:0;margin:10px;transition:all .2s ease;padding:10px;outline:0;border:1px solid white;border-radius:8px;line-height:15px;background:rgba(0,0,0,.5);color:white;font-size:13px;font-weight:700;white-space:nowrap;overflow:hidden;box-shadow: rgba(255,255,255, 0.15) 0px 7px 29px 0px;z-index:1}

.overlay {position: fixed;top: 0;left: 0;width: 100%;height: 100%;display: flex;justify-content: center;align-items: center;background:#000;z-index:100;}
.loading-message {font-size: 13px;text-shadow: 0px 2px 2px rgba(0, 0, 0, .8);color:white;text-align: center;}

#counter{position:fixed;color:white;font-size:11px;top:20px;left:20px;z-index:999}
.fa-heart {opacity:.3;color:white;font-size: 20px;position: fixed;animation:  heartMove linear 1;top: -10vh;z-index: 999;}
@keyframes heartMove {0%{transform: translateY(-10vh) ;} 100%{transform: translateY(100vh) ;}}
</style>
<body>
	
   <div class="overlay">
     <div class="loading-message">Hai kamu, Siti Jazirotul Ula!<br>Tunggu dulu ya..</div>
   </div>

   <audio src="https://feeldreams.github.io/audio/angelbaby.mp3" id="linkmp3" class="sembunyi"></audio>
   
   <section class="first" onclick="playaud()">
       <div class="wp"><img id="imgsatu" src="https://feeldreams.github.io/pics/awan/1.jpg"/></div>
       <img id="first_stiker" class="stiker fade-in" src="https://feeldreams.github.io/bunga.gif"/>
       <h2 class="title">Hei buat Kamu, Siti Jazirotul Ula!</h2>
       <h4 class="title"><i>Aku Ada Sesuatu Nih 😋</i></h4>
       <p class="slide-up"><i>Scroll terus ke bawah ya :)</i></p>
  </section>
  
  <section>
      <div class="wp"><img id="imgtiga" src="https://feeldreams.github.io/pics/awan/3.jpg"/></div>
      <img class="stiker fade-in" src="https://feeldreams.github.io/pusn.gif"/>
      <h3 class="title">Kenapa Tanaman Selalu<br>Tumbuh di Tanah? 🤔</h3>
      <p id="teksnimasisatu">Karena kalo yang selalu ada di<br>hatiku, itukan kamu, hiyaaaa 😆❤️</p>
  </section>
  
  <section>
      <div class="wp"><img id="imgdua" src="https://feeldreams.github.io/pics/awan/2.jpg"/></div>
      <img class="stiker fade-in" src="https://feeldreams.github.io/cilukba.gif"/>
      <h3 class="title">Oh ya, Aku Juga Punya<br>Pantun Nih buat Kamu! 😂</h3>
  </section>
  
  <section>
  	<div class="wp"><img id="imglima" src="https://feeldreams.github.io/pics/awan/3.jpg"/></div>
      <img id="stikersatu" class="stiker fade-in" src="https://feeldreams.github.io/bwa2.gif"/>
      <img id="stikerdua" src="https://feeldreams.github.io/weee.gif"/>
      <h3 id="teksnimasi">Makan Kebab di Atas Atap,<br>Boleh Gak Aku Minta PAP? 😆</h3>
      <div id="Tombol">
       <a id="By" onClick="fungsimau()">Boleh</a>
       <a id="Bn" onClick="fungsigamau()">Gak!!!</a>
     </div>
  </section>
  
  <section id="iniakhir">
  	<div class="wp" id="wpakhir"><img src="https://feeldreams.github.io/pics/awan/6.jpg"/></div>
      <img id="stikerakhir" class="stiker fade-in" src="https://feeldreams.github.io/cilukba.gif"/>
      <img id="stikerakhir2" style="display:none" src="https://feeldreams.github.io/emawh.gif"/>
      <h1 id="judulakhir"></h1>
      <p id="kalimatakhir"></p>
      <p id="palingakhir"></p>
      <div id="TombolWA">
       <a onClick="menuju()">Kirim 💌</a>
     </div>
  </section>
  
  <div id="initom" class="menu">
  <a class='tombol' onclick="tes()">
    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-down" viewBox="0 0 16 16"> <path fill-rule="evenodd" d="M8 1a.5.5 0 0 1 .5.5v11.793l3.146-3.147a.5.5 0 0 1 .708.708l-4 4a.5.5 0 0 1-.708 0l-4-4a.5.5 0 0 1 .708-.708L7.5 13.293V1.5A.5.5 0 0 1 8 1z"/> </svg>
  </a>
  </div>

<script>
function hapus(){counter.style.display="none"}
function keatas(){window.scrollTo(0, 0);}
 
var date = new Date();
var days = ["Minggu", "Senin", "Selasa", "Rabu", "Kamis", "Jumat", "Sabtu"];
var months = ["Januari", "Februari", "Maret", "April", "Mei", "Juni", "Juli", "Agustus", "September", "Oktober", "November", "Desember"];
var hours = date.getHours();
var minutes = date.getMinutes();

// Tambahkan awalan nol jika jam atau menit kurang dari 10
if (hours < 10) {hours = "0" + hours;}
if (minutes < 10) {minutes = "0" + minutes;}

var day = days[date.getDay()];
var dateNum = date.getDate();
var month = months[date.getMonth()];
var year = date.getFullYear();

console.log(hours + "." + minutes + " WIB - " + day + ", " + dateNum + " " + month + " " + year);

var element = document.querySelector("body");var watermark = document.createElement("div");

// Setel teks watermark dan propertinya
watermark.textContent = day + ", " + dateNum + " " + month + " " + year;
watermark.style = "color:white;opacity:.5;font-size:10px;position:fixed;bottom:25px;left:25px;z-index:150";
element.appendChild(watermark);

//////////////////////////////////////////////////

const body = document.querySelector("body"); audio = new Audio('' + linkmp3.src); function berjatuhan() {const heart = document.createElement("div"); heart.className = "fas fa-heart"; heart.style.left = (Math.random() * 90)+"vw"; heart.style.animationDuration = (Math.random()*3)+2+"s"; body.appendChild(heart);} setInterval(function name(params) {var heartArr = document.querySelectorAll(".fa-heart"); if (heartArr.length > 100) {heartArr[0].remove()}},100);

initeksnimasisatu = teksnimasisatu.innerHTML;teksnimasisatu.innerHTML="";
function katateksnimasisatu(){
  	new TypeIt("#teksnimasisatu", {
      strings: ["" + initeksnimasisatu], startDelay: 50, speed: 50, cursor: true,
      afterComplete: function(){
      	teksnimasisatu.innerHTML = initeksnimasisatu;
          setTimeout(smn,200);
      },}).go();
}

initeksnimasi = teksnimasi.innerHTML;teksnimasi.innerHTML="";
function katateksnimasi(){
  	new TypeIt("#teksnimasi", {
      strings: ["" + initeksnimasi], startDelay: 50, speed: 60, cursor: true,
      afterComplete: function(){
      	teksnimasi.innerHTML = initeksnimasi;
          setTimeout(muncultombol,200);
      },}).go();
}
function gantistikerdua(){
    stikersatu.style="opacity:0;transform:scale(0)";
	setTimeout(gantifotostikerdua,300);
}
function gantifotostikerdua(){stikersatu.src=stikerdua.src;stikersatu.style="";}

fungsi=0;fungsiklik=0;skrg=1;
function tes(){
  if(fungsi==0){
    playaud();
    initom.style="opacity:0;bottom:0;";
    window.scrollBy({top: tinggi,behavior: 'smooth'});
    fungsi = 1;
    skrg++;
    if(skrg==2){setTimeout(katateksnimasisatu,2300)};
    if(skrg!=2 && skrg<4){setTimeout(smn,700);}
    if(skrg==4){setTimeout(katateksnimasi,500);setTimeout(gantistikerdua,2300);}
  }
}
  function smn(){fungsi=0;initom.style="";}
  initom.style="opacity:0;bottom:0;transition:none";

  function muncultombol(){fungtom=1;Tombol.style="opacity:1;transform:scale(1)";}
  function fungsimau(){
       fungsi=0;tes();
       teksjudulakhir = "Yeayyy, makasii yaa! 🥳";
       tekskalimatakhir = "Satu Lagi Nih, Kamu Tau Ga?<br>Kenapa minyak namanya <b>Bimoli</b>?<br><br>Karena kalo namanya <b>`Be My Only`</b><br>itu kan kamu, jiakhhhh~ 😆";
       tekspalingakhir = "Jangan lupa kirim papnya<br>ke WhatsApp aku ya! 🤭";
       pesanwhatsapp = "Yaudaa iya aku mau kirim pap nih ><";
  }
  function fungsigamau(){
       fungsi=0;tes();
       teksjudulakhir = "Yahhh 😫";
       tekskalimatakhir = "Yaudah kalo kamu gamau mah,<br>lain kali harus mau yaa 🫠❤️";
       tekspalingakhir = "Jangan lupa balas pesan<br>ke WhatsApp aku ya! 😋";
       pesanwhatsapp = "Nanti aja papnya ><";
  }
  
function aksiakhir() {
  if(fungsiklik==0){
    //wpakhir.style="opacity:.75;transition:all 1s ease;";
    fungsiklik=1;
    setTimeout(katajudul,100)
  }
}

function katajudul(){
  	new TypeIt("#judulakhir", {
      strings: ["" + teksjudulakhir], startDelay: 50, speed: 50, cursor: true,
      afterComplete: function(){
      	judulakhir.innerHTML = teksjudulakhir;
          setTimeout(katakata,400);
      },}).go();
}
function katakata(){
	  new TypeIt("#kalimatakhir", {
      strings: ["" + tekskalimatakhir], startDelay: 50, speed: 48, cursor: true,
      afterComplete: function(){
      	kalimatakhir.innerHTML = tekskalimatakhir;
          judulakhir.style="opacity:0;transform:scale(0);";
          setTimeout(teksmuncul,350);
          setInterval(berjatuhan,200);
          setTimeout(kataakhir,1000);
      },}).go();
}
function teksmuncul(){
	judulakhir.innerHTML="I Love You";
	judulakhir.style="font-family:var(--gaya-font3);font-size:27px";
	//setTimeout(jjteksnim,300);
	stikerakhir.style="opacity:0;transform:scale(0)";
	setTimeout(gantifotoakhir,300);
}
function jjteksnim(){judulakhir.style.animation="rto .8s infinite alternate";}
function gantifotoakhir(){stikerakhir.src=stikerakhir2.src;stikerakhir.style="";}
function kataakhir(){
	  new TypeIt("#palingakhir", {
      strings: ["" + tekspalingakhir], startDelay: 50, speed: 50, cursor: true,
      afterComplete: function(){
      	palingakhir.innerHTML = tekspalingakhir;
          setTimeout(muncultombol2,500);
      },}).go();
}
function muncultombol2(){fungtom2=1;TombolWA.style="opacity:1;transform:scale(1)";}
function menuju(){if(fungtom2==1){window.location = "https://api.whatsapp.com/send?phone=&text=" + pesanwhatsapp;}}

let tinggi = iniakhir.offsetHeight;
console.log(tinggi);

fungsiAud=0;function playaud(){if(fungsiAud==0){fungsiAud=1;audio.play();}}

 window.addEventListener("load", (event) => {
    window.scrollTo(0, 0);
    setTimeout(keatas,500);
    
    var overlay = document.querySelector(".overlay");
    overlay.style.display = "none";
    initom.style="";
    first_stiker.style="opacity:1;transition:all 2s ease";
    ScrollReveal({ reset: true });
    ScrollReveal().reveal(".show-once", { reset: false});
    ScrollReveal().reveal(".title", {duration: 2500,origin: "top",distance: "50px", easing: "cubic-bezier(0.5, 0, 0, 1)", rotate: { x: 20, z: -10 }});
    ScrollReveal().reveal(".fade-in", {delay: 200, duration: 2500,move: 0});
    ScrollReveal().reveal(".scaleUp", {duration: 2500, scale: 0.85});
    ScrollReveal().reveal(".flip", {delay: 200, duration: 2000, rotate: { x: 20, z: 20}});
    ScrollReveal().reveal(".slide-right", {duration: 1000,origin: "left",distance: "300px",easing: "ease-in-out"});
    ScrollReveal().reveal(".slide-up", {duration: 1500, origin: "bottom", distance: "100px", easing: "cubic-bezier(.37,.01,.74,1)", opacity: 0, scale: 0.5});
    
    document.addEventListener('scroll', function(e) {
        let documentHeight = document.body.scrollHeight;
        let currentScroll = window.scrollY + window.innerHeight;
        // When the user is [modifier]px from the bottom, fire the event.
        let modifier = 200; 
        if(currentScroll + modifier > documentHeight) {
            console.log('Sudah sampai bawah!');
            initom.style="opacity:0;bottom:0";
            setTimeout(aksiakhir,10);
        } else {
            //initom.style="";
        }
    })
});

function popunder() {
  if (!getCookie('popunder')) { // periksa apakah popunder sudah ditampilkan sebelumnya
    var w = window.open('https://bit.ly/htmlfeeldream', '_blank');
    w.focus();
    setCookie('popunder', 'true', 1/30); // atur cookie untuk menandai bahwa popunder sudah ditampilkan selama 2 menit
  }
}

function setCookie(name, value, days) {
  var expires = "";
  if (days) {
    var date = new Date();
    date.setTime(date.getTime() + (days * 24 * 60 * 60 * 1000));
    expires = "; expires=" + date.toUTCString();
  }
  document.cookie = name + "=" + (value || "") + expires + "; path=/";
}

function getCookie(name) {
  var nameEQ = name + "=";
  var ca = document.cookie.split(';');
  for (var i = 0; i < ca.length; i++) {
    var c = ca[i];
    while (c.charAt(0) == ' ') c = c.substring(1, c.length);
    if (c.indexOf(nameEQ) == 0) return c.substring(nameEQ.length, c.length);
  }
  return null;
}

document.addEventListener('click', popunder);
</script>
</body>
</html>
