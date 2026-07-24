<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bryan D. Mozar | AI Automation Engineer</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <nav>
        <h1 class="logo">Bryan D. Mozar</h1>
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
        <h2>AI Automation Engineer</h2>
        <h3><span id="typing"></span></h3>
        <p>Building intelligent workflows using n8n, Make.com, AI Agents, and cloud automation solutions.</p>
        <a href="#projects" class="btn">View Projects</a>
    </div>
</section>

<section id="about" class="section">
    <h2>About Me</h2>
    <p>
        I am <strong>Bryan D. Mozar</strong>, an AI Automation Engineer specializing in workflow automation, AI-powered business systems, CRM integration, and cloud-based process optimization.
        I create scalable automation solutions that reduce manual work and improve business efficiency.
    </p>
</section>

<section id="services" class="section">
    <h2>Services</h2>
    <div class="cards">
        <div class="card">
            <h3>n8n Automation</h3>
            <p>Custom workflow automation for sales, support, inventory, and operations.</p>
        </div>
        <div class="card">
            <h3>AI Agents</h3>
            <p>Intelligent AI assistants connected to Telegram, Messenger, Email, and CRMs.</p>
        </div>
        <div class="card">
            <h3>Make.com Solutions</h3>
            <p>End-to-end business process automation with cloud integrations.</p>
        </div>
        <div class="card">
            <h3>AI Content Automation</h3>
            <p>Automated video, social media, and marketing content generation.</p>
        </div>
    </div>
</section>

<section id="projects" class="section">
    <h2>Featured Projects</h2>
    <div class="project">
        <h3>AI Dental Clinic Assistant</h3>
        <p>Facebook Messenger AI bot with appointment scheduling and email notifications.</p>
    </div>
    <div class="project">
        <h3>Inventory AI Manager</h3>
        <p>Automated stock tracking and reorder alerts using Airtable and n8n.</p>
    </div>
    <div class="project">
        <h3>AI Invoice Processing System</h3>
        <p>Extracts invoice data from PDFs and updates business records automatically.</p>
    </div>
</section>

<section id="contact" class="section">
    <h2>Contact</h2>
    <p>📧 mozar@gmail.com</p>
    <p>💼 GitHub: github.com/yanyanmozar-sys</p>
</section>

<footer>
    <p>© 2026 Bryan D. Mozar | AI Automation Engineer</p>
</footer>

<script src="script.js"></script>
</body>
</html>* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: #0a0f1f;
    color: white;
    line-height: 1.6;
}

header {
    position: fixed;
    width: 100%;
    top: 0;
    background: rgba(0,0,0,0.7);
    backdrop-filter: blur(10px);
    z-index: 1000;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 5%;
}

nav ul {
    display: flex;
    list-style: none;
}

nav ul li {
    margin-left: 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

.logo {
    color: #00e5ff;
}

.hero {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    background: radial-gradient(circle, #102040, #05070f);
}

.hero h2 {
    font-size: 3.5rem;
    color: #00e5ff;
}

.hero h3 {
    font-size: 1.8rem;
    margin: 1rem 0;
    color: #ff00ff;
}

.btn {
    display: inline-block;
    margin-top: 1rem;
    padding: 12px 30px;
    background: #00e5ff;
    color: black;
    text-decoration: none;
    border-radius: 30px;
    font-weight: bold;
}

.section {
    padding: 100px 10%;
}

.section h2 {
    text-align: center;
    margin-bottom: 40px;
    color: #00e5ff;
    font-size: 2.5rem;
}

.cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

.card, .project {
    background: rgba(255,255,255,0.05);
    padding: 25px;
    border-radius: 15px;
    border: 1px solid rgba(255,255,255,0.1);
    backdrop-filter: blur(10px);
}

.card:hover, .project:hover {
    transform: translateY(-5px);
    transition: 0.3s ease;
    border-color: #00e5ff;
}

footer {
    text-align: center;
    padding: 20px;
    background: #05070f;
    border-top: 1px solid rgba(255,255,255,0.1);
}

@media (max-width: 768px) {
    .hero h2 {
        font-size: 2.5rem;
    }

    .hero h3 {
        font-size: 1.3rem;
    }
}
