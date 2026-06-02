<html lang="en">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>SLC | Shree Lakshmi & Co</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
scroll-behavior:smooth;
}

body{
background:black;
color:white;
overflow-x:hidden;
}

/* VIDEO */

#bgvideo{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
object-fit:cover;
z-index:-2;
filter:brightness(0.35);
}

.overlay{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:
linear-gradient(
rgba(0,0,0,0.72),
rgba(60,0,0,0.82)
);
z-index:-1;
}

/* HEADER */

header{
position:fixed;
top:0;
left:0;
width:100%;
padding:18px 8%;
display:flex;
justify-content:space-between;
align-items:center;
background:rgba(0,0,0,0.4);
backdrop-filter:blur(14px);
z-index:1000;
border-bottom:1px solid rgba(255,204,0,0.2);
}

.logo{
font-size:48px;
font-weight:800;
color:#ffcc00;
letter-spacing:2px;
animation:logoGlow 2s infinite alternate;
}

@keyframes logoGlow{

from{

text-shadow:
0 0 10px #ffcc00,
0 0 30px red;

}

to{

text-shadow:
0 0 20px #ffcc00,
0 0 50px #ffcc00,
0 0 100px red,
0 0 160px red;

}

}

nav{
display:flex;
gap:25px;
}

nav a{
text-decoration:none;
color:white;
font-weight:600;
transition:0.3s;
}

nav a:hover{
color:#ffcc00;
text-shadow:0 0 10px #ffcc00;
}

/* HERO */

.hero{
min-height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:130px 20px;
}

.hero h1{
font-size:92px;
font-weight:800;
color:#ffcc00;
line-height:1.1;
animation:heroGlow 2s infinite alternate;
}

@keyframes heroGlow{

from{

transform:translateY(0px);

text-shadow:
0 0 20px #ffcc00,
0 0 40px red;

}

to{

transform:translateY(-8px);

text-shadow:
0 0 30px #ffcc00,
0 0 60px #ffcc00,
0 0 120px red,
0 0 200px red;

}

}

.hero p{
margin-top:25px;
font-size:24px;
max-width:900px;
line-height:1.8;
color:#ddd;
}

/* SEARCH */

.searchBox{
margin-top:45px;
display:flex;
width:100%;
max-width:1000px;
background:rgba(255,255,255,0.08);
border-radius:60px;
padding:10px;
backdrop-filter:blur(14px);
border:1px solid rgba(255,204,0,0.2);

box-shadow:
0 0 30px rgba(255,204,0,0.25),
0 0 60px rgba(255,0,0,0.35),
0 0 120px rgba(255,0,0,0.2);

}

.searchBox input{
flex:1;
padding:20px 24px;
background:transparent;
border:none;
outline:none;
color:white;
font-size:18px;
}

.searchBox input::placeholder{
color:#ccc;
}

.searchBox button{
padding:18px 36px;
border:none;
border-radius:50px;
background:linear-gradient(to right,#ff0000,#ffcc00);
font-size:17px;
font-weight:700;
cursor:pointer;
transition:0.3s;

box-shadow:
0 0 20px red,
0 0 40px #ffcc00;

}

.searchBox button:hover{
transform:scale(1.05);
}

/* RESULT */

#result{
display:none;
margin-top:40px;
width:100%;
max-width:1100px;
padding:35px;
border-radius:30px;
background:rgba(255,255,255,0.08);
backdrop-filter:blur(16px);
border:1px solid rgba(255,204,0,0.2);

box-shadow:
0 0 30px rgba(255,204,0,0.2),
0 0 70px rgba(255,0,0,0.35),
0 0 130px rgba(255,0,0,0.2);

animation:fade 0.4s ease;
}

@keyframes fade{

from{
opacity:0;
transform:translateY(20px);
}

to{
opacity:1;
transform:translateY(0);
}

}

/* ABOUT SECTION */

.about{
padding:120px 8%;
text-align:center;
}

.aboutTitle{
font-size:68px;
color:#ffcc00;
margin-bottom:70px;

text-shadow:
0 0 20px #ffcc00,
0 0 50px red,
0 0 100px red;

animation:aboutGlow 2s infinite alternate;
}

@keyframes aboutGlow{

from{

text-shadow:
0 0 20px #ffcc00,
0 0 50px red;

}

to{

text-shadow:
0 0 30px #ffcc00,
0 0 70px #ffcc00,
0 0 130px red,
0 0 180px red;

}

}

