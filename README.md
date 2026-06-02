
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
}

.overlay{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:rgba(0,0,0,0.75);
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
backdrop-filter:blur(10px);
z-index:1000;
}

.logo{
font-size:42px;
font-weight:800;
color:#ffcc00;
text-shadow:0 0 20px red;
}

nav{
display:flex;
gap:25px;
}

nav a{
color:white;
text-decoration:none;
font-weight:600;
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
padding:120px 20px;
}

.hero h1{
font-size:88px;
color:#ffcc00;
text-shadow:
0 0 20px #ffcc00,
0 0 40px red;
}

.hero p{
font-size:24px;
margin-top:20px;
max-width:900px;
line-height:1.8;
}

/* SEARCH */

.searchBox{
margin-top:40px;
display:flex;
width:100%;
max-width:950px;
background:rgba(255,255,255,0.08);
border-radius:60px;
padding:10px;
backdrop-filter:blur(10px);
}

.searchBox input{
flex:1;
padding:20px;
background:transparent;
border:none;
outline:none;
color:white;
font-size:18px;
}

.searchBox button{
padding:18px 35px;
border:none;
border-radius:50px;
background:linear-gradient(to right,red,#ffcc00);
font-weight:700;
cursor:pointer;
font-size:17px;
}

.searchBox button:hover{
transform:scale(1.04);
}

/* RESULT */

#result{
display:none;
margin-top:40px;
width:100%;
max-width:1100px;
background:rgba(255,255,255,0.08);
padding:35px;
border-radius:30px;
backdrop-filter:blur(12px);
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
border-radius:25px;
background:rgba(255,255,255,0.08);
backdrop-filter:blur(12px);
}

.card h2{
color:#ffcc00;
margin-bottom:15px;
}

.card p{
line-height:1.8;
}

/* CONTACT */

.contact{
padding:100px 20px;
text-align:center;
}

.contact h2{
font-size:55px;
color:#ffcc00;
margin-bottom:25px;
}

.buttons{
display:flex;
justify-content:center;
gap:20px;
flex-wrap:wrap;
margin-top:30px;
}

.buttons a{
padding:18px 32px;
border-radius:50px;
text-decoration:none;
font-weight:700;
font-size:18px;
}

.call{
background:red;
color:white;
}

.whatsapp{
background:#25D366;
color:white;
}

.address{
margin-top:40px;
font-size:18px;
line-height:2;
}

footer{
padding:30px;
text-align:center;
color:#aaa;
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
<source src="https://cdn.coverr.co/videos/coverr-steel-factory-1560082031954?download=1080p" type="video/mp4">
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
placeholder="Search 5mm rod, beam, pipe, gi sheet, tmt bar...">

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
Instant AI product search with features, applications and specifications.
</p>
</div>

<div class="card">
<h2>Trusted Supply</h2>
<p>
Reliable supply chain with fast delivery and premium steel products.
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

const materials = {

"channel":{
title:"Steel Channels",
sizes:"75mm × 40mm to 400mm × 110mm",
features:[
"Strong structural support",
"Superior load distribution",
"Industrial strength",
"Heavy construction ready"
],
uses:[
"Industrial frameworks",
"Vehicle chassis",
"Warehouse structures"
]
},

"beam":{
title:"Universal Beams",
sizes:"127mm × 76mm to 1016mm × 305mm",
features:[
"High bending resistance",
"Heavy load support",
"Industrial grade steel"
],
uses:[
"Bridge construction",
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
"Tower structures"
]
},

"angle":{
title:"Steel Angles",
sizes:"20mm × 20mm × 3mm to 250mm × 250mm × 35mm",
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

"5mm rod":{
title:"5MM Wire Rod",
sizes:"5mm",
features:[
"Flexible material",
"Easy bending",
"Smooth finish"
],
uses:[
"Nails",
"Screws",
"Wire mesh"
]
},

"6mm rod":{
title:"6MM TMT Rebar",
sizes:"6mm",
features:[
"High tensile strength",
"Corrosion resistant",
"Concrete bonding"
],
uses:[
"Buildings",
"Structural support",
"Concrete reinforcement"
]
},

"8mm rod":{
title:"8MM TMT Rebar",
sizes:"8mm",
features:[
"Strong reinforcement",
"Long lifespan",
"Durable steel"
],
uses:[
"Concrete slabs",
"Columns",
"Frames"
]
},

"10mm rod":{
title:"10MM TMT Rebar",
sizes:"10mm",
features:[
"Heavy load support",
"Reliable structure",
"Industrial quality"
],
uses:[
"Beams",
"Columns",
"Industrial projects"
]
},

"12mm rod":{
title:"12MM TMT Rebar",
sizes:"12mm",
features:[
"Very strong support",
"Corrosion resistant",
"Heavy construction ready"
],
uses:[
"Foundations",
"Buildings",
"Large structures"
]
},

"16mm rod":{
title:"16MM TMT Rebar",
sizes:"16mm",
features:[
"Maximum strength",
"Industrial grade",
"Earthquake resistant"
],
uses:[
"Bridges",
"Industrial foundations",
"High-rise buildings"
]
},

"20mm rod":{
title:"20MM TMT Rebar",
sizes:"20mm",
features:[
"Ultra heavy support",
"Premium steel",
"High durability"
],
uses:[
"Flyovers",
"Massive buildings",
"Industrial structures"
]
},

"25mm rod":{
title:"25MM TMT Rebar",
sizes:"25mm",
features:[
"Extreme strength",
"Heavy duty",
"Reliable structure"
],
uses:[
"Bridges",
"Factories",
"Large foundations"
]
},

"32mm rod":{
title:"32MM TMT Rebar",
sizes:"32mm",
features:[
"Industrial grade",
"Very high strength",
"Premium steel"
],
uses:[
"Industrial projects",
"Large towers",
"Heavy structures"
]
},

"40mm rod":{
title:"40MM TMT Rebar",
sizes:"40mm",
features:[
"Extreme load capacity",
"Heavy construction",
"Long lifespan"
],
uses:[
"Massive foundations",
"Industrial plants",
"Mega structures"
]
},

"50mm rod":{
title:"50MM TMT Rebar",
sizes:"50mm",
features:[
"Maximum reinforcement",
"Ultra strong steel",
"Industrial strength"
],
uses:[
"Dams",
"Bridges",
"Mega projects"
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
"Flyovers",
"Bridges"
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
"Cost effective",
"Strong welded joints",
"Reliable quality"
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
"Car bodies",
"Furniture",
"Containers"
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
"Modern buildings",
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
sizes:"12mm to 300mm width",
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
"Strong material",
"Machining ready"
],
uses:[
"Bolts",
"Nuts",
"Hydraulic fittings"
]
}

};

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

"<h1 style='color:#ffcc00;margin-bottom:20px;font-size:48px;'>" +
data.title +
"</h1>" +

"<h2 style='color:red;margin-bottom:15px;'>Sizes</h2>" +

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

Object.keys(materials).join("<br>• ");

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
