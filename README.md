<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cyber AI & Automation Hub</title>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600;800;900&family=Rajdhani:wght@400;500;600;700&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --bg-color: #050814;
            --card-bg: rgba(15, 23, 42, 0.55);
            --card-border: rgba(56, 189, 248, 0.2);
            --neon-blue: #00f0ff;
            --neon-purple: #7000ff;
            --neon-pink: #ff007f;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
            --glass-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            font-family: 'Rajdhani', sans-serif;
            overflow-x: hidden;
            line-height: 1.6;
        }

        /* Canvas Background */
        #bg-canvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            z-index: -1;
            background: radial-gradient(circle at center, #0a0f24 0%, #03050b 100%);
        }

        /* Typography & Utilities */
        h1, h2, h3, .brand {
            font-family: 'Orbitron', sans-serif;
            letter-spacing: 1px;
        }

        .neon-text-blue {
            color: var(--neon-blue);
            text-shadow: 0 0 10px rgba(0, 240, 255, 0.6);
        }

        .neon-text-purple {
            color: var(--neon-purple);
            text-shadow: 0 0 10px rgba(112, 0, 255, 0.6);
        }

        .glass-card {
            background: var(--card-bg);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid var(--card-border);
            border-radius: 16px;
            box-shadow: var(--glass-shadow);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .glass-card:hover {
            border-color: var(--neon-blue);
            box-shadow: 0 0 20px rgba(0, 240, 255, 0.25);
            transform: translateY(-5px);
        }

        /* Navbar */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 1.2rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1000;
            background: rgba(5, 8, 20, 0.8);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
        }

        nav .logo {
            font-size: 1.5rem;
            font-weight: 800;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav ul li a {
            color: var(--text-muted);
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: 0.3s;
        }

        nav ul li a:hover {
            color: var(--neon-blue);
            text-shadow: 0 0 8px var(--neon-blue);
        }

        /* Buttons */
        .btn {
            padding: 0.8rem 1.8rem;
            border-radius: 8px;
            font-family: 'Orbitron', sans-serif;
            font-size: 0.9rem;
            font-weight: 600;
            cursor: pointer;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            transition: all 0.3s ease;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--neon-blue), var(--neon-purple));
            color: #fff;
            border: none;
            box-shadow: 0 0 15px rgba(0, 240, 255, 0.4);
        }

        .btn-primary:hover {
            box-shadow: 0 0 25px rgba(0, 240, 255, 0.8);
            transform: scale(1.03);
        }

        .btn-outline {
            background: transparent;
            color: var(--neon-blue);
            border: 1px solid var(--neon-blue);
        }

        .btn-outline:hover {
            background: rgba(0, 240, 255, 0.1);
            box-shadow: 0 0 15px rgba(0, 240, 255, 0.3);
        }

        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 0 5%;
            text-align: center;
            position: relative;
        }

        .hero-content {
            max-width: 850px;
            margin-top: 60px;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            text-transform: uppercase;
        }

        .typing-container {
            font-size: 1.8rem;
            color: var(--text-muted);
            margin-bottom: 2rem;
            min-height: 2.8rem;
        }

        .hero-btns {
            display: flex;
            gap: 1.5rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        /* Stats Section */
        .stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            padding: 4rem 10%;
        }

        .stat-card {
            padding: 2rem;
            text-align: center;
        }

        .stat-number {
            font-size: 3rem;
            font-weight: 900;
            font-family: 'Orbitron', sans-serif;
        }

        /* Section Layout */
        section {
            padding: 6rem 8%;
        }

        .section-title {
            text-align: center;
            font-size: 2.3rem;
            margin-bottom: 3rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background: var(--neon-blue);
            margin: 10px auto 0;
            box-shadow: 0 0 10px var(--neon-blue);
        }

        /* Grid Cards */
        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2rem;
        }

        .card-header {
            display: flex;
            align-items: center;
            gap: 12px;
            margin-bottom: 1rem;
        }

        .card-header i {
            font-size: 1.8rem;
        }

        .tag {
            display: inline-block;
            padding: 0.2rem 0.6rem;
            border-radius: 4px;
            font-size: 0.75rem;
            font-weight: 700;
            background: rgba(0, 240, 255, 0.1);
            color: var(--neon-blue);
            border: 1px solid rgba(0, 240, 255, 0.3);
            margin-top: 1rem;
        }

        /* Contact Section */
        .contact-container {
            max-width: 650px;
            margin: 0 auto;
            padding: 3rem;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
        }

        .form-group input, 
        .form-group textarea {
            width: 100%;
            padding: 1rem;
            background: rgba(5, 8, 20, 0.6);
            border: 1px solid var(--card-border);
            border-radius: 8px;
            color: #fff;
            font-family: inherit;
            outline: none;
            transition: 0.3s;
        }

        .form-group input:focus, 
        .form-group textarea:focus {
            border-color: var(--neon-blue);
            box-shadow: 0 0 10px rgba(0, 240, 255, 0.3);
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.05);
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        /* Mobile Responsive */
        @media (max-width: 768px) {
            nav ul { display: none; }
            .hero h1 { font-size: 2.2rem; }
            .typing-container { font-size: 1.2rem; }
            section { padding: 4rem 5%; }
        }
    </style>
