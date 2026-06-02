
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>SLC | Shree Lakshmi & Co</title>

<meta name="description"
content="SLC - Shree Lakshmi & Co Modern Iron & Steel Business Website">

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

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
right:0;
bottom:0;
min-width:100%;
min-height:100%;
object-fit:cover;
z-index:-2;
filter:brightness(0.25);
}

.overlay{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:linear-gradient(to bottom,
rgba(0,0,0,0.5),
rgba(60,0,0,0.7));
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
background:rgba(0,0,0,0.5);
backdrop-filter:blur(12px);
z-index:1000;
}

.logo{
font-size:42px;
font-weight:700;
color:#ffcc00;
text-shadow:
0 0 10px #ffcc00,
0 0 20px red,
0 0 40px red;
}

nav a{
text-decoration:none;
color:white;
margin-left:25px;
font-weight:600;
transition:0.3s;
}

nav a:hover{
color:#ffcc00;
}

/* HERO */

.hero{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
}

.hero h1{
font-size:90px;
color:#ffcc00;
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
font-size:24px;
margin-top:20px;
max-width:800px;
line-height:1.7;
}

/* SEARCH */

.search-box{
margin-top:35px;
display:flex;
gap:10px;
flex-wrap:wrap;
justify-content:center;
}

.search-box input{
padding:18px 22px;
width:340px;
border:none;
border-radius:50px;
outline:none;
font-size:17px;
}

.search-box button{
padding:18px 28px;
border:none;
border-radius:50px;
background:red;
color:white;
font-size:16px;
font-weight:bold;
cursor:pointer;
transition:0.3s;
}

.search-box button:hover{
background:#ffcc00;
color:black;
transform:scale(1.05);
}

/* AI RESULT */

#aiResult{
margin-top:30px;
max-width:760px;
padding:30px;
border-radius:25px;
background:rgba(255,255,255,0.08);
backdrop-filter:blur(12px);
box-shadow:0 0 25px rgba(255,0,0,0.3);
display:none;
text-align:left;
animation:fade 0.5s ease;
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

/* SECTION */

.section{
padding:100px 8%;
}

.section-title{
text-align:center;
font-size:55px;
margin-bottom:50px;
color:#ffcc00;
text-shadow:0 0 20px red;
}

/* CARDS */

.cards{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:30px;
}

.card{
width:300px;
padding:35px;
border-radius:25px;
background:rgba(255,255,255,0.08);
backdrop-filter:blur(12px);
border:2px solid rgba(255,204,0,0.2);
transition:0.4s;
}

.card:hover{
transform:translateY(-10px);
box-shadow:
0 0 20px #ffcc00,
0 0 40px red;
}

.card h3{
color:#ffcc00;
margin-bottom:15px;
font-size:28px;
}

.card p{
line-height:1.7;
}

/* CONTACT */

.contact{
padding:100px 20px;
text-align:center;
}

.contact h2{
font-size:55px;
color:#ffcc00;
margin-bottom:20px;
}

.contact p{
font-size:20px;
margin-bottom:35px;
}

.buttons{
display:flex;
justify-content:center;
gap:20px;
flex-wrap:wrap;
}

