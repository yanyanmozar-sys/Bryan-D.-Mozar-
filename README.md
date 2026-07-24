<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bryan D. Mozar | AI Automation Specialist</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

body{
    background:#050816;
    color:#fff;
    overflow-x:hidden;
}

header{
    position:fixed;
    width:100%;
    top:0;
    z-index:100;
    background:rgba(0,0,0,0.7);
    backdrop-filter:blur(10px);
}

nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 10%;
}

.logo{
    font-size:24px;
    font-weight:700;
    color:#00f7ff;
}

nav ul{
    display:flex;
    list-style:none;
    gap:25px;
}

nav ul li a{
    text-decoration:none;
    color:white;
    transition:0.3s;
}

nav ul li a:hover{
    color:#00f7ff;
}

.hero{
    min-height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:100px 20px;
    background:linear-gradient(135deg,#050816,#0f172a);
}

.hero-content h1{
    font-size:60px;
    margin-bottom:10px;
}

.hero-content span{
    color:#00f7ff;
}

.typing{
    font-size:24px;
    color:#00f7ff;
    margin-bottom:20px;
}

.hero p{
    max-width:700px;
    margin:auto;
    color:#cbd5e1;
}

.btn{
    display:inline-block;
    margin-top:30px;
    padding:14px 35px;
    background:#00f7ff;
    color:#000;
    text-decoration:none;
    border-radius:30px;
    font-weight:600;
}

section{
    padding:100px 10%;
}

.section-title{
    text-align:center;
    margin-bottom:50px;
    font-size:40px;
    color:#00f7ff;
}

.about{
    text-align:center;
}

.services{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}

.card{
    background:rgba(255,255,255,0.05);
    padding:30px;
    border-radius:15px;
    backdrop-filter:blur(10px);
    transition:0.3s;
}

.card:hover{
    transform:translateY(-10px);
}

.card h3{
    margin-bottom:15px;
    color:#00f7ff;
}

.projects{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:25px;
}

.project{
    background:#111827;
    border-radius:15px;
    overflow:hidden;
}

.project img{
    width:100%;
    height:200px;
    object-fit:cover;
}

.project-content{
    padding:20px;
}

footer{
    text-align:center;
    padding:30px;
    background:#020617;
}

.contact{
    text-align:center;
}

.contact a{
    color:#00f7ff;
    text-decoration:none;
}

.glow{
    animation:glow 2s infinite alternate;
}

@keyframes glow{
    from{
        text-shadow:0 0 10px #00f7ff;
    }
    to{
        text-shadow:0 0 25px #00f7ff;
    }
}

@media(max-width:768px){
    .hero-content h1{
        font-size:40px;
    }

    .typing{
        font-size:20px;
    }

    nav{
        flex-direction:column;
        gap:15px;
    }
}
</style>
</head>
<body>

<header>
<nav>
<div class="logo">Bryan Mozar</div>

<ul>
<li><a href="#about">About</a></li>
<li><a href="#services">Services</a></li>
<li><a href="#projects">Projects</a></li>
<li><a href="#contact">Contact</a></li>
</ul>
</nav>
</header>

<section class="hero">
<div class="hero-content">
<h1 class="glow">Bryan D. <span>Mozar</span></h1>

<div class="typing">
<span id="typed"></span>
</div>

<p>
Helping businesses automate workflows using AI, n8n, Make.com, OpenAI,
Telegram Bots, CRM integrations, Google Workspace automation,
and intelligent AI Agents.
</p>

<a href="#contact" class="btn">Let's Automate</a>
</div>
</section>

<section id="about" class="about">
<h2 class="section-title">About Me</h2>

<p>
I'm Bryan D. Mozar, an AI Automation Specialist focused on building
intelligent workflows that save time, reduce manual tasks,
and increase business productivity.

I create custom automation systems using n8n, Make.com,
OpenAI, Airtable, Google Workspace, Telegram, Facebook Messenger,
and CRM integrations.
</p>
</section>

<section id="services">
<h2 class="section-title">Services</h2>

<div class="services">

<div class="card">
<h3>AI Agents</h3>
<p>
Custom AI assistants for customer support, lead generation,
and business operations.
</p>
</div>

<div class="card">
<h3>n8n Automation</h3>
<p>
Workflow automation connecting APIs, databases,
emails, CRMs, and AI tools.
</p>
</div>

<div class="card">
<h3>Make.com Systems</h3>
<p>
Advanced automation scenarios for business processes
and productivity.
</p>
</div>

<div class="card">
<h3>Chatbots</h3>
<p>
Telegram, Facebook Messenger,
and AI-powered customer service bots.
</p>
</div>

</div>
</section>

<section id="projects">
<h2 class="section-title">Featured Projects</h2>

<div class="projects">

<div class="project">
<img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3" alt="">
<div class="project-content">
<h3>AI Lead Generation System</h3>
<p>
Automated lead research, qualification,
and personalized outreach.
</p>
</div>
</div>

<div class="project">
<img src="https://images.unsplash.com/photo-1551434678-e076c223a692" alt="">
<div class="project-content">
<h3>Customer Support AI Agent</h3>
<p>
AI chatbot integrated with Telegram
and CRM systems.
</p>
</div>
</div>

<div class="project">
<img src="https://images.unsplash.com/photo-1451187580459-43490279c0fa" alt="">
<div class="project-content">
<h3>Business Workflow Automation</h3>
<p>
Automated approvals, notifications,
and reporting systems.
</p>
</div>
</div>

</div>
</section>

<section id="contact" class="contact">
<h2 class="section-title">Contact</h2>

<p>Email: bryanmozar@gmail.com</p>
<p>GitHub: github.com/YanyanMozar-SYS</p>

<br>

<a href="https://github.com/YanyanMozar-SYS">
Visit My GitHub
</a>
</section>

<footer>
<p>© 2026 Bryan D. Mozar | AI Automation Specialist</p>
</footer>

<script>
const words = [
"AI Automation Specialist",
"n8n Expert",
"Make.com Developer",
"AI Agent Builder",
"Workflow Automation Consultant"
];

let i = 0;
let j = 0;
let currentWord = "";
let isDeleting = false;

function type(){
    currentWord = words[i];

    if(!isDeleting){
        document.getElementById("typed").textContent =
        currentWord.substring(0,j++);
    }else{
        document.getElementById("typed").textContent =
        currentWord.substring(0,j--);
    }

    if(j === currentWord.length + 1){
        isDeleting = true;
        setTimeout(type,1000);
        return;
    }

    if(j === 0){
        isDeleting = false;
        i = (i + 1) % words.length;
    }

    setTimeout(type,isDeleting ? 50 : 100);
}

type();
</script>

</body>
</html>