</head>
<body>

    <!-- Canvas Animated Background -->
    <canvas id="bg-canvas"></canvas>

    <!-- Navigation -->
    <nav>
        <div class="logo neon-text-blue">
            <i class="fa-solid fa-brain"></i> CYBER.AI
        </div>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#n8n">n8n Workflows</a></li>
            <li><a href="#make">Make.com</a></li>
            <li><a href="#ai-agents">AI Agents</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
        <a href="#contact" class="btn btn-outline"><i class="fa-solid fa-terminal"></i> Connect</a>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="about">
        <div class="hero-content">
            <h1 class="neon-text-blue">Architecting Autonomous AI</h1>
            <div class="typing-container">
                <span id="typing-text"></span><span style="color:var(--neon-blue);">|</span>
            </div>
            <p style="color: var(--text-muted); margin-bottom: 2.5rem;">
                Engineering intelligent neural workflows, multi-agent AI ecosystems, and seamless automation pipelines for complex business logic.
            </p>
            <div class="hero-btns">
                <a href="#n8n" class="btn btn-primary"><i class="fa-solid fa-bolt"></i> Explore Showcase</a>
                <!-- Replace # with actual CV file URL path in GitHub repo -->
                <a href="#" class="btn btn-outline" id="cv-btn"><i class="fa-solid fa-file-arrow-down"></i> Download CV</a>
            </div>
        </div>
    </section>

    <!-- Animated Counters Section -->
    <div class="stats">
        <div class="glass-card stat-card">
            <div class="stat-number neon-text-blue" data-target="150">0</div>
            <p style="color:var(--text-muted);">Workflows Built</p>
        </div>
        <div class="glass-card stat-card">
            <div class="stat-number neon-text-purple" data-target="45">0</div>
            <p style="color:var(--text-muted);">AI Agents Deployed</p>
        </div>
        <div class="glass-card stat-card">
            <div class="stat-number neon-text-blue" data-target="99">0</div>
            <p style="color:var(--text-muted);">% Uptime Rate</p>
        </div>
    </div>

    <!-- n8n Workflows Section -->
    <section id="n8n">
        <h2 class="section-title neon-text-blue">n8n Workflows</h2>
        <div class="grid-container">
            <div class="glass-card" style="padding: 2rem;">
                <div class="card-header">
                    <i class="fa-solid fa-diagram-project neon-text-blue"></i>
                    <h3>Autonomous Lead Enrichment</h3>
                </div>
                <p style="color:var(--text-muted);">Webhooks trigger deep web scraping, LLM entity extraction, and automated CRM sync.</p>
                <span class="tag">n8n + OpenAI + HubSpot</span>
            </div>

            <div class="glass-card" style="padding: 2rem;">
                <div class="card-header">
                    <i class="fa-solid fa-comments neon-text-purple"></i>
                    <h3>RAG Support Assistant</h3>
                </div>
                <p style="color:var(--text-muted);">Vector database querying with Pinecone & LangChain inside n8n for zero-latency customer support.</p>
                <span class="tag">n8n + Pinecone + Claude 3</span>
            </div>

            <div class="glass-card" style="padding: 2rem;">
                <div class="card-header">
                    <i class="fa-solid fa-database neon-text-blue"></i>
                    <h3>Self-Healing Data Pipeline</h3>
                </div>
                <p style="color:var(--text-muted);">Automated error checking, fallback AI repair nodes, and Slack alert dispatches.</p>

                <span class="tag">n8n + PostgreSQL + Slack</span>
            </div>
        </div>
    </section>

    <!-- Make.com Section -->
    <section id="make">
        <h2 class="section-title neon-text-purple">Make.com Ecosystems</h2>
        <div class="grid-container">
            <div class="glass-card" style="padding: 2rem;">
                <div class="card-header">
                    <i class="fa-solid fa-share-nodes neon-text-purple"></i>
                    <h3>Omnichannel Content Engine</h3>
                </div>
                <p style="color:var(--text-muted);">Automated YouTube summary extraction generating LinkedIn posts, Tweets, and newsletters via GPT-4.</p>
                <span class="tag">Make + Airtable + OpenAI</span>
            </div>

            <div class="glass-card" style="padding: 2rem;">
                <div class="card-header">
                    <i class="fa-solid fa-file-invoice-dollar neon-text-blue"></i>
                    <h3>Financial Document Processing</h3>
                </div>
                <p style="color:var(--text-muted);">OCR vision parsing for invoices and automated accounting categorization.</p>
                <span class="tag">Make + Vision API + Quickbooks</span>
            </div>
        </div>
    </section>

    <!-- AI Agents Showcase -->
    <section id="ai-agents">
        <h2 class="section-title neon-text-blue">Autonomous AI Agents</h2>
        <div class="grid-container">
            <div class="glass-card" style="padding: 2rem;">
                <div class="card-header">
                    <i class="fa-solid fa-robot neon-text-blue"></i>
                    <h3>DevOps Monitoring Agent</h3>
                </div>
                <p style="color:var(--text-muted);">Monitors cluster logs, detects anomalies, and drafts GitHub pull requests automatically.</p>
                <span class="tag">Python + LangGraph + Docker</span>
            </div>

            <div class="glass-card" style="padding: 2rem;">
                <div class="card-header">
                    <i class="fa-solid fa-chart-line neon-text-purple"></i>
                    <h3>Market Research Analyst</h3>
                </div>
                <p style="color:var(--text-muted);">Multi-agent system aggregating competitor news, analyzing sentiment, and generating weekly PDF reports.</p>
                <span class="tag">CrewAI + GPT-4o + Tavily</span>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2 class="section-title neon-text-blue">Initialize Contact</h2>
        <div class="glass-card contact-container">
            <form onsubmit="event.preventDefault(); alert('Signal Transmitted!');">
                <div class="form-group">
                    <label>Identity / Name</label>
                    <input type="text" placeholder="John Doe" required>
                </div>
                <div class="form-group">
                    <label>Signal Address / Email</label>
                    <input type="email" placeholder="john@cyber.io" required>
                </div>
                <div class="form-group">
                    <label>Transmission / Message</label>
                    <textarea rows="5" placeholder="State your objective..." required></textarea>
                </div>
                <button type="submit" class="btn btn-primary" style="width: 100%; justify-content: center;">
                    <i class="fa-solid fa-paper-plane"></i> Send Signal
                </button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 CYBER.AI | Built for GitHub Pages</p>
    </footer>

    <!-- Interactive Scripts -->
    <script>
        /* --- Neural Network & Particle Background --- */
        const canvas = document.getElementById('bg-canvas');
        const ctx = canvas.getContext('2d');

        let width, height, particles = [];

        function resizeCanvas() {
            width = canvas.width = window.innerWidth;
            height = canvas.height = window.innerHeight;
        }

        window.addEventListener('resize', resizeCanvas);
        resizeCanvas();

        class Particle {
            constructor() {
                this.x = Math.random() * width;
                this.y = Math.random() * height;
                this.vx = (Math.random() - 0.5) * 1.2;
                this.vy = (Math.random() - 0.5) * 1.2;
                this.radius = Math.random() * 2 + 1;
            }

            update() {
                this.x += this.vx;
                this.y += this.vy;

                if (this.x < 0 || this.x > width) this.vx *= -1;
                if (this.y < 0 || this.y > height) this.vy *= -1;
            }

            draw() {
                ctx.beginPath();
                ctx.arc(this.x, this.y, this.radius, 0, Math.PI * 2);
                ctx.fillStyle = '#00f0ff';
                ctx.shadowBlur = 10;
                ctx.shadowColor = '#00f0ff';
                ctx.fill();
            }
        }

        function initParticles() {
            particles = [];
            const count = Math.floor((width * height) / 15000);
            for (let i = 0; i < count; i++) {
                particles.push(new Particle());
            }
        }

        function animate() {
            ctx.clearRect(0, 0, width, height);

            for (let i = 0; i < particles.length; i++) {
                particles[i].update();
                particles[i].draw();

                for (let j = i + 1; j < particles.length; j++) {
                    const dx = particles[i].x - particles[j].x;
                    const dy = particles[i].y - particles[j].y;
                    const dist = Math.sqrt(dx * dx + dy * dy);

                    if (dist < 130) {
                        ctx.beginPath();
                        ctx.moveTo(particles[i].x, particles[i].y);
                        ctx.lineTo(particles[j].x, particles[j].y);
                        ctx.strokeStyle = `rgba(0, 240, 255, ${1 - dist / 130})`;
                        ctx.lineWidth = 0.6;
                        ctx.stroke();
                    }
                }
            }
            requestAnimationFrame(animate);
        }

        initParticles();
        animate();

        /* --- AI Typing Effect --- */
        const phrases = [
            "Specializing in n8n & Make.com Architectures",
            "Deploying Autonomous Multi-Agent Systems",
            "Optimizing Enterprise API Integrations"
        ];
        let phraseIdx = 0;
        let charIdx = 0;
        let isDeleting = false;
        const typingSpeed = 70;
        const targetElement = document.getElementById("typing-text");

        function typeEffect() {
            const currentPhrase = phrases[phraseIdx];
            
            if (isDeleting) {
                targetElement.textContent = currentPhrase.substring(0, charIdx - 1);
                charIdx--;
            } else {
                targetElement.textContent = currentPhrase.substring(0, charIdx + 1);
                charIdx++;
            }

            if (!isDeleting && charIdx === currentPhrase.length) {
                setTimeout(() => isDeleting = true, 2000);
            } else if (isDeleting && charIdx === 0) {
                isDeleting = false;
                phraseIdx = (phraseIdx + 1) % phrases.length;
            }

            setTimeout(typeEffect, isDeleting ? typingSpeed / 2 : typingSpeed);
        }

        document.addEventListener("DOMContentLoaded", typeEffect);

        /* --- Animated Counter Numbers --- */
        const counters = document.querySelectorAll('.stat-number');
        let counterTriggered = false;

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting && !counterTriggered) {
                    counters.forEach(counter => {
                        const target = +counter.getAttribute('data-target');
                        const speed = 200;
                        const updateCount = () => {
                            const count = +counter.innerText;
                            const inc = target / speed;
                            if (count < target) {
                                counter.innerText = Math.ceil(count + inc);
                                setTimeout(updateCount, 15);
                            } else {
                                counter.innerText = target + "+";
                            }
                        };
                        updateCount();
                    });
                    counterTriggered = true;
                }
            });
        }, { threshold: 0.5 });

        observer.observe(document.querySelector('.stats'));
    </script>
</body>
</html>