.buttons a{
padding:18px 32px;
border-radius:50px;
text-decoration:none;
font-weight:bold;
font-size:18px;
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

/* FOOTER */

footer{
padding:30px;
text-align:center;
background:black;
color:#aaa;
}

/* MOBILE */

@media(max-width:768px){

.hero h1{
font-size:55px;
}

.hero p{
font-size:18px;
}

nav{
display:none;
}

.search-box input{
width:100%;
}

}

</style>
</head>

<body>

<!-- VIDEO -->

<video autoplay muted loop id="bgvideo">
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
Modern Iron & Steel Experience Powered by SLC AI
</p>

<div class="search-box">

<input
type="text"
id="searchInput"
placeholder="Search any material...">

<button onclick="searchAI()">
Search
</button>

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
High quality iron and steel products for modern construction and industrial use.
</p>
</div>

<div class="card">
<h3>Fast Delivery</h3>
<p>
Quick transportation and trusted supply chain service.
</p>
</div>

<div class="card">
<h3>Modern Technology</h3>
<p>
AI powered product support and smart customer experience.
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

</section>

<footer>
© 2026 SLC | Shree Lakshmi & Co
</footer>

<script>

const database = {

"channel":{
title:"Steel Channel",
info:"Steel channels are used for construction frames, support structures and factories.",
features:[
"Strong load support",
"Rust resistant",
"Long lasting",
"Industrial strength",
"Used in buildings"
]
},

"5mm rod":{
title:"5MM Steel Rod",
info:"5MM rods are used for reinforcement and small construction work.",
features:[
"Flexible usage",
"Easy bending",
"High durability",
"Strong grip",
"Construction ready"
]
},

"6mm rod":{
title:"6MM Steel Rod",
info:"6MM rods are used in structural support and house construction.",
features:[
"Weather resistant",
"High strength",
"Long lifespan",
"Reliable quality",
"Easy installation"
]
},

"8mm rod":{
title:"8MM Steel Rod",
info:"8MM rods are used in slabs and reinforced concrete structures.",
features:[
"Strong reinforcement",
"Durable material",
"Construction grade",
"High load capacity",
"Corrosion resistant"
]
},

"10mm rod":{
title:"10MM Steel Rod",
info:"10MM rods are used in beams and heavy structures.",
features:[
"Heavy duty support",
"Excellent strength",
"Long lasting",
"Reliable structure",
"Industrial quality"
]
},

"12mm rod":{
title:"12MM Steel Rod",
info:"12MM rods are used in large construction projects.",
features:[
"Very high strength",
"Supports heavy loads",
"Corrosion resistant",
"Premium quality",
"Strong bonding"
]
},

"16mm rod":{
title:"16MM Steel Rod",
info:"16MM rods are used in bridges and industrial foundations.",
features:[
"Maximum support",
"Industrial grade",
"Earthquake resistant",
"Very durable",
"Heavy construction ready"
]
},

"tmt bar":{
title:"TMT Bar",
info:"TMT bars are used in reinforced concrete structures like buildings and bridges.",
features:[
"Earthquake resistant",
"Fire resistant",
"High tensile strength",
"Corrosion resistant",
"Excellent bonding"
]
},

"pipe":{
title:"Steel Pipe",
info:"Steel pipes are used in plumbing and industries.",
features:[
"Leak resistant",
"Heavy duty",
"Smooth finish",
"Long lasting",
"Strong body"
]
},

"sheet":{
title:"Steel Sheet",
info:"Steel sheets are used in roofing and fabrication industries.",
features:[
"Smooth surface",
"Easy cutting",
"Weather protection",
"Durable finish",
"Industrial grade"
]
},

"angle":{
title:"Steel Angle",
info:"Steel angles are used for frames and industrial supports.",
features:[
"Strong corner support",
"Easy fabrication",
"High durability",
"Industrial use",
"Long lasting"
]
},

"beam":{
title:"Steel Beam",
info:"Steel beams are used in buildings and bridge construction.",
features:[
"Supports heavy loads",
"Strong structure",
"Long lifespan",
"Industrial strength",
"Reliable support"
]
},

"plate":{
title:"Steel Plate",
info:"Steel plates are used in machinery and fabrication.",
features:[
"Heavy duty material",
"High strength",
"Durable finish",
"Easy welding",
"Industrial grade"
]
},

"coil":{
title:"Steel Coil",
info:"Steel coils are used in roofing and manufacturing industries.",
features:[
"Flexible usage",
"Smooth surface",
"Easy transport",
"Durable quality",
"Factory ready"
]
},

"wire":{
title:"Steel Wire",
info:"Steel wires are used in fencing and industrial applications.",
features:[
"Flexible material",
"Strong tension",
"Rust resistant",
"Easy handling",
"Long lasting"
]
},

"cement":{
title:"Cement",
info:"Cement is used in concrete and building construction.",
features:[
"High bonding strength",
"Smooth finish",
"Reliable construction",
"Weather resistant",
"Strong foundation"
]
},

"brick":{
title:"Construction Brick",
info:"Bricks are used for walls and building structures.",
features:[
"Strong material",
"Heat resistant",
"Durable structure",
"Long lifespan",
"Construction ready"
]
},

"sand":{
title:"Construction Sand",
info:"Sand is used in plastering and construction mixing.",
features:[
"Smooth mixing",
"Construction grade",
"Reliable quality",
"Easy usage",
"Strong support"
]
},

"gravel":{
title:"Gravel Stone",
info:"Gravel stones are used in roads and concrete mixing.",
features:[
"Strong support",
"Water drainage",
"Road construction",
"Long lasting",
"Heavy duty"
]
}

};

function searchAI(){

let input =
document
.getElementById("searchInput")
.value
.toLowerCase()
.trim();

let result =
document.getElementById("aiResult");

if(database[input]){

let data = database[input];

let featuresHTML = "";

data.features.forEach(function(feature){

featuresHTML +=
"<li>" + feature + "</li>";

});

result.innerHTML = `

<h2 style="
color:#ffcc00;
font-size:40px;
margin-bottom:15px;
">
${data.title}
</h2>

<p style="
font-size:18px;
line-height:1.8;
margin-bottom:25px;
">
${data.info}
</p>

<h3 style="
color:red;
margin-bottom:12px;
font-size:26px;
">
Features
</h3>

<ul style="
padding-left:25px;
line-height:2;
font-size:17px;
">
${featuresHTML}
</ul>

`;

}else{

result.innerHTML = `

<h2 style="color:#ffcc00;">
SLC AI Assistant
</h2>

<p style="
font-size:18px;
line-height:1.8;
margin-top:15px;
">

Material not found.

Try searching:

<br><br>

• channel<br>
• 5mm rod<br>
• 6mm rod<br>
• 8mm rod<br>
• 10mm rod<br>
• 12mm rod<br>
• 16mm rod<br>
• tmt bar<br>
• pipe<br>
• sheet<br>
• angle<br>
• beam<br>
• plate<br>
• coil<br>
• wire<br>
• cement<br>
• brick<br>
• sand<br>
• gravel

</p>

`;

}

result.style.display = "block";

}

</script>

</body>
</html>
```
