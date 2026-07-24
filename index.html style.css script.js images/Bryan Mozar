/* ==========================================
   Bryan Mozar AI Portfolio
   Cyber Glassmorphism Theme
========================================== */

:root{

--bg:#050816;
--bg2:#0b1023;
--primary:#00f5ff;
--secondary:#6c63ff;
--text:#ffffff;
--text2:#cbd5e1;
--glass:rgba(255,255,255,.08);
--border:rgba(255,255,255,.15);
--shadow:0 10px 40px rgba(0,245,255,.25);

}

*{
margin:0;
padding:0;
box-sizing:border-box;
}

html{
scroll-behavior:smooth;
}

body{

font-family:Poppins,sans-serif;
background:linear-gradient(135deg,var(--bg),#081226,var(--bg2));
color:white;
overflow-x:hidden;

}

/* Scrollbar */

::-webkit-scrollbar{
width:8px;
}

::-webkit-scrollbar-thumb{
background:var(--primary);
border-radius:50px;
}

::-webkit-scrollbar-track{
background:#111827;
}

/* Animated Background */

#particles{

position:fixed;
width:100%;
height:100%;
left:0;
top:0;
z-index:-1;

background:
radial-gradient(circle at 20% 20%,rgba(0,245,255,.15),transparent 25%),
radial-gradient(circle at 80% 40%,rgba(108,99,255,.15),transparent 25%),
radial-gradient(circle at 40% 80%,rgba(0,245,255,.08),transparent 25%);

animation:bgMove 20s linear infinite;

}

@keyframes bgMove{

0%{
transform:translateY(0);
}

50%{
transform:translateY(-40px);
}

100%{
transform:translateY(0);
}

}

/* NAVIGATION */

.navbar{

position:fixed;
top:0;
left:0;
width:100%;
padding:20px 8%;
display:flex;
justify-content:center;
z-index:999;
backdrop-filter:blur(20px);
background:rgba(10,15,35,.55);
border-bottom:1px solid rgba(255,255,255,.08);

}

.container{

width:100%;
display:flex;
justify-content:space-between;
align-items:center;

}

.logo{

font-size:30px;
font-weight:700;
color:white;
text-decoration:none;

}

.logo span{

color:var(--primary);

}

.nav-links{

display:flex;
list-style:none;
gap:35px;

}

.nav-links a{

text-decoration:none;
color:white;
transition:.3s;
font-weight:500;

}

.nav-links a:hover{

color:var(--primary);

}

.menu-btn{

display:none;
font-size:30px;
cursor:pointer;

}

/* HERO */

.hero{

min-height:100vh;
display:flex;
align-items:center;
justify-content:center;
padding:120px 8%;

}

.hero-content{

max-width:900px;
width:100%;

}

/* Glass Card */

.glass-card{

background:var(--glass);

backdrop-filter:blur(20px);

border:1px solid var(--border);

padding:60px;

border-radius:25px;

box-shadow:var(--shadow);

position:relative;

overflow:hidden;

}

.glass-card::before{

content:'';

position:absolute;

width:300px;
height:300px;

background:rgba(0,245,255,.08);

border-radius:50%;

top:-120px;
right:-120px;

}

.hero h3{

font-size:22px;
color:var(--primary);

margin-bottom:10px;

}

.hero h1{

font-size:70px;

margin-bottom:15px;

line-height:1.1;

}

.hero h1 span{

color:var(--primary);

}

.hero h2{

font-size:30px;

height:40px;

margin-bottom:25px;

color:#7dd3fc;

}

.hero p{

font-size:18px;

line-height:1.8;

color:var(--text2);

margin-bottom:40px;

}

/* BUTTONS */

.hero-buttons{

display:flex;
gap:20px;
flex-wrap:wrap;

margin-bottom:40px;

}

.btn{

padding:15px 40px;

border-radius:50px;

text-decoration:none;

font-weight:600;

transition:.4s;

}

.primary{

background:var(--primary);

color:#000;

}

.primary:hover{

transform:translateY(-5px);

box-shadow:0 10px 30px rgba(0,245,255,.45);

}

.secondary{

background:transparent;

border:2px solid var(--primary);

color:white;

}

.secondary:hover{

background:var(--primary);

color:black;

}

/* SOCIAL */

.social-icons{

display:flex;

gap:18px;

}

.social-icons a{

width:50px;

height:50px;

display:flex;

align-items:center;

justify-content:center;

border-radius:50%;

background:rgba(255,255,255,.08);

color:white;

font-size:22px;

transition:.3s;

}

.social-icons a:hover{

background:var(--primary);

color:black;

transform:translateY(-8px);

}

/* Floating Cards */

.floating-card{

position:absolute;

background:rgba(255,255,255,.06);

backdrop-filter:blur(15px);

border:1px solid rgba(255,255,255,.1);

padding:20px;

border-radius:20px;

width:180px;

text-align:center;

animation:float 5s ease-in-out infinite;

box-shadow:0 10px 30px rgba(0,245,255,.15);

}

.floating-card i{

font-size:38px;

color:var(--primary);

margin-bottom:10px;

}

.card1{

top:140px;
left:40px;

}

.card2{

top:180px;
right:60px;

}

.card3{

bottom:120px;
left:80px;

}

.card4{

bottom:100px;
right:80px;

}

@keyframes float{

0%{

transform:translateY(0);

}

50%{

transform:translateY(-18px);

}

100%{

transform:translateY(0);

}

}

/* Typing Cursor */

#typing::after{

content:"|";

color:var(--primary);

animation:blink .7s infinite;

}

@keyframes blink{

50%{

opacity:0;

}

}

/* Responsive */

@media(max-width:900px){

.hero h1{

font-size:48px;

}

.hero h2{

font-size:24px;

}

.glass-card{

padding:35px;

}

.nav-links{

display:none;

}

.menu-btn{

display:block;

}

.floating-card{

display:none;

}

.hero-buttons{

flex-direction:column;

}

.btn{

width:100%;

text-align:center;

}

}

@media(max-width:600px){

.hero{

padding-top:140px;

}

.hero h1{

font-size:38px;

}

.hero p{

font-size:16px;

}

.logo{

font-size:24px;

}

}
