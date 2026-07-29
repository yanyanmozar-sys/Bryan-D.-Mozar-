<!DOCTYPE html>
<html lang="en" class="dark scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bryan Mozar | AI & Make.com Automation Specialist</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: #0B0F17;
            color: #F3F4F6;
        }
        .glow-purple {
            box-shadow: 0 0 50px -10px rgba(147, 51, 234, 0.3);
        }
        .glow-card:hover {
            box-shadow: 0 0 30px -5px rgba(168, 85, 247, 0.25);
            border-color: rgba(168, 85, 247, 0.4);
        }
        .gradient-text {
            background: linear-gradient(135deg, #A855F7 0%, #EC4899 50%, #3B82F6 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .bg-grid {
            background-image: radial-gradient(rgba(255, 255, 255, 0.07) 1px, transparent 0);
            background-size: 24px 24px;
        }
    </style>
</head>
<body class="bg-grid antialiased selection:bg-purple-500 selection:text-white">

    <!-- Header / Navbar -->
    <header class="fixed top-0 left-0 right-0 z-50 backdrop-blur-md bg-[#0B0F17]/80 border-b border-white/10">
        <div class="max-w-6xl mx-auto px-6 h-20 flex items-center justify-between">
            <a href="#" class="text-xl font-extrabold tracking-tight">
                Bryan <span class="gradient-text">Mozar</span>
            </a>
            <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-400">
                <a href="#about" class="hover:text-purple-400 transition-colors">About</a>
                <a href="#services" class="hover:text-purple-400 transition-colors">Services</a>
                <a href="#projects" class="hover:text-purple-400 transition-colors">Automations</a>
                <a href="#stack" class="hover:text-purple-400 transition-colors">Tech Stack</a>
            </nav>
            <a href="#contact" class="px-5 py-2.5 text-sm font-semibold text-white bg-gradient-to-r from-purple-600 to-pink-600 rounded-full hover:opacity-90 transition-all glow-purple">
                Let's Connect
            </a>
        </div>
    </header>

    <main class="pt-32 px-6 max-w-6xl mx-auto">
        
        <!-- Hero Section -->
        <section id="about" class="py-16 md:py-24 flex flex-col md:flex-row items-center justify-between gap-12">
            <div class="flex-1 space-y-6">
                <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-purple-500/10 border border-purple-500/20 text-purple-400 text-xs font-semibold">
                    <i data-lucide="zap" class="w-4 h-4"></i> Make.com & AI Specialist
                </div>
                <h1 class="text-4xl sm:text-6xl font-extrabold tracking-tight leading-tight">
                    Architecting <br>
                    <span class="gradient-text">Autonomous Workflows</span> <br>
                    & AI Systems.
                </h1>
                <p class="text-gray-400 text-lg leading-relaxed max-w-xl">
                    Hi, I'm <strong class="text-white">Bryan Mozar</strong>. I help businesses eliminate repetitive manual work by building high-performing Make.com scenarios, custom API integrations, and AI agent workflows.
                </p>
                <div class="pt-4 flex flex-wrap gap-4">
                    <a href="#projects" class="px-6 py-3 bg-purple-600 hover:bg-purple-500 text-white font-semibold rounded-xl transition-all shadow-lg flex items-center gap-2">
                        View Automations <i data-lucide="arrow-right" class="w-4 h-4"></i>
                    </a>
                    <a href="https://github.com" target="_blank" class="px-6 py-3 bg-white/5 border border-white/10 hover:bg-white/10 text-white font-semibold rounded-xl transition-all flex items-center gap-2">
                        <i data-lucide="github" class="w-4 h-4"></i> GitHub Profile
                    </a>
                </div>
            </div>

            <!-- Visual Badge Card -->
            <div class="flex-1 w-full max-w-md">
                <div class="relative bg-white/5 border border-white/10 rounded-2xl p-6 backdrop-blur-xl glow-purple space-y-4">
                    <div class="flex items-center justify-between border-b border-white/10 pb-4">
                        <div class="flex items-center gap-3">
                            <div class="w-10 h-10 rounded-lg bg-purple-600/20 border border-purple-500/30 flex items-center justify-center">
                                <i data-lucide="cpu" class="w-5 h-5 text-purple-400"></i>
                            </div>
                            <div>
                                <h3 class="text-sm font-semibold text-white">Active Automation Engine</h3>
                                <p class="text-xs text-gray-400">Make.com Scenario Matrix</p>
                            </div>
                        </div>
                        <span class="inline-flex items-center gap-1.5 text-xs text-emerald-400 bg-emerald-500/10 px-2.5 py-1 rounded-full border border-emerald-500/20">
                            <span class="w-1.5 h-1.5 rounded-full bg-emerald-400 animate-pulse"></span> Running
                        </span>
                    </div>

                    <div class="space-y-3 font-mono text-xs text-gray-300">
                        <div class="bg-black/40 p-3 rounded-lg border border-white/5 flex justify-between items-center">
                            <span>Webhooks & Custom APIs</span>
                            <span class="text-purple-400">Connected</span>
                        </div>
                        <div class="bg-black/40 p-3 rounded-lg border border-white/5 flex justify-between items-center">
                            <span>LLM / OpenAI Integration</span>
                            <span class="text-purple-400">Active</span>
                        </div>
                        <div class="bg-black/40 p-3 rounded-lg border border-white/5 flex justify-between items-center">
                            <span>CRM & Database Sync</span>
                            <span class="text-purple-400">Real-time</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Services Section -->
        <section id="services" class="py-16 border-t border-white/10">
            <div class="text-center max-w-2xl mx-auto mb-12">
                <h2 class="text-3xl font-bold">What I Build</h2>
                <p class="text-gray-400 mt-2">End-to-end automation solutions tailored for scalability and zero-downtime execution.</p>
            </div>

            <div class="grid md:grid-cols-3 gap-6">
                <div class="bg-white/5 border border-white/10 p-6 rounded-2xl glow-card transition-all space-y-4">
                    <div class="w-12 h-12 rounded-xl bg-purple-500/10 border border-purple-500/20 flex items-center justify-center text-purple-400">
                        <i data-lucide="workflow" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-xl font-bold">Make.com Scenarios</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">
                        Complex multi-branch scenarios with error handling, data transformation, routing, and pagination for enterprise tools.
                    </p>
                </div>

                <div class="bg-white/5 border border-white/10 p-6 rounded-2xl glow-card transition-all space-y-4">
                    <div class="w-12 h-12 rounded-xl bg-pink-500/10 border border-pink-500/20 flex items-center justify-center text-pink-400">
                        <i data-lucide="bot" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-xl font-bold">AI Agent Workflows</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">
                        Embedding OpenAI, Claude, and custom LLM prompts directly into operational flows for smart categorization and triage.
                    </p>
                </div>

                <div class="bg-white/5 border border-white/10 p-6 rounded-2xl glow-card transition-all space-y-4">
                    <div class="w-12 h-12 rounded-xl bg-blue-500/10 border border-blue-500/20 flex items-center justify-center text-blue-400">
                        <i data-lucide="database" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-xl font-bold">API & Database Sync</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">
                        Connecting Webhooks, REST APIs, Airtable, Notion, CRM systems, and SQL databases with seamless two-way synchronizations.
                    </p>
                </div>
            </div>
        </section>

        <!-- Projects / Portfolio Section -->
        <section id="projects" class="py-16 border-t border-white/10">
            <div class="text-center max-w-2xl mx-auto mb-12">
                <h2 class="text-3xl font-bold">Featured Automations</h2>
                <p class="text-gray-400 mt-2">A snapshot of systems engineered to optimize business ops.</p>
            </div>

            <div class="grid md:grid-cols-2 gap-8">
                <!-- Project Card 1 -->
                <div class="bg-white/5 border border-white/10 rounded-2xl p-6 glow-card transition-all space-y-4">
                    <div class="flex justify-between items-center">
                        <span class="text-xs font-semibold px-3 py-1 bg-purple-500/10 text-purple-400 rounded-full border border-purple-500/20">Make.com + OpenAI</span>
                        <i data-lucide="external-link" class="w-4 h-4 text-gray-500"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white">AI Lead Qualification & CRM Router</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">
                        Captures incoming webhook leads, passes details to GPT-4o for scoring based on custom criteria, and routes high-priority prospects directly to HubSpot & Slack.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="text-xs bg-black/40 text-gray-300 px-2.5 py-1 rounded-md border border-white/5">Make.com</span>
                        <span class="text-xs bg-black/40 text-gray-300 px-2.5 py-1 rounded-md border border-white/5">OpenAI API</span>
                        <span class="text-xs bg-black/40 text-gray-300 px-2.5 py-1 rounded-md border border-white/5">HubSpot</span>
                        <span class="text-xs bg-black/40 text-gray-300 px-2.5 py-1 rounded-md border border-white/5">Slack</span>
                    </div>
                </div>

                <!-- Project Card 2 -->
                <div class="bg-white/5 border border-white/10 rounded-2xl p-6 glow-card transition-all space-y-4">
                    <div class="flex justify-between items-center">
                        <span class="text-xs font-semibold px-3 py-1 bg-pink-500/10 text-pink-400 rounded-full border border-pink-500/20">Airtable + Make.com</span>
                        <i data-lucide="external-link" class="w-4 h-4 text-gray-500"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white">Automated Content Engine</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">
                        Transforms raw video transcriptions into multi-channel social media posts, generates thumbnail concepts, and drafts scheduled newsletters automatically.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="text-xs bg-black/40 text-gray-300 px-2.5 py-1 rounded-md border border-white/5">Make.com</span>
                        <span class="text-xs bg-black/40 text-gray-300 px-2.5 py-1 rounded-md border border-white/5">Airtable</span>
                        <span class="text-xs bg-black/40 text-gray-300 px-2.5 py-1 rounded-md border border-white/5">Claude API</span>
                        <span class="text-xs bg-black/40 text-gray-300 px-2.5 py-1 rounded-md border border-white/5">LinkedIn API</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Tech Stack -->
        <section id="stack" class="py-16 border-t border-white/10">
            <div class="text-center max-w-2xl mx-auto mb-10">
                <h2 class="text-3xl font-bold">Platforms & Integrations</h2>
                <p class="text-gray-400 mt-2">Tools I use every day to connect services and build reliable pipelines.</p>
            </div>

            <div class="flex flex-wrap justify-center gap-3">
                <span class="px-4 py-2 bg-white/5 border border-white/10 rounded-xl text-sm font-medium hover:border-purple-500 transition-colors">Make.com (Integromat)</span>
                <span class="px-4 py-2 bg-white/5 border border-white/10 rounded-xl text-sm font-medium hover:border-purple-500 transition-colors">OpenAI / Claude API</span>
                <span class="px-4 py-2 bg-white/5 border border-white/10 rounded-xl text-sm font-medium hover:border-purple-500 transition-colors">Webhooks & REST APIs</span>
                <span class="px-4 py-2 bg-white/5 border border-white/10 rounded-xl text-sm font-medium hover:border-purple-500 transition-colors">JSON & Regex</span>
                <span class="px-4 py-2 bg-white/5 border border-white/10 rounded-xl text-sm font-medium hover:border-purple-500 transition-colors">Airtable / Notion</span>
                <span class="px-4 py-2 bg-white/5 border border-white/10 rounded-xl text-sm font-medium hover:border-purple-500 transition-colors">HubSpot & Salesforce</span>
                <span class="px-4 py-2 bg-white/5 border border-white/10 rounded-xl text-sm font-medium hover:border-purple-500 transition-colors">Zapier</span>
                <span class="px-4 py-2 bg-white/5 border border-white/10 rounded-xl text-sm font-medium hover:border-purple-500 transition-colors">Python Scripting</span>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="py-20 border-t border-white/10 text-center">
            <div class="max-w-xl mx-auto space-y-6">
                <h2 class="text-3xl sm:text-4xl font-extrabold">Ready to Automate Your Business?</h2>
                <p class="text-gray-400">Let's discuss how we can streamline your processes using Make.com and cutting-edge AI.</p>
                <div class="pt-4 flex justify-center gap-4">
                    <a href="mailto:bryanmozar@example.com" class="px-8 py-3.5 bg-gradient-to-r from-purple-600 to-pink-600 text-white font-semibold rounded-xl hover:opacity-90 transition-all glow-purple flex items-center gap-2">
                        <i data-lucide="mail" class="w-5 h-5"></i> Send an Email
                    </a>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="border-t border-white/10 py-8 text-center text-xs text-gray-500">
        <p>&copy; 2026 Bryan Mozar. All rights reserved. Powered by GitHub Pages.</p>
    </footer>

    <!-- Initialize Lucide Icons -->
    <script>
        lucide.createIcons();
    </script>
</body>
</html>
