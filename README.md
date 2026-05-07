 <title>Abdul & Syahrillah</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:'Poppins',sans-serif;
background:#000;
overflow:hidden;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
}

/* OPENING */

#opening{
position:fixed;
width:100%;
height:100%;
background:
linear-gradient(rgba(0,0,0,.55),rgba(0,0,0,.55)),
url('https://images.unsplash.com/photo-1519741497674-611481863552?q=80&w=1200&auto=format&fit=crop');

background-size:cover;
background-position:center;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
z-index:99999;
color:white;
text-align:center;
padding:30px;
}

#opening h1{
font-size:42px;
margin-bottom:10px;
}

#opening p{
font-size:16px;
opacity:.9;
}

#openBtn{
margin-top:25px;
padding:14px 30px;
border:none;
border-radius:999px;
background:white;
color:black;
font-family:'Poppins',sans-serif;
font-weight:600;
font-size:15px;
cursor:pointer;
}

/* PHONE */

.phone{
width:100%;
max-width:430px;
height:100vh;
background:#000;
position:relative;
overflow:hidden;
display:none;
border-radius:40px;
box-shadow:0 0 40px rgba(0,0,0,.5);
border:8px solid #111;
}

.phone::before{
content:'';
position:absolute;
top:10px;
left:50%;
transform:translateX(-50%);
width:140px;
height:28px;
background:#000;
border-radius:20px;
z-index:9999;
}

/* HEADER */

.header{
height:95px;
background:rgba(28,28,30,.92);
backdrop-filter:blur(20px);
padding:10px 16px;
color:white;
display:flex;
flex-direction:column;
justify-content:center;
border-bottom:1px solid rgba(255,255,255,.06);
}

.topbar{
display:flex;
justify-content:space-between;
align-items:center;
margin-bottom:10px;
font-size:14px;
font-weight:600;
padding:0 2px;
}

.icons-ios{
font-size:12px;
letter-spacing:2px;
opacity:.9;
}

.header-content{
display:flex;
align-items:center;
}

.profile{
width:45px;
height:45px;
border-radius:50%;
background:#2c2c2e;
display:flex;
justify-content:center;
align-items:center;
font-size:22px;
margin-right:12px;
}

.name{
font-size:16px;
font-weight:600;
}

.status{
font-size:12px;
color:#aaa;
}

/* CHAT */

.chat-area{
height:calc(100vh - 95px);
overflow-y:auto;
padding:20px 14px 120px;

background:
linear-gradient(rgba(0,0,0,.55),rgba(0,0,0,.55)),
url('https://images.unsplash.com/photo-1516589091380-5d8e87df6999?q=80&w=1200&auto=format&fit=crop');

background-size:cover;
background-position:center;
}

.message{
max-width:78%;
padding:12px 16px;
margin-bottom:12px;
font-size:15px;
line-height:1.5;
display:none;
animation:show .35s ease;
position:relative;
backdrop-filter:blur(10px);
}

.message-time{
font-size:10px;
opacity:.7;
margin-top:4px;
text-align:right;
}

.sent{
background:#0A7CFF;
color:white;
margin-left:auto;
border-radius:22px 22px 6px 22px;
box-shadow:0 2px 10px rgba(10,124,255,.25);
}

.received{
background:#2c2c2e;
color:white;
border-radius:22px 22px 22px 6px;
}

.typing{
display:none;
background:#2c2c2e;
padding:10px 15px;
border-radius:20px;
width:70px;
margin-bottom:12px;
}

.dot{
width:8px;
height:8px;
background:#aaa;
border-radius:50%;
display:inline-block;
animation:blink 1.2s infinite;
}

.dot:nth-child(2){
animation-delay:.2s;
}

.dot:nth-child(3){
animation-delay:.4s;
}

@keyframes blink{
0%{opacity:.2}
20%{opacity:1}
100%{opacity:.2}
}

@keyframes show{
from{
opacity:0;
transform:translateY(10px);
}
to{
opacity:1;
transform:translateY(0);
}
}

/* INVITATION */

.invitation{
display:none;
background:rgba(255,255,255,.96);
backdrop-filter:blur(20px);
padding:30px;
border-radius:30px;
text-align:center;
margin-top:30px;
animation:show 1s ease;
}

.invitation h1{
font-size:32px;
margin-bottom:10px;
color:#111;
}

.invitation p{
color:#333;
line-height:1.8;
}

.button{
display:inline-block;
margin-top:20px;
padding:12px 24px;
background:#111;
color:white;
text-decoration:none;
border-radius:999px;
font-size:14px;
}

.fade{
opacity:.8;
font-size:14px;
margin-top:10px;
}

</style>
</head>

<body>

<!-- OPENING -->

<div id="opening">

<h1>Abdul & Syahrillah</h1>
<p>A Wedding Invitation</p>

<button id="openBtn">
Buka Undangan
</button>

</div>

<!-- PHONE -->

<div class="phone" id="phone">

<div class="header">