.cards{
display:flex;
justify-content:center;
flex-wrap:wrap;
gap:35px;
}

.card{
width:320px;
padding:40px;
border-radius:30px;
background:rgba(255,255,255,0.08);
backdrop-filter:blur(14px);
border:1px solid rgba(255,204,0,0.15);

transition:0.4s;

box-shadow:
0 0 20px rgba(255,204,0,0.15),
0 0 50px rgba(255,0,0,0.15);

}

.card:hover{

transform:translateY(-12px) scale(1.04);

box-shadow:
0 0 30px #ffcc00,
0 0 80px red,
0 0 150px red;

}

.card h2{
color:#ffcc00;
margin-bottom:20px;
font-size:30px;

text-shadow:
0 0 10px #ffcc00,
0 0 30px red;

}

.card p{
line-height:1.9;
color:#ddd;
font-size:17px;
}

/* CONTACT */

.contact{
padding:120px 20px;
text-align:center;
}

.contact h2{
font-size:65px;
color:#ffcc00;
margin-bottom:20px;

text-shadow:
0 0 20px #ffcc00,
0 0 60px red,
0 0 120px red;

}

.contact p{
font-size:21px;
margin-bottom:35px;
}

.buttons{
display:flex;
justify-content:center;
gap:20px;
flex-wrap:wrap;
}

.buttons a{
padding:18px 34px;
border-radius:50px;
text-decoration:none;
font-size:18px;
font-weight:700;
transition:0.3s;
}

.call{
background:red;
color:white;

box-shadow:
0 0 20px red,
0 0 50px red;

}

.whatsapp{
background:#25D366;
color:white;

box-shadow:
0 0 20px #25D366,
0 0 50px #25D366;

}

.buttons a:hover{
transform:scale(1.08);
}

.address{
margin-top:40px;
font-size:18px;
line-height:2;
color:#ddd;
}

footer{
padding:30px;
text-align:center;
color:#aaa;
background:black;
}

/* MOBILE */

@media(max-width:768px){

.hero h1{
font-size:55px;
}

.hero p{
font-size:18px;
}

.aboutTitle{
font-size:45px;
}

.contact h2{
font-size:45px;
}

nav{
display:none;
}

.searchBox{
flex-direction:column;
border-radius:30px;
}

.searchBox button{
width:100%;
}

}

</style>

</head>

<body>

<!-- VIDEO -->

<video autoplay muted loop playsinline id="bgvideo">

<source src="https://assets.mixkit.co/videos/preview/mixkit-industrial-smoke-coming-out-from-a-factory-1561-large.mp4" type="video/mp4">

</video>

<div class="overlay"></div>

<!-- HEADER -->

<header>

<div class="logo">SLC</div>

<nav>

<a href="#">Home</a>
<a href="#about">About</a>
<a href="#contact">Contact</a>

</nav>

</header>

<!-- HERO -->

<section class="hero">

<h1>Shree Lakshmi & Co</h1>

<p>
Premium Iron & Steel Solutions Powered by SLC AI Technology
</p>

<div class="searchBox">

<input
type="text"
id="searchInput"
placeholder="Search 9mm rod, beam, channel, pipe, gi sheet...">

<button onclick="searchMaterial()">

Search

</button>

</div>

<div id="result"></div>

</section>

<!-- ABOUT -->

<section class="about" id="about">

<h1 class="aboutTitle">
Why Choose SLC?
</h1>

<div class="cards">

<div class="card">

<h2>Premium Steel</h2>

<p>
Industrial quality iron and steel products with maximum durability and performance.
</p>

</div>

<div class="card">

<h2>SLC AI Search</h2>

<p>
Search 50+ materials instantly with sizes, features and industrial applications.
</p>

</div>

<div class="card">

<h2>Trusted Supply</h2>

<p>
Fast delivery, modern infrastructure and trusted steel distribution across projects.
</p>

</div>

</div>

</section>

<!-- CONTACT -->

<section class="contact" id="contact">

<h2>Contact SLC</h2>

<p>
Call or WhatsApp instantly for enquiries and orders.
</p>

<div class="buttons">

<a
class="call"
href="tel:+919841282311">

📞 Call Now

</a>

<a
class="whatsapp"
href="https://wa.me/919841282311"
target="_blank">

