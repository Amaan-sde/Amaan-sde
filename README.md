<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amaan Khan - Software Engineer Portfolio README</title>
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;600&family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --bg-color: #0d1117;
            --card-bg: #161b22;
            --border-color: #30363d;
            --text-primary: #c9d1d9;
            --text-secondary: #8b949e;
            --accent-green: #238636;
            --accent-green-hover: #2ea043;
            --accent-blue: #58a6ff;
            --accent-purple: #bc8cff;
            --accent-orange: #ffa657;
            --glow-color: rgba(88, 166, 255, 0.15);
        }

        [data-theme="light"] {
            --bg-color: #f6f8fa;
            --card-bg: #ffffff;
            --border-color: #d0d7de;
            --text-primary: #24292f;
            --text-secondary: #57606a;
            --accent-green: #1f883d;
            --accent-green-hover: #1a7f37;
            --accent-blue: #0969da;
            --accent-purple: #8250df;
            --accent-orange: #bc4c00;
            --glow-color: rgba(9, 105, 218, 0.1);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            transition: background-color 0.3s ease, color 0.3s ease, border-color 0.3s ease;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-primary);
            line-height: 1.6;
            padding: 2rem 1rem;
            display: flex;
            justify-content: center;
        }

        .container {
            width: 100%;
            max-width: 900px;
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            box-shadow: 0 8px 24px rgba(0,0,0,0.2);
            overflow: hidden;
            position: relative;
        }

        /* Top Bar / README Header */
        .readme-header {
            background: linear-gradient(135deg, var(--card-bg), var(--bg-color));
            padding: 1rem 1.5rem;
            border-bottom: 1px solid var(--border-color);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .readme-title {
            display: flex;
            align-items: center;
            gap: 10px;
            font-family: 'Fira Code', monospace;
            font-size: 0.95rem;
            color: var(--text-secondary);
        }

        .readme-title i {
            color: var(--accent-blue);
        }

        .controls {
            display: flex;
            gap: 10px;
            align-items: center;
        }

        .theme-toggle, .btn-action {
            background: transparent;
            border: 1px solid var(--border-color);
            color: var(--text-primary);
            padding: 6px 12px;
            border-radius: 6px;
            cursor: pointer;
            font-size: 0.85rem;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .theme-toggle:hover, .btn-action:hover {
            background: var(--border-color);
        }

        /* Content Padding */
        .content {
            padding: 2.5rem;
        }

        h1, h2, h3 {
            font-weight: 800;
            letter-spacing: -0.025em;
        }

        .hero {
            text-align: center;
            margin-bottom: 2.5rem;
            position: relative;
        }

        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
            background: linear-gradient(90deg, var(--accent-blue), var(--accent-purple));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero p {
            font-size: 1.1rem;
            color: var(--text-secondary);
            margin-bottom: 1.5rem;
        }

        .badges {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 8px;
            margin-bottom: 1.5rem;
        }

        .badge {
            background: var(--glow-color);
            border: 1px solid var(--border-color);
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            color: var(--accent-blue);
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 6px;
        }

        .badge:hover {
            border-color: var(--accent-blue);
        }

        /* Sections */
        section {
            margin-bottom: 2.5rem;
        }

        h2 {
            font-size: 1.5rem;
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 0.5rem;
            margin-bottom: 1.2rem;
            display: flex;
            align-items: center;
            gap: 10px;
            color: var(--text-primary);
        }

        h2 i {
            color: var(--accent-orange);
            font-size: 1.2rem;
        }

        /* Skills Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1rem;
        }

        .skill-card {
            background: var(--bg-color);
            border: 1px solid var(--border-color);
            padding: 1.2rem;
            border-radius: 8px;
            position: relative;
            overflow: hidden;
        }

        .skill-card h3 {
            font-size: 1rem;
            margin-bottom: 0.8rem;
            color: var(--accent-purple);
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .tag-list {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
        }

        .tag {
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            padding: 4px 8px;
            font-size: 0.75rem;
            border-radius: 4px;
            font-family: 'Fira Code', monospace;
            color: var(--text-primary);
        }

        /* Timeline / Experience & Projects */
        .timeline-item {
            background: var(--bg-color);
            border: 1px solid var(--border-color);
            border-radius: 8px;
            padding: 1.5rem;
            margin-bottom: 1.2rem;
            position: relative;
        }

        .timeline-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 0.8rem;
        }

        .timeline-title {
            font-size: 1.1rem;
            font-weight: 700;
            color: var(--text-primary);
        }

        .timeline-subtitle {
            font-size: 0.9rem;
            color: var(--accent-blue);
            font-weight: 600;
        }

        .timeline-date {
            font-family: 'Fira Code', monospace;
            font-size: 0.8rem;
            background: var(--glow-color);
            padding: 4px 8px;
            border-radius: 4px;
            color: var(--accent-orange);
            border: 1px solid var(--border-color);
        }

        ul {
            list-style-type: none;
            padding-left: 0;
        }

        ul li {
            position: relative;
            padding-left: 20px;
            margin-bottom: 0.6rem;
            color: var(--text-secondary);
            font-size: 0.95rem;
        }

        ul li::before {
            content: '▹';
            position: absolute;
            left: 0;
            color: var(--accent-green);
            font-weight: bold;
        }

        /* Stats & Footer */
        .stats-section {
            text-align: center;
            background: var(--bg-color);
            border: 1px solid var(--border-color);
            padding: 1.5rem;
            border-radius: 8px;
            margin-top: 2rem;
        }

        .stats-section img {
            max-width: 100%;
            border-radius: 6px;
            margin-top: 1rem;
        }

        .footer {
            text-align: center;
            padding: 1.5rem;
            border-top: 1px solid var(--border-color);
            color: var(--text-secondary);
            font-size: 0.85rem;
            font-family: 'Fira Code', monospace;
        }

        /* Interactive Easter Egg */
        .quote-box {
            background: var(--glow-color);
            border-left: 4px solid var(--accent-blue);
            padding: 1rem;
            border-radius: 0 8px 8px 0;
            margin-top: 1.5rem;
            font-style: italic;
            color: var(--text-primary);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .interactive-btn {
            background: var(--accent-blue);
            color: #fff;
            border: none;
            padding: 6px 12px;
            border-radius: 4px;
            font-size: 0.75rem;
            font-family: 'Inter', sans-serif;
            font-weight: 600;
            cursor: pointer;
        }

        .interactive-btn:hover {
            opacity: 0.9;
        }

        @media(max-width: 768px) {
            .content { padding: 1.2rem; }
            .hero h1 { font-size: 2rem; }
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- README File Header Toolbar -->
        <div class="readme-header">
            <div class="readme-title">
                <i class="fa-solid fa-book-open"></i>
                <span>README.md — Amaan Khan Profile</span>
            </div>
            <div class="controls">
                <button class="theme-toggle" id="themeToggleBtn">
                    <i class="fa-solid fa-moon" id="themeIcon"></i> <span id="themeText">Dark</span>
                </button>
                <button class="btn-action" onclick="copyReadmeCode()">
                    <i class="fa-solid fa-copy"></i> Copy HTML
                </button>
            </div>
        </div>

        <!-- Main README Body Content -->
        <div class="content">
            
            <!-- Hero Section -->
            <div class="hero">
                <h1>Hi there, I'm Amaan Khan <span class="wave">👋</span></h1>
                <p>Software Engineer specializing in full-stack architecture & high-performance applications [cite: 1].</p>
                
                <div class="badges">
                    <a href="mailto:amaankhan172595@gmail.com" class="badge"><i class="fa-solid fa-envelope"></i> Email Me</a>
                    <a href="https://github.com/Amaan-sde" target="_blank" class="badge"><i class="fa-brands fa-github"></i> GitHub</a>
                    <a href="https://www.linkedin.com/in/Amaan_Khan1" target="_blank" class="badge"><i class="fa-brands fa-linkedin"></i> LinkedIn</a>
                    <a href="https://leetcode.com/u/Amaan_Khan1/" target="_blank" class="badge"><i class="fa-solid fa-code"></i> LeetCode (9690978277)</a>
                </div>
            </div>

            <!-- About Me Section -->
            <section>
                <h2><i class="fa-solid fa-user-astronaut"></i> About Me</h2>
                <p style="color: var(--text-secondary); margin-bottom: 1rem;">
                    Software Engineer specializing in full-stack development and production deployment, building scalable, high-performance applications with Flutter, React, NestJS, and Java [cite: 1]. Proficient in RESTful APIs, cloud-native deployment, and modern DevOps practices, with a strong foundation in Data Structures & Algorithms [cite: 1].
                </p>
                <p style="color: var(--text-secondary);">
                    Currently pursuing B.Tech in Computer Science & Engineering (Expected 2027) at Birla Institute of Applied Sciences, Bhimtal, Uttarakhand (CGPA: 7.3/10) [cite: 1].
                </p>

                <div class="quote-box">
                    <span id="quoteText">"Building scalable systems and robust cloud architectures, one commit at a time."</span>
                    <button class="interactive-btn" onclick="rotateQuote()">New Quote ⚡</button>
                </div>
            </section>

            <!-- Skills Matrix Section -->
            <section>
                <h2><i class="fa-solid fa-toolbox"></i> Tech Stack & Core Skills</h2>
                <div class="skills-grid">
                    <div class="skill-card">
                        <h3><i class="fa-solid fa-code"></i> Languages</h3>
                        <div class="tag-list">
                            <span class="tag">Java</span>
                            <span class="tag">JavaScript</span>
                            <span class="tag">TypeScript</span>
                            <span class="tag">C++</span>
                            <span class="tag">C</span>
                            <span class="tag">Python</span>
                        </div>
                    </div>
                    <div class="skill-card">
                        <h3><i class="fa-solid fa-layer-group"></i> Frameworks & Tech</h3>
                        <div class="tag-list">
                            <span class="tag">React</span>
                            <span class="tag">Flutter</span>
                            <span class="tag">Node.js</span>
                            <span class="tag">Express.js</span>
                            <span class="tag">NestJS</span>
                            <span class="tag">Tailwind CSS</span>
                        </div>
                    </div>
                    <div class="skill-card">
                        <h3><i class="fa-solid fa-cloud"></i> Databases & DevOps</h3>
                        <div class="tag-list">
                            <span class="tag">MySQL</span>
                            <span class="tag">MongoDB</span>
                            <span class="tag">Redis</span>
                            <span class="tag">AWS</span>
                            <span class="tag">Docker</span>
                            <span class="tag">Kubernetes</span>
                            <span class="tag">Nginx</span>
                            <span class="tag">CI/CD</span>
                        </div>
                    </div>
                    <div class="skill-card">
                        <h3><i class="fa-solid fa-screwdriver-wrench"></i> Tools & Concepts</h3>
                        <div class="tag-list">
                            <span class="tag">Git & GitHub</span>
                            <span class="tag">Postman</span>
                            <span class="tag">REST APIs</span>
                            <span class="tag">DSA</span>
                            <span class="tag">OOP</span>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Professional Experience -->
            <section>
                <h2><i class="fa-solid fa-briefcase"></i> Professional Experience</h2>
                
                <div class="timeline-item">
                    <div class="timeline-header">
                        <div>
                            <div class="timeline-title">Software Engineer</div>
                            <div class="timeline-subtitle">Wotpan | Kashipur, Uttarakhand [cite: 1]</div>
                        </div>
                        <div class="timeline-date">Nov 2025 - Present [cite: 1]</div>
                    </div>
                    <ul>
                        <li>Developed and maintained cross-platform mobile applications using <b>Flutter</b>, building reusable UI components and integrating REST APIs for Android & iOS [cite: 1].</li>
                        <li>Built and maintained scalable backend services using <b>NestJS</b>, implementing RESTful APIs, JWT authentication, and modular architecture [cite: 1].</li>
                        <li>Containerized and deployed apps using <b>Docker</b>, configured <b>Nginx</b> reverse proxies, managed processes with <b>PM2</b>, and secured SSL production environments [cite: 1].</li>
                        <li>Implemented <b>CI/CD pipelines</b> to automate build and deployment workflows for fast, consistent application releases [cite: 1].</li>
                        <li>Collaborated across frontend, backend, and DevOps teams to troubleshoot production issues in an agile environment [cite: 1].</li>
                    </ul>
                </div>
            </section>

            <!-- Featured Projects -->
            <section>
                <h2><i class="fa-solid fa-rocket"></i> Featured Projects</h2>

                <div class="timeline-item">
                    <div class="timeline-header">
                        <div>
                            <div class="timeline-title">AI Conversational Assistant</div>
                            <div class="timeline-subtitle">Full-Stack AI Platform [cite: 1]</div>
                        </div>
                        <div class="timeline-date">React • Express • MongoDB</div>
                    </div>
                    <ul>
                        <li>Engineered a full-stack AI platform with modular architecture using <b>React.js</b>, <b>Express.js</b>, and <b>MongoDB</b> [cite: 1].</li>
                        <li>Developed secure authentication & session management using <b>JWT</b>, HTTP-only cookies, and <b>bcrypt</b> encryption [cite: 1].</li>
                        <li>Optimized REST API integration with Axios and built responsive, reusable React components [cite: 1].</li>
                        <li>Integrated <b>Cloudinary</b> media management for efficient asset handling and data processing [cite: 1].</li>
                    </ul>
                </div>

                <div class="timeline-item">
                    <div class="timeline-header">
                        <div>
                            <div class="timeline-title">LaunchPad</div>
                            <div class="timeline-subtitle">Portfolio Platform [cite: 1]</div>
                        </div>
                        <div class="timeline-date">React • Tailwind • Vercel</div>
                    </div>
                    <ul>
                        <li>Engineered a portfolio platform using <b>React.js</b> and <b>Tailwind CSS</b> leveraging component-based architecture [cite: 1].</li>
                        <li>Optimized performance through lazy loading, responsive layouts, and modern frontend practices [cite: 1].</li>
                        <li>Designed a pixel-perfect, mobile-first interface ensuring accessibility and rapid UI development [cite: 1].</li>
                        <li>Deployed on <b>Vercel</b> enabling automated builds, continuous deployment, and high-availability hosting [cite: 1].</li>
                    </ul>
                </div>
            </section>

            <!-- Certifications & Achievements -->
            <section>
                <h2><i class="fa-solid fa-award"></i> Certifications & Achievements</h2>
                <div class="skills-grid">
                    <div class="skill-card" style="text-align: center;">
                        <i class="fa-solid fa-space-shuttle" style="font-size: 2rem; color: var(--accent-blue); margin-bottom: 0.5rem;"></i>
                        <h3 style="justify-content: center;">NASA Space Apps Challenge</h3>
                        <p style="font-size: 0.85rem; color: var(--text-secondary);">Official Participant [cite: 1]</p>
                    </div>
                    <div class="skill-card" style="text-align: center;">
                        <i class="fa-brands fa-aws" style="font-size: 2rem; color: var(--accent-orange); margin-bottom: 0.5rem;"></i>
                        <h3 style="justify-content: center;">AWS Cloud Quest</h3>
                        <p style="font-size: 0.85rem; color: var(--text-secondary);">Cloud Practitioner Certification [cite: 1]</p>
                    </div>
                </div>
            </section>

            <!-- GitHub Stats Visualizer -->
            <div class="stats-section">
                <h3>GitHub Contribution Stats & Metrics</h3>
                <p style="font-size: 0.85rem; color: var(--text-secondary); margin-top: 0.3rem;">Real-time tracking of code quality and activity.</p>
                <img src="https://github-readme-stats.vercel.app/api?username=Amaan-sde&show_icons=true&theme=tokyonight&hide_border=true&bg_color=161b22" alt="Amaan's GitHub Stats">
            </div>

        </div>

        <!-- Footer -->
        <div class="footer">
            Designed with HTML5, CSS3 & JavaScript • Amaan Khan © 2026
        </div>
    </div>

    <!-- JavaScript for Interactivity -->
    <script>
        // Theme Toggle Functionality
        const themeToggleBtn = document.getElementById('themeToggleBtn');
        const themeIcon = document.getElementById('themeIcon');
        const themeText = document.getElementById('themeText');
        const htmlElement = document.documentElement;

        themeToggleBtn.addEventListener('click', () => {
            if (htmlElement.getAttribute('data-theme') === 'light') {
                htmlElement.removeAttribute('data-theme');
                themeIcon.className = 'fa-solid fa-moon';
                themeText.textContent = 'Dark';
            } else {
                htmlElement.setAttribute('data-theme', 'light');
                themeIcon.className = 'fa-solid fa-sun';
                themeText.textContent = 'Light';
            }
        });

        // Interactive Quotes Array
        const quotes = [
            "Building scalable systems and robust cloud architectures, one commit at a time.",
            "Clean code always looks like it was written by someone who cares.",
            "Turning complex backend logic into seamless, high-performance user experiences.",
            "Automate everything. Deploy with confidence. Scale infinitely."
        ];

        function rotateQuote() {
            const quoteElem = document.getElementById('quoteText');
            const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
            quoteElem.style.opacity = 0;
            setTimeout(() => {
                quoteElem.textContent = `"${randomQuote}"`;
                quoteElem.style.opacity = 1;
            }, 200);
        }

         Copy HTML Function
        function copyReadmeCode() {
            const fullHtml = document.documentElement.outerHTML;
            navigator.clipboard.writeText(fullHtml).then(() => {
                alert('HTML README code copied successfully to clipboard! You can now paste and save it as index.html');
            }).catch(err => {
                console.error('Failed to copy text: ', err);
            });
        }
    </script>
</body>
</html>