<div class="topbar">
<div>23.09</div>
<div class="icons-ios">📶 🔋</div>
</div>

<div class="header-content">

<div class="profile">💍</div>

<div>
<div class="name">Syahrillah ❤️</div>
<div class="status">online</div>
</div>

</div>

</div>

<div class="chat-area" id="chatArea">

<div class="message sent">
kamu belum tidur?
<div class="message-time">23.09</div>
</div>

<div class="typing">
<span class="dot"></span>
<span class="dot"></span>
<span class="dot"></span>
</div>

<div class="message received">
belum hehe, kenapa?
<div class="message-time">23.09</div>
</div>

<div class="message sent">
aku lagi mikir
<div class="message-time">23.10</div>
</div>

<div class="typing">
<span class="dot"></span>
<span class="dot"></span>
<span class="dot"></span>
</div>

<div class="message received">
tumben serius 😭
<div class="message-time">23.10</div>
</div>

<div class="message sent">
ga kerasa ya kita udah sejauh ini
<div class="message-time">23.10</div>
</div>

<div class="message received">
iyaa 🥺
<div class="message-time">23.10</div>
</div>

<div class="message sent">
makasih ya udah bertahan sejauh ini
<div class="message-time">23.11</div>
</div>

<div class="typing">
<span class="dot"></span>
<span class="dot"></span>
<span class="dot"></span>
</div>

<div class="message received">
jadi terharu :(
<div class="message-time">23.11</div>
</div>

<div class="message sent">
jadi...
<div class="message-time">23.11</div>
</div>

<div class="message sent">
lanjut hidup bareng terus yuk
<div class="message-time">23.11</div>
</div>

<div class="typing">
<span class="dot"></span>
<span class="dot"></span>
<span class="dot"></span>
</div>

<div class="message received">
ke pelaminan?
<div class="message-time">23.12</div>
</div>

<div class="message sent">
iya 🤍
<div class="message-time">23.12</div>
</div>

<!-- INVITATION -->

<div class="invitation" id="invite">

<h1>Abdul & Syahrillah</h1>

<p>
Dengan penuh kebahagiaan,<br>
kami mengundang Anda<br>
untuk hadir di hari pernikahan kami.
</p>

<br>

<p>
<strong>Selasa, 20 Juli 2027</strong><br>
08.00 WIB
</p>

<br>

<p>
📍 Kediaman Mempelai Wanita<br>
Jl. Penamas No.32,<br>
Sonosari, Kebonagung,<br>
Pakisaji, Malang
</p>

<a href="https://www.google.com/maps/place/Jl.+Penamas+No.32,+Sonosari,+Kebonagung,+Kec.+Pakisaji,+Kabupaten+Malang,+Jawa+Timur+65162/@-8.0346205,112.6073664,19.83z/data=!4m6!3m5!1s0x2e789d70062432e9:0xa2901c7369fabbbc!8m2!3d-8.0347719!4d112.6077009!16s%2Fg%2F11y3317l61?entry=ttu&g_ep=EgoyMDI2MDUwMi4wIKXMDSoASAFQAw%3D%3D"
class="button" target="_blank">

Buka Maps

</a>

<div class="fade">
“And suddenly, all the love songs were about you.”
</div>

</div>

</div>

</div>

<!-- SOUND -->

<audio id="chatSound">
<source src="assets.mixkit.co/active_storage/sfx/2354/2354-preview.mp3" type="audio/mpeg">
</audio>

<audio id="music" loop>
<source src="https://files.catbox.moe/0wfhli.mp3" type="audio/mpeg">
</audio>

<script>

const openBtn = document.getElementById('openBtn');
const opening = document.getElementById('opening');
const phone = document.getElementById('phone');

const chatArea = document.getElementById('chatArea');
const messages = document.querySelectorAll('.message');
const typings = document.querySelectorAll('.typing');
const invite = document.getElementById('invite');

const chatSound = document.getElementById('chatSound');
const music = document.getElementById('music');

openBtn.addEventListener('click', async ()=>{

opening.style.display='none';
phone.style.display='block';

/* START MUSIC DIAM-DIAM */
music.volume = 0;

try{
await music.play();
}catch(e){
console.log(e);
}

let delay = 1000;

messages.forEach((msg,index)=>{

setTimeout(()=>{

msg.style.display='block';

chatSound.currentTime = 0;
chatSound.play();

chatArea.scrollTop = chatArea.scrollHeight;

},delay);

delay += 1800;

if(typings[index]){

setTimeout(()=>{
typings[index].style.display='block';
chatArea.scrollTop = chatArea.scrollHeight;
},delay-900);

setTimeout(()=>{
typings[index].style.display='none';
},delay);

}

});

setTimeout(()=>{

invite.style.display='block';

/* NAIKKAN VOLUME PAS UNDANGAN MUNCUL */
music.volume = 0.45;

chatArea.scrollTop = chatArea.scrollHeight;

},delay+1200);

});

</script>

</body>
</html>
