
<html lang="en">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>SLC | Shree Lakshmi & Co</title>

<meta name="description" content="Premium Iron & Steel Solutions">

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

/* VIDEO BACKGROUND */

#bgvideo{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
object-fit:cover;
z-index:-2;
filter:brightness(0.25);
}

/* OVERLAY */

.overlay{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:
linear-gradient(
rgba(0,0,0,0.82),
rgba(50,0,0,0.88)
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
background:rgba(0,0,0,0.45);
backdrop-filter:blur(12px);
z-index:1000;
border-bottom:1px solid rgba(255,204,0,0.2);
}

.logo{
font-size:44px;
font-weight:800;
color:#ffcc00;
letter-spacing:2px;
text-shadow:
0 0 10px #ffcc00,
0 0 25px red;
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
padding:140px 20px 60px;
}

.hero h1{
font-size:92px;
font-weight:800;
color:#ffcc00;
line-height:1.1;
text-shadow:
0 0 20px #ffcc00,
0 0 40px red;
animation:float 3s ease-in-out infinite;
}

@keyframes float{
50%{
transform:translateY(-10px);
}
}

.hero p{
margin-top:25px;
font-size:24px;
max-width:850px;
line-height:1.8;
color:#ddd;
}

/* SEARCH */

.search-container{
margin-top:45px;
width:100%;
display:flex;
justify-content:center;
}

.search-box{
width:100%;
max-width:950px;
display:flex;
background:rgba(255,255,255,0.08);
backdrop-filter:blur(14px);
border-radius:60px;
padding:10px;
box-shadow:0 0 25px rgba(255,0,0,0.25);
}

.search-box input{
flex:1;
padding:20px 24px;
border:none;
outline:none;
background:transparent;
color:white;
font-size:18px;
}

.search-box input::placeholder{
color:#ccc;
}

.search-box button{
padding:18px 34px;
border:none;
border-radius:50px;
background:linear-gradient(to right,#ff0000,#ffcc00);
color:black;
font-weight:700;
font-size:16px;
cursor:pointer;
transition:0.3s;
}

.search-box button:hover{
transform:scale(1.05);
}

/* RESULT */

#aiResult{
display:none;
margin-top:35px;
width:100%;
max-width:1050px;
padding:35px;
border-radius:30px;
background:rgba(255,255,255,0.08);
backdrop-filter:blur(16px);
border:1px solid rgba(255,204,0,0.25);
box-shadow:0 0 30px rgba(255,0,0,0.35);
text-align:left;
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

/* SECTIONS */

.section{
padding:110px 8%;
}

.section-title{
font-size:58px;
text-align:center;
color:#ffcc00;
margin-bottom:60px;
text-shadow:0 0 20px red;
}

/* CARDS */

.cards{
display:flex;
justify-content:center;
flex-wrap:wrap;
gap:30px;
}

.card{
width:320px;
padding:35px;
border-radius:30px;
background:rgba(255,255,255,0.08);
backdrop-filter:blur(12px);
border:1px solid rgba(255,204,0,0.15);
transition:0.4s;
}

.card:hover{
transform:translateY(-10px);
box-shadow:
0 0 20px #ffcc00,
0 0 40px red;
}

.card h3{
font-size:28px;
margin-bottom:18px;
color:#ffcc00;
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
font-size:58px;
color:#ffcc00;
margin-bottom:20px;
}

.contact p{
font-size:21px;
margin-bottom:35px;
color:#ddd;
}

.buttons{
display:flex;
justify-content:center;
gap:22px;
flex-wrap:wrap;
}

.buttons a{
padding:18px 34px;
border-radius:60px;
text-decoration:none;
font-size:18px;
font-weight:700;
transition:0.3s;
}

.call{
background:red;
color:white;
box-shadow:0 0 20px red;
}

.whatsapp{
background:#25D366;
color:white;
box-shadow:0 0 20px #25D366;
}

.buttons a:hover{
transform:scale(1.08);
}

.address{
margin-top:40px;
font-size:19px;
line-height:2;
color:#ddd;
}

/* FOOTER */

footer{
padding:28px;
text-align:center;
background:black;
color:#aaa;
font-size:15px;
}

/* MOBILE */

@media(max-width:768px){

.hero h1{
font-size:52px;
}

.hero p{
font-size:18px;
}

nav{
display:none;
}

.search-box{
flex-direction:column;
border-radius:30px;
}

.search-box button{
width:100%;
}

}

</style>

</head>

<body>

<!-- VIDEO -->

<video autoplay muted loop playsinline id="bgvideo">
<source src="https://www.w3schools.com/howto/rain.mp4" type="video/mp4">
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
Premium Iron & Steel Solutions Powered by SLC AI Search Technology
</p>

<div class="search-container">

<div class="search-box">

<input
type="text"
id="searchInput"
placeholder="Search channel, beam, tmt bar, pipe, gi sheet...">

<button onclick="searchAI()">
Search
</button>

</div>

</div>

<div id="aiResult"></div>

</section>

<!-- ABOUT -->

<section class="section" id="about">

<h2 class="section-title">
Why Choose SLC?
</h2>

<div class="cards">

<div class="card">
<h3>Premium Steel</h3>
<p>
High quality iron and steel products for construction and industrial projects.
</p>
</div>

<div class="card">
<h3>SLC AI Search</h3>
<p>
Search materials instantly and view sizes, features and industrial applications.
</p>
</div>

<div class="card">
<h3>Trusted Supply</h3>
<p>
Reliable supply chain with fast delivery for commercial and industrial requirements.
</p>
</div>

</div>

</section>

<!-- CONTACT -->

<section class="contact" id="contact">

<h2>Contact SLC</h2>

<p>
Call or WhatsApp instantly for orders and enquiries.
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

<b>Address:</b><br>

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

const database = {

"channel":{
title:"Steel Channels",
info:"Steel channels are structural profiles used in industrial frameworks and heavy buildings.",
sizes:"75mm × 40mm up to 400mm × 110mm",
features:[
"Strong structural support",
"Superior load distribution",
"Industrial strength",
"Rust resistant",
"Heavy construction ready"
],
uses:[
"Industrial frameworks",
"Vehicle chassis",
"Building columns",
"Warehouse structures"
]
},

"beam":{
title:"Universal Beams",
info:"Universal beams resist heavy bending forces in industrial buildings and bridges.",
sizes:"127mm × 76mm up to 1016mm × 305mm",
features:[
"High bending resistance",
"Heavy load capacity",
"Reliable support",
"Construction grade steel"
],
uses:[
"Bridge construction",
"Industrial buildings",
"Steel floors"
]
},

"column":{
title:"Universal Columns",
info:"Universal columns are thick steel sections designed for massive vertical loads.",
sizes:"152mm × 152mm up to 356mm × 406mm",
features:[
"Extreme vertical support",
"Heavy duty structure",
"Earthquake resistant",
"Industrial strength"
],
uses:[
"Building columns",
"Industrial sheds",
"Warehouse supports"
]
},

"angle":{
title:"Steel Angles",
info:"Steel angles are L-shaped structural sections used in framing systems.",
sizes:"20mm × 20mm × 3mm up to 250mm × 250mm × 35mm",
features:[
"Strong corner support",
"Easy fabrication",
"High durability",
"Industrial quality"
],
uses:[
"Roof trusses",
"Cell towers",
"Structural framing"
]
},

"5mm rod":{
title:"5MM Wire Rod",
info:"5MM smooth steel rods are used for manufacturing steel products.",
sizes:"5mm",
features:[
"Flexible material",
"Smooth finish",
"Easy bending",
"High durability"
],
uses:[
"Nails",
"Screws",
"Wire mesh",
"Fencing"
]
},

"6mm rod":{
title:"6MM TMT Rebar",
info:"6MM rebars are reinforcement bars engineered for concrete bonding.",
sizes:"6mm",
features:[
"Concrete bonding ribs",
"High tensile strength",
"Corrosion resistant",
"Construction ready"
],
uses:[
"Buildings",
"Concrete reinforcement",
"Structural support"
]
},

"tmt bar":{
title:"TMT Rebar",
info:"TMT rebars are deformed reinforcement bars engineered for concrete bonding.",
sizes:"6mm to 50mm",
features:[
"Earthquake resistant",
"Fire resistant",
"High tensile strength",
"Corrosion resistant"
],
uses:[
"Buildings",
"Flyovers",
"Bridges",
"Towers"
]
},

"sheet":{
title:"Steel Sheets",
info:"Steel sheets are flat rolled products used in manufacturing.",
sizes:"0.3mm to 6mm",
features:[
"Smooth surface",
"Easy cutting",
"Industrial grade",
"Durable quality"
],
uses:[
"Car bodies",
"Furniture",
"Containers",
"Roofing"
]
},

"gi sheet":{
title:"GI Sheets",
info:"Galvanized iron sheets are zinc coated for rust resistance.",
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

"pipe":{
title:"Steel Pipes",
info:"Steel pipes are tubular products used for transport and structures.",
sizes:"1/8 inch to 26 inch",
features:[
"Leak resistant",
"Heavy duty",
"Smooth finish",
"Long lasting"
],
uses:[
"Water supply",
"Gas pipelines",
"Industrial transport"
]
},

"shs":{
title:"Square Hollow Sections",
info:"SHS are square hollow steel sections used in structures.",
sizes:"20mm × 20mm to 400mm × 400mm",
features:[
"Modern appearance",
"Strong structure",
"Architectural grade"
],
uses:[
"Columns",
"Architectural frames",
"Solar structures"
]
},

"rhs":{
title:"Rectangular Hollow Sections",
info:"RHS are rectangular hollow steel sections used in trusses and trailers.",
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

};

function searchAI(){

let input =
document.getElementById("searchInput").value.toLowerCase().trim();

let result =
document.getElementById("aiResult");

if(database[input]){

let data = database[input];

let featuresHTML = "";
let usesHTML = "";

for(let i=0;i<data.features.length;i++){

featuresHTML += "<li>" + data.features[i] + "</li>";

}

for(let i=0;i<data.uses.length;i++){

usesHTML += "<li>" + data.uses[i] + "</li>";

}

result.innerHTML =

"<h2 style='color:#ffcc00;font-size:46px;margin-bottom:15px;'>" +
data.title +
"</h2>" +

"<p style='font-size:19px;line-height:1.9;margin-bottom:20px;color:#ddd;'>" +
data.info +
"</p>" +

"<h3 style='color:red;font-size:28px;margin-bottom:10px;'>Available Sizes</h3>" +

"<p style='font-size:18px;margin-bottom:25px;color:#fff;'>" +
data.sizes +
"</p>" +

"<h3 style='color:#ffcc00;font-size:28px;margin-bottom:10px;'>Features</h3>" +

"<ul style='padding-left:25px;line-height:2;font-size:18px;margin-bottom:25px;'>" +
featuresHTML +
"</ul>" +

"<h3 style='color:red;font-size:28px;margin-bottom:10px;'>Applications / Uses</h3>" +

"<ul style='padding-left:25px;line-height:2;font-size:18px;'>" +
usesHTML +
"</ul>";

}else{

result.innerHTML =

"<h2 style='color:#ffcc00;font-size:42px;'>SLC AI Assistant</h2>" +

"<p style='margin-top:20px;font-size:18px;line-height:2;color:#ddd;'>" +

"Material not found.<br><br>" +

"Try searching:<br><br>" +

"• channel<br>" +
"• beam<br>" +
"• column<br>" +
"• angle<br>" +
"• 5mm rod<br>" +
"• 6mm rod<br>" +
"• tmt bar<br>" +
"• sheet<br>" +
"• gi sheet<br>" +
"• pipe<br>" +
"• shs<br>" +
"• rhs" +

"</p>";

}

result.style.display = "block";

}

</script>

</body>
</html>
