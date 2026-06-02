
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
rgba(0,0,0,0.7),
rgba(50,0,0,0.82)
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
backdrop-filter:blur(12px);
z-index:1000;
border-bottom:1px solid rgba(255,204,0,0.15);
}

.logo{
font-size:46px;
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
0 0 90px red,
0 0 140px red;
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
0 0 180px red;
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
0 0 25px rgba(255,204,0,0.25),
0 0 50px rgba(255,0,0,0.3),
0 0 100px rgba(255,0,0,0.2);
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
0 0 60px rgba(255,0,0,0.35),
0 0 120px rgba(255,0,0,0.2);
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

/* CARDS */

.cards{
display:flex;
justify-content:center;
flex-wrap:wrap;
gap:30px;
padding:100px 8%;
}

.card{
width:320px;
padding:35px;
border-radius:30px;
background:rgba(255,255,255,0.08);
backdrop-filter:blur(14px);
border:1px solid rgba(255,204,0,0.12);
transition:0.4s;
box-shadow:
0 0 20px rgba(255,204,0,0.1),
0 0 40px rgba(255,0,0,0.1);
}

.card:hover{
transform:translateY(-10px) scale(1.03);
box-shadow:
0 0 30px #ffcc00,
0 0 70px red,
0 0 130px red;
}

.card h2{
color:#ffcc00;
margin-bottom:18px;
font-size:30px;
}

.card p{
line-height:1.9;
color:#ddd;
}

/* CONTACT */

.contact{
padding:110px 20px;
text-align:center;
}

.contact h2{
font-size:60px;
color:#ffcc00;
margin-bottom:20px;
text-shadow:
0 0 20px #ffcc00,
0 0 50px red;
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
box-shadow:0 0 25px red;
}

.whatsapp{
background:#25D366;
color:white;
box-shadow:0 0 25px #25D366;
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
font-size:54px;
}

.hero p{
font-size:18px;
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
placeholder="Search 9mm rod, channel, beam, pipe, gi sheet...">

<button onclick="searchMaterial()">
Search
</button>

</div>

<div id="result"></div>

</section>

<!-- ABOUT -->

<section class="cards" id="about">

<div class="card">
<h2>Premium Steel</h2>
<p>
Industrial quality iron and steel materials for every construction project.
</p>
</div>

<div class="card">
<h2>SLC AI Search</h2>
<p>
Search materials instantly with sizes, features and applications.
</p>
</div>

<div class="card">
<h2>Trusted Supply</h2>
<p>
Reliable delivery and modern industrial steel solutions.
</p>
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
"Reliable support",
"Heavy construction ready"
],

uses:[
"Buildings",
"Concrete reinforcement",
"Industrial projects",
"Structural support"
]

};

}

/* EXTRA MATERIALS */

Object.assign(materials,{

"channel":{
title:"Steel Channels",
sizes:"75mm × 40mm to 400mm × 110mm",
features:[
"Strong structural support",
"Heavy load distribution",
"Industrial strength"
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
"High bending resistance",
"Heavy load support",
"Industrial grade"
],
uses:[
"Bridges",
"Steel buildings",
"Industrial floors"
]
},

"column":{
title:"Universal Columns",
sizes:"152mm × 152mm to 356mm × 406mm",
features:[
"Extreme vertical support",
"Earthquake resistant",
"Heavy duty"
],
uses:[
"Building columns",
"Industrial sheds",
"Towers"
]
},

"angle":{
title:"Steel Angles",
sizes:"20mm × 20mm to 250mm × 250mm",
features:[
"Strong corner support",
"Easy fabrication",
"High durability"
],
uses:[
"Roof trusses",
"Cell towers",
"Structural framing"
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

"gi pipe":{
title:"GI Pipes",
sizes:"15mm to 300mm",
features:[
"Rust resistant",
"Outdoor ready",
"Strong piping"
],
uses:[
"Handrails",
"Water lines",
"Scaffolding"
]
},

"erw pipe":{
title:"ERW Pipes",
sizes:"15mm to 600mm",
features:[
"Strong welded joints",
"Reliable quality",
"Industrial grade"
],
uses:[
"Irrigation",
"Water lines",
"Gas systems"
]
},

"sheet":{
title:"Steel Sheets",
sizes:"0.3mm to 6mm",
features:[
"Smooth surface",
"Easy cutting",
"Industrial grade"
],
uses:[
"Containers",
"Roofing",
"Furniture"
]
},

"gi sheet":{
title:"GI Sheets",
sizes:"0.3mm to 3mm",
features:[
"Rust resistant",
"Weather protection",
"Strong zinc coating"
],
uses:[
"Roofing",
"Outdoor structures",
"Air ducts"
]
},

"ppgi sheet":{
title:"PPGI Sheets",
sizes:"0.3mm to 1mm",
features:[
"Color coated",
"Heat resistant",
"Modern appearance"
],
uses:[
"Warehouse roofing",
"Buildings",
"Architectural facades"
]
},

"plate":{
title:"Steel Plates",
sizes:"6mm to 300mm+",
features:[
"Heavy duty strength",
"Impact resistant",
"Industrial grade"
],
uses:[
"Ship hulls",
"Bridges",
"Machinery beds"
]
},

"checkered plate":{
title:"Checkered Plates",
sizes:"3mm to 12mm",
features:[
"Slip resistant",
"Weather resistant",
"Heavy duty"
],
uses:[
"Industrial stairs",
"Catwalks",
"Ramps"
]
},

"wire rod":{
title:"Wire Rods",
sizes:"5mm to 16mm",
features:[
"Flexible steel",
"Smooth finish",
"Industrial grade"
],
uses:[
"Nails",
"Springs",
"Fencing mesh"
]
},

"square bar":{
title:"Square Bars",
sizes:"8mm × 8mm to 100mm × 100mm",
features:[
"Solid steel body",
"Strong structure",
"Long lasting"
],
uses:[
"Industrial grills",
"Machinery components",
"Forged tools"
]
},

"flat bar":{
title:"Flat Bars",
sizes:"12mm to 300mm",
features:[
"Easy welding",
"Strong support",
"Durable steel"
],
uses:[
"Brackets",
"Structural joints",
"Base plates"
]
},

"hex bar":{
title:"Hexagonal Bars",
sizes:"6mm to 75mm",
features:[
"Precision finish",
"Machining ready",
"Strong material"
],
uses:[
"Bolts",
"Nuts",
"Hydraulic fittings"
]
},

"shs":{
title:"Square Hollow Sections",
sizes:"20mm × 20mm to 400mm × 400mm",
features:[
"Modern appearance",
"Strong structure",
"Architectural grade"
],
uses:[
"Columns",
"Frames",
"Solar structures"
]
},

"rhs":{
title:"Rectangular Hollow Sections",
sizes:"40mm × 20mm to 500mm × 300mm",
features:[
"High strength",
"Industrial grade",
"Reliable durability"
],
uses:[
"Trailers",
"Trusses",
"Mechanical structures"
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