💬 WhatsApp

</a>

</div>

<div class="address">

Vaikund<br>
11/10 108, Canal Bank Rd,<br>
Rukmani Nagar, Adyar,<br>
Chennai, Tamil Nadu 600020

</div>

</section>

<footer>

© 2026 SLC | Shree Lakshmi & Co

</footer>

<script>

const materials = {};

const sizes = [
"5mm","6mm","7mm","8mm","9mm","10mm","11mm","12mm",
"13mm","14mm","15mm","16mm","17mm","18mm","19mm","20mm",
"21mm","22mm","23mm","24mm","25mm","26mm","27mm","28mm",
"29mm","30mm","32mm","35mm","40mm","45mm","50mm"
];

for(let i=0;i<sizes.length;i++){

let size = sizes[i];

materials[size + " rod"] = {

title:size + " Steel Rod",

sizes:size,

features:[
"High tensile strength",
"Industrial grade steel",
"Corrosion resistant",
"Heavy construction ready",
"Reliable support"
],

uses:[
"Buildings",
"Concrete reinforcement",
"Industrial structures",
"Structural support"
]

};

}

Object.assign(materials,{

"channel":{
title:"Steel Channels",
sizes:"75mm × 40mm to 400mm × 110mm",
features:[
"Strong structural support",
"Industrial strength",
"Heavy load distribution"
],
uses:[
"Frameworks",
"Warehouses",
"Vehicle chassis"
]
},

"beam":{
title:"Universal Beams",
sizes:"127mm × 76mm to 1016mm × 305mm",
features:[
"Heavy load support",
"High bending resistance",
"Industrial grade"
],
uses:[
"Bridges",
"Steel buildings",
"Industrial floors"
]
},

"pipe":{
title:"Steel Pipes",
sizes:"1/8 inch to 26 inch",
features:[
"Leak resistant",
"Heavy duty",
"Long lasting"
],
uses:[
"Water supply",
"Gas pipelines",
"Industrial transport"
]
},

"sheet":{
title:"Steel Sheets",
sizes:"0.3mm to 6mm",
features:[
"Smooth surface",
"Industrial grade",
"Easy cutting"
],
uses:[
"Roofing",
"Furniture",
"Containers"
]
},

"tmt bar":{
title:"TMT Bars",
sizes:"6mm to 50mm",
features:[
"Earthquake resistant",
"Fire resistant",
"Corrosion resistant"
],
uses:[
"Buildings",
"Bridges",
"Flyovers"
]
}

});

function searchMaterial(){

let input =
document.getElementById("searchInput")
.value
.toLowerCase()
.trim();

let result =
document.getElementById("result");

if(materials[input]){

let data = materials[input];

let featuresHTML = "";
let usesHTML = "";

for(let i=0;i<data.features.length;i++){

featuresHTML += "<li>" + data.features[i] + "</li>";

}

for(let i=0;i<data.uses.length;i++){

usesHTML += "<li>" + data.uses[i] + "</li>";

}

result.innerHTML =

"<h1 style='color:#ffcc00;font-size:50px;margin-bottom:20px;text-shadow:0 0 20px red;'>" +

data.title +

"</h1>" +

"<h2 style='color:red;margin-bottom:15px;'>Available Sizes</h2>" +

"<p style='font-size:20px;margin-bottom:25px;'>" +

data.sizes +

"</p>" +

"<h2 style='color:#ffcc00;margin-bottom:15px;'>Features</h2>" +

"<ul style='line-height:2;font-size:18px;padding-left:25px;margin-bottom:25px;'>" +

featuresHTML +

"</ul>" +

"<h2 style='color:red;margin-bottom:15px;'>Applications / Uses</h2>" +

"<ul style='line-height:2;font-size:18px;padding-left:25px;'>" +

usesHTML +

"</ul>";

}else{

result.innerHTML =

"<h1 style='color:#ffcc00;'>SLC AI Assistant</h1>" +

"<p style='margin-top:20px;font-size:18px;line-height:2;'>" +

"Material not found.<br><br>" +

"Try searching:<br><br>" +

Object.keys(materials).map(x=>"• "+x).join("<br>");

}

result.style.display = "block";

}

document.getElementById("searchInput")
.addEventListener("keypress",function(e){

if(e.key==="Enter"){

searchMaterial();

}

});

</script>

</body>
</html>
