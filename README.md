# AMRI-BONUS
<!DOCTYPE html>
<html lang="ro">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bonus Casino România</title>

<style>
body{
    margin:0;
    padding:0;
    font-family:Arial,sans-serif;
    background:#0b1020;
    color:white;
    overflow-x:hidden;
}

.container{
    max-width:420px;
    margin:auto;
    padding:20px;
    text-align:center;
}

.logo{
    font-size:32px;
    font-weight:bold;
    color:#ffd700;
    margin-top:20px;
}

.badge{
    display:inline-block;
    background:#22c55e;
    padding:8px 18px;
    border-radius:30px;
    margin-top:15px;
    font-weight:bold;
}

h1{
    font-size:34px;
    margin-top:25px;
    line-height:1.2;
}

.subtitle{
    margin-top:20px;
    font-size:19px;
    opacity:0.9;
}

.bonus-box{
    background:#111827;
    border:2px solid #22c55e;
    border-radius:18px;
    padding:20px;
    margin-top:30px;
}

.bonus-title{
    font-size:24px;
    color:#ffd700;
    font-weight:bold;
}

.bonus-text{
    margin-top:12px;
    font-size:18px;
}

.timer{
    margin-top:20px;
    font-size:18px;
    color:#ff4d4d;
    font-weight:bold;
}

.features{
    margin-top:30px;
    text-align:left;
}

.feature{
    background:#111827;
    padding:14px;
    border-radius:12px;
    margin-bottom:12px;
    font-size:17px;
}

.cta{
    display:block;
    margin-top:35px;
    background:#22c55e;
    color:white;
    text-decoration:none;
    padding:20px;
    border-radius:14px;
    font-size:24px;
    font-weight:bold;
    animation:pulse 1.2s infinite;
}

@keyframes pulse{
    0%{transform:scale(1);}
    50%{transform:scale(1.05);}
    100%{transform:scale(1);}
}

.people{
    margin-top:20px;
    opacity:0.85;
    font-size:16px;
}

.warning{
    margin-top:30px;
    font-size:13px;
    opacity:0.5;
}

.popup{
    position:fixed;
    bottom:20px;
    left:50%;
    transform:translateX(-50%);
    background:#111827;
    padding:12px 18px;
    border-radius:12px;
    font-size:15px;
    border:1px solid #22c55e;
    animation:fadein 0.5s;
}

@keyframes fadein{
    from{opacity:0; bottom:0;}
    to{opacity:1; bottom:20px;}
}
</style>
</head>

<body>

<div class="container">

<div class="logo">
🎰 CASINO RO
</div>

<div class="badge">
BONUS ACTIV ASTĂZI
</div>

<h1>
Primești până la 500 RON + 150 Rotiri Gratuite
</h1>

<div class="subtitle">
Doar pentru utilizatorii din România.
Activare în mai puțin de 1 minut.
</div>

<div class="bonus-box">
<div class="bonus-title">
🎁 BONUS EXCLUSIV
</div>

<div class="bonus-text">
Depozit minim: 20 RON
</div>

<div class="timer" id="timer">
Oferta expiră în: 09:59
</div>
</div>

<div class="features">

<div class="feature">
⚡ Retrageri rapide
</div>

<div class="feature">
📱 Funcționează pe Android & iPhone
</div>

<div class="feature">
🔒 Înregistrare securizată
</div>

<div class="feature">
🎲 Sloturi și jocuri live
</div>

</div>

<a href="https://1wthlj.life/casino?p=ekxe" class="cta" target="_blank">
ACTIVEAZĂ BONUSUL
</a>

<div class="people">
🔥 127 persoane activează bonusul chiar acum
</div>

<div class="warning">
18+ | Joacă responsabil.
</div>

</div>

<div class="popup" id="popup">
🎉 Andrei din București a activat bonusul
</div>

<script>
let time = 599;

setInterval(() => {
    let minutes = Math.floor(time / 60);
    let seconds = time % 60;

    if(seconds < 10){
        seconds = "0" + seconds;
    }

    document.getElementById("timer").innerHTML =
    "Oferta expiră în: " + minutes + ":" + seconds;

    if(time > 0){
        time--;
    }

},1000);

const names = [
"Andrei din București",
"Alex din Cluj",
"Daniel din Iași",
"Robert din Timișoara",
"Mihai din Constanța"
];

setInterval(() => {
    const randomName =
    names[Math.floor(Math.random() * names.length)];

    document.getElementById("popup").innerHTML =
    "🎉 " + randomName + " a activat bonusul";

},4000);
</script>

</body>
</html>