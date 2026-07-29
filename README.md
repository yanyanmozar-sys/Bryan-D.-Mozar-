<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bryan Mozar | AI Automation & Workflow Specialist</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --bg-primary: #0a0e17;
            --bg-card: #131b2e;
            --accent-n8n: #ff6d5a;
            --accent-make: #6f00ff;
            --accent-ai: #00f2fe;
            --text-main: #f0f4f8;
            --text-muted: #94a3b8;
            --border-color: rgba(255, 255, 255, 0.08);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
        }

        body {
            background-color: var(--bg-primary);
            color: var(--text-main);
            line-height: 1.6;
            overflow-x: hidden;
        }

        header {
            min-height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 2rem;
            background: radial-gradient(circle at 50% 30%, rgba(111, 0, 255, 0.15), transparent 70%);
        }

        .avatar-container {
            position: relative;
            margin-bottom: 1.5rem;
        }

        .avatar-svg {
            width: 130px;
            height: 130px;
            border-radius: 50%;
            background: linear-gradient(135deg, #00f2fe, #6f00ff);
            padding: 4px;
        }

        h1 {
            font-size: 3rem;
            font-weight: 800;
            margin-bottom: 0.5rem;
            background: linear-gradient(90deg, #ffffff, #00f2fe);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        p.subtitle {
            font-size: 1.25rem;
            color: var(--text-muted);
            max-width: 600px;
            margin-bottom: 2rem;
        }

        .tech-logos {
            display: flex;
            gap: 2rem;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 1rem;
        }

        .logo-card {
            background: var(--bg-card);
            border: 1px solid var(--border-color);
            padding: 1rem 1.5rem;
            border-radius: 12px;
            display: flex;
            align-items: center;
            gap: 0.75rem;
            font-weight: 600;
            transition: transform 0.3s ease, border-color 0.3s ease;
        }

        .logo-card:hover {
            transform: translateY(-5px);
            border-color: var(--accent-ai);
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 4rem 2rem;
        }

        .section-title {
            font-size: 2rem;
            margin-bottom: 2rem;
            position: relative;
            display: inline-block;
        }

        .section-title::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: -8px;
            width: 50%;
            height: 3px;
            background: linear-gradient(90deg, var(--accent-ai), transparent);
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .card {
            background: var(--bg-card);
            border: 1px solid var(--border-color);
            border-radius: 16px;
            padding: 2rem;
            transition: all 0.3s ease;
        }

        .card:hover {
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
        }

        .card-icon {
            font-size: 2rem;
            margin-bottom: 1rem;
        }

        .tag {
            display: inline-block;
            padding: 0.25rem 0.75rem;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
            margin-right: 0.5rem;
            margin-top: 1rem;
        }

        .tag-n8n { background: rgba(255, 109, 90, 0.2); color: var(--accent-n8n); }
        .tag-make { background: rgba(111, 0, 255, 0.2); color: #a855f7; }
        .tag-ai { background: rgba(0, 242, 254, 0.2); color: var(--accent-ai); }

        footer {
            text-align: center;
            padding: 2rem;
            border-top: 1px solid var(--border-color);
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-bottom: 1rem;
        }

        .social-links a {
            color: var(--text-main);
            font-size: 1.5rem;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: var(--accent-ai);
        }
    </style>
</head>
<body>

    <header>
        <div class="avatar-container">
            <!-- AI Generated Profile Graphic SVG -->
            <svg class="avatar-svg" viewBox="0 0 100 100">
                <circle cx="50" cy="50" r="45" fill="#0d1117"/>
                <path d="M30 65 C 30 50, 70 50, 70 65" stroke="#00f2fe" stroke-width="4" fill="none" stroke-linecap="round"/>
                <circle cx="50" cy="38" r="14" fill="#00f2fe"/>
                <circle cx="35" cy="50" r="4" fill="#ff6d5a"/>
                <circle cx="65" cy="50" r="4" fill="#6f00ff"/>
                <line x1="35" y1="50" x2="50" y2="38" stroke="#ff6d5a" stroke-width="2"/>
                <line x1="65" y1="50" x2="50" y2="38" stroke="#6f00ff" stroke-width="2"/>
            </svg>
        </div>
        <h1>Bryan Mozar</h1>
        <p class="subtitle">AI Automation Engineer & Workflow Architect specializing in custom autonomous agents and no-code/low-code integrations.</p>

        <div class="tech-logos">
            <!-- Dynamically Rendered n8n SVG Logo -->
            <div class="logo-card">
                <svg width="28" height="28" viewBox="0 0 24 24" fill="none">
                    <path d="M4 12h4m4 0h4m-8-6a3 3 0 100 6 3 3 0 000-6zm8 6a3 3 0 100 6 3 3 0 000-6z" stroke="#ff6d5a" stroke-width="2.5" stroke-linecap="round"/>
                </svg>
                <span style="color: #ff6d5a;">n8n</span>
            </div>

            <!-- Dynamically Rendered Make.com SVG Logo -->
            <div class="logo-card">
                <svg width="28" height="28" viewBox="0 0 24 24" fill="none">
                    <rect x="3" y="3" width="7" height="7" rx="2" fill="#6f00ff"/>
                    <rect x="14" y="3" width="7" height="7" rx="2" fill="#6f00ff"/>
                    <rect x="14" y="14" width="7" height="7" rx="2" fill="#6f00ff"/>
                    <rect x="3" y="14" width="7" height="7" rx="2" fill="#6f00ff"/>
                    <path d="M10 6.5h4M17.5 10v4M14 17.5h-4M6.5 14v-4" stroke="#00f2fe" stroke-width="2"/>
                </svg>
                <span style="color: #a855f7;">Make.com</span>
            </div>

            <!-- AI Engine Logo -->
            <div class="logo-card">
                <i class="fa-solid fa-brain" style="color: #00f2fe;"></i>
                <span style="color: #00f2fe;">AI Agents</span>
            </div>
        </div>
    </header>

    <main class="container">
        <h2 class="section-title">Featured Automations</h2>
        <div class="grid" style="margin-top: 1.5rem;">
            
            <div class="card">
                <div class="card-icon"><i class="fa-solid fa-robot" style="color: #ff6d5a;"></i></div>
                <h3>Autonomous AI Customer Support Agent</h3>
                <p>An end-to-end support engine using n8n, OpenAI Function Calling, and Pinecone vector store to resolve technical queries autonomously.</p>
                <div>
                    <span class="tag tag-n8n">n8n</span>
                    <span class="tag tag-ai">OpenAI</span>
                </div>
            </div>

            <div class="card">
                <div class="card-icon"><i class="fa-solid fa-diagram-project" style="color: #a855f7;"></i></div>
                <h3>Multi-Channel CRM Sync Pipeline</h3>
                <p>Make.com scenario capturing lead interactions across Webhooks, HubSpot, and Slack with automatic image generation for report digests.</p>
                <div>
                    <span class="tag tag-make">Make.com</span>
                    <span class="tag tag-ai">Midjourney / DALL-E</span>
                </div>
            </div>

            <div class="card">
                <div class="card-icon"><i class="fa-solid fa-wand-magic-sparkles" style="color: #00f2fe;"></i></div>
                <h3>Automated Content & Image Engine</h3>
                <p>Hybrid pipeline combining Make.com router logic and n8n code nodes to automatically generate articles, prompts, and visual assets.</p>
                <div>
                    <span class="tag tag-n8n">n8n</span>
                    <span class="tag tag-make">Make.com</span>
                    <span class="tag tag-ai">Stable Diffusion</span>
                </div>
            </div>

        </div>
    </main>

    <footer>
        <div class="social-links">
            <a href="https://github.com" target="_blank"><i class="fa-brands fa-github"></i></a>
            <a href="https://linkedin.com" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
            <a href="mailto:bryan@example.com"><i class="fa-solid fa-envelope"></i></a>
        </div>
        <p>© 2026 Bryan Mozar. Built for AI Automation & No-Code Orchestration.</p>
    </footer>

</body>
</html>
