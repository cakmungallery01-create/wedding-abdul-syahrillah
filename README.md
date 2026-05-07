
<!DOCTYPE html>
<html lang="id">

<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">

<title>Abdul & Syahrillah</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
-webkit-tap-highlight-color:transparent;
}

html,body{
width:100%;
height:100%;
overflow:hidden;
font-family:'Poppins',sans-serif;
background:#000;
}

/* OPENING */

#opening{
position:fixed;
inset:0;
z-index:999999;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:30px;
color:white;

background:
linear-gradient(rgba(0,0,0,.55),rgba(0,0,0,.55)),
url('https://images.unsplash.com/photo-1519741497674-611481863552?q=80&w=1200&auto=format&fit=crop');

background-size:cover;
background-position:center;

transition:1s;
}

#opening.hide{
opacity:0;
pointer-events:none;
}

#opening h1{
font-size:42px;
font-weight:700;
margin-bottom:10px;
}

#opening p{
font-size:15px;
opacity:.9;
}

#openBtn{
margin-top:28px;
padding:15px 34px;
border:none;
border-radius:999px;
background:white;
color:black;
font-size:15px;
font-weight:600;
cursor:pointer;
transition:.2s;
}

#openBtn:active{
transform:scale(.95);
}

/* PHONE */

.phone{
position:relative;
width:100%;
max-width:430px;
height:100dvh;
margin:auto;
background:#000;
overflow:hidden;
display:none;
border-radius:40px;
box-shadow:0 0 40px rgba(0,0,0,.5);
}

/* DYNAMIC ISLAND */

.phone::before{
content:'';
position:absolute;
top:12px;
left:50%;
transform:translateX(-50%);
width:126px;
height:34px;
border-radius:40px;
background:#000;
z-index:999;
}

/* HEADER */

.header{
position:relative;
z-index:5;

height:95px;
padding:14px 16px 10px;

background:rgba(20,20,20,.88);
backdrop-filter:blur(25px);

border-bottom:1px solid rgba(255,255,255,.06);

color:white;
}

.topbar{
display:flex;
justify-content:space-between;
align-items:center;
font-size:13px;
font-weight:600;
padding:0 4px;
margin-bottom:14px;
}

.icons{
font-size:12px;
opacity:.9;
}

.header-content{
display:flex;
align-items:center;
}

.profile{
width:42px;
height:42px;
border-radius:50%;
background:#2c2c2e;

display:flex;
justify-content:center;
align-items:center;

font-size:20px;
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

/* CHAT AREA */

.chat-area{
height:calc(100dvh - 95px);
overflow-y:auto;

padding:18px 12px 120px;

scroll-behavior:smooth;

background:
linear-gradient(rgba(0,0,0,.45),rgba(0,0,0,.45)),
url('https://images.unsplash.com/photo-1516589091380-5d8e87df6999?q=80&w=1200&auto=format&fit=crop');

background-size:cover;
background-position:center;
}

.chat-area::-webkit-scrollbar{
display:none;
}

/* MESSAGE */

.message{
display:none;
max-width:78%;

padding:10px 14px 6px;

margin-bottom:8px;

font-size:15px;
line-height:1.45;

animation:show .35s ease;
}

.sent{
margin-left:auto;

background:#0A84FF;
color:white;

border-radius:22px 22px 6px 22px;

box-shadow:0 3px 12px rgba(10,132,255,.25);
}

.received{
background:#2c2c2e;
color:white;

border-radius:22px 22px 22px 6px;
}

.message-time{
font-size:10px;
opacity:.72;
margin-top:4px;
text-align:right;
}

/* TYPING */

.typing{
display:none;

background:#2c2c2e;

width:74px;

padding:10px 14px;

border-radius:20px;

margin-bottom:10px;

animation:show .3s ease;
}

.dot{
width:7px;
height:7px;

background:#aaa;

border-radius:50%;

display:inline-block;

margin-right:3px;

animation:blink 1.2s infinite;
}

.dot:nth-child(2){
animation-delay:.2s;
}

.dot:nth-child(3){
animation-delay:.4s;
}

@keyframes blink{

0%{
opacity:.25;
transform:translateY(0);
}

50%{
opacity:1;
transform:translateY(-2px);
}

100%{
opacity:.25;
transform:translateY(0);
}

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

background:rgba(255,255,255,.97);

backdrop-filter:blur(30px);

padding:32px 28px;

border-radius:34px;

text-align:center;

margin-top:26px;

animation:show .8s ease;

box-shadow:0 15px 40px rgba(0,0,0,.35);
}

.invitation h1{
font-size:32px;
margin-bottom:12px;
color:#111;
}

.invitation p{
font-size:15px;
line-height:1.8;
color:#333;
}

.button{
display:inline-block;

margin-top:20px;

padding:14px 24px;

border-radius:999px;

background:#111;
color:white;

text-decoration:none;

font-size:14px;
font-weight:600;
}

.fade{
margin-top:16px;
font-size:13px;
opacity:.7;
font-style:italic;
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

<!-- HEADER -->

<div class="header">

<div class="topbar">
<div>23.09</div>
<div class="icons">📶 5G 🔋</div>
</div>

<div class="header-content">

<div class="profile">💍</div>

<div>
<div class="name">Syahrillah ❤️</div>
<div class="status">online</div>
</div>

</div>

</div>

<!-- CHAT -->

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

<a href="https://maps.google.com" class="button" target="_blank">
Buka Maps
</a>

<div class="fade">
“And suddenly, all the love songs were about you.”
</div>

</div>

</div>

</div>

<!-- AUDIO -->

<audio id="chatSound" preload="auto">
<source src="https://assets.mixkit.co/active_storage/sfx/2354/2354-preview.mp3" type="audio/mpeg">
</audio>

<audio id="music" preload="auto" loop playsinline webkit-playsinline>
<source src="https://files.catbox.moe/0wfhli.mp3" type="audio/mpeg">
</audio>

<script>

const openBtn = document.getElementById('openBtn');
const opening = document.getElementById('opening');
const phone = document.getElementById('phone');

const messages = document.querySelectorAll('.message');
const typings = document.querySelectorAll('.typing');

const invite = document.getElementById('invite');

const chatArea = document.getElementById('chatArea');

const chatSound = document.getElementById('chatSound');
const music = document.getElementById('music');

openBtn.addEventListener('click', ()=>{

phone.style.display='block';

opening.classList.add('hide');

let delay = 1000;

/* MESSAGE FLOW */

messages.forEach((msg,index)=>{

if(index > 0){

setTimeout(()=>{

if(typings[index-1]){

typings[index-1].style.display='block';

chatArea.scrollTop = chatArea.scrollHeight;

}

},delay - 900);

setTimeout(()=>{

if(typings[index-1]){

typings[index-1].style.display='none';

}

},delay - 200);

}

setTimeout(()=>{

msg.style.display='block';

chatSound.currentTime = 0;

chatSound.play().catch(()=>{});

chatArea.scrollTop = chatArea.scrollHeight;

},delay);

delay += 1900;

});

/* SHOW INVITATION */

setTimeout(async ()=>{

invite.style.display='block';

chatArea.scrollTop = chatArea.scrollHeight;

/* MUSIC */

music.volume = 0;

try{

await music.play();

let volume = 0;

const fade = setInterval(()=>{

volume += 0.02;

if(volume >= 0.45){

volume = 0.45;

clearInterval(fade);

}

music.volume = volume;

},120);

}catch(err){

console.log(err);

}

},delay + 1000);

});

</script>

</body>
</html>
