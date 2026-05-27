<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>تهنئة عيد الأضحى المبارك</title>

<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;900&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Cairo',sans-serif;
}

body{
min-height:100vh;
display:flex;
justify-content:center;
align-items:center;
background:
linear-gradient(rgba(0,0,0,.45),rgba(0,0,0,.45)),
url('https://images.unsplash.com/photo-1564769625905-50e93615e769?q=80&w=1600&auto=format&fit=crop');
background-size:cover;
background-position:center;
overflow:hidden;
}

.card{
width:90%;
max-width:700px;
padding:40px 25px;
border-radius:30px;
background:rgba(255,255,255,.08);
backdrop-filter:blur(12px);
border:1px solid rgba(255,255,255,.15);
text-align:center;
color:#fff;
box-shadow:0 15px 40px rgba(0,0,0,.35);
}

.moon{
font-size:80px;
animation:float 3s ease-in-out infinite;
}

@keyframes float{
0%,100%{transform:translateY(0)}
50%{transform:translateY(-12px)}
}

h1{
font-size:2.5rem;
margin:15px 0;
color:#ffd54f;
}

.subtitle{
font-size:1.3rem;
font-weight:700;
margin-bottom:20px;
}

.message{
line-height:2;
font-size:1.1rem;
margin-top:15px;
}

.name{
margin-top:30px;
font-size:1.5rem;
font-weight:900;
color:#ffd54f;
}

.btn{
display:inline-block;
margin-top:30px;
padding:14px 35px;
border:none;
border-radius:50px;
background:#ffd54f;
color:#111;
font-weight:900;
font-size:1rem;
cursor:pointer;
transition:.3s;
}

.btn:hover{
transform:scale(1.05);
}

.stars{
position:absolute;
inset:0;
pointer-events:none;
}

.star{
position:absolute;
color:white;
animation:blink 2s infinite;
}

@keyframes blink{
0%,100%{opacity:.2}
50%{opacity:1}
}
</style>
</head>
<body>

<div class="stars">
<div class="star" style="top:10%;left:15%">✦</div>
<div class="star" style="top:20%;left:80%">✦</div>
<div class="star" style="top:70%;left:10%">✦</div>
<div class="star" style="top:80%;left:85%">✦</div>
<div class="star" style="top:40%;left:92%">✦</div>
<div class="star" style="top:15%;left:55%">✦</div>
</div>

<div class="card">

<div class="moon">🌙</div>

<h1>عيد أضحى مبارك</h1>

<div class="subtitle">

</div>

<div class="message">
بمناسبة عيد الأضحى المبارك،
أتقدم إليكم بأطيب التهاني وأصدق الأمنيات.

أسأل الله أن يجعل أيامكم مليئة بالسعادة والبركة،
وأن يتقبل منكم صالح الأعمال والطاعات،
وأن يديم عليكم الصحة والعافية والرزق الوفير.

كل عام وأنتم بخير،
وعيدكم مبارك،
وأعاده الله عليكم بالخير واليمن والبركات.
</div>

<div class="name">
محمد صلاح
</div>

<button class="btn" onclick="shareGreeting()">
مشاركة التهنئة
</button>

</div>

<script>
function shareGreeting(){

const text = `
🌙 عيد أضحى مبارك 🌙

إلى الأهل والأقارب والمعارف والأحباب ❤️

كل عام وأنتم بخير وعيدكم مبارك.

تهنئة من محمد صلاح
`;

if(navigator.share){
navigator.share({
title:'عيد أضحى مبارك',
text:text
});
}else{
navigator.clipboard.writeText(text);
alert('تم نسخ التهنئة بنجاح');
}
}
</script>

</body>
</html># -
