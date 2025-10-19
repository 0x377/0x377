<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ahmed Gamal - Software Developer & Tester</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@300;400;600;700&family=Segoe+UI:wght@300;400;600&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a2e 50%, #16213e 100%);
            color: #e0e0e0;
            font-family: 'Segoe UI', sans-serif;
            line-height: 1.6;
            overflow-x: hidden;
            min-height: 100vh;
            padding: 20px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
        }
        
        .header {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }
        
        .gradient-text {
            background: linear-gradient(45deg, #36CFC9, #FF69B4, #FFD700, #00FFFF);
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            background-size: 300% 300%;
            animation: gradientShift 8s ease infinite;
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        h1 {
            font-size: 3.5rem;
            margin-bottom: 15px;
            font-weight: 700;
            font-family: 'JetBrains Mono', monospace;
        }
        
        .tagline {
            font-size: 1.5rem;
            margin-bottom: 25px;
            opacity: 0.9;
        }
        
        .divider {
            height: 3px;
            background: linear-gradient(90deg, transparent, #36CFC9, #FF69B4, transparent);
            margin: 30px 0;
            border-radius: 2px;
        }
        
        .section {
            margin: 40px 0;
            padding: 25px;
            background: rgba(30, 30, 46, 0.6);
            border-radius: 15px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 40px rgba(0, 0, 0, 0.4);
        }
        
        h2 {
            color: #00FFFF;
            font-size: 2rem;
            margin-bottom: 20px;
            font-family: 'JetBrains Mono', monospace;
            border-left: 4px solid #00FFFF;
            padding-left: 15px;
        }
        
        h3 {
            color: #FFD700;
            font-size: 1.4rem;
            margin: 20px 0 15px;
            font-family: 'JetBrains Mono', monospace;
        }
        
        ul {
            list-style: none;
            padding-left: 10px;
        }
        
        li {
            margin: 12px 0;
            padding-left: 25px;
            position: relative;
            font-size: 1.1rem;
        }
        
        li:before {
            content: "▹";
            position: absolute;
            left: 0;
            color: #FF69B4;
            font-weight: bold;
        }
        
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin: 15px 0;
        }
        
        .tech-badge {
            background: rgba(54, 207, 201, 0.15);
            color: #36CFC9;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 600;
            border: 1px solid rgba(54, 207, 201, 0.3);
            transition: all 0.3s ease;
            font-family: 'JetBrains Mono', monospace;
        }
        
        .tech-badge:hover {
            background: rgba(54, 207, 201, 0.3);
            transform: scale(1.05);
        }
        
        .stats-container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
            margin: 30px 0;
        }
        
        .stat-box {
            flex: 1;
            min-width: 280px;
            background: rgba(40, 40, 60, 0.7);
            border-radius: 12px;
            padding: 20px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .contact-links {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
            margin-top: 20px;
        }
        
        .contact-link {
            display: flex;
            align-items: center;
            gap: 10px;
            padding: 12px 25px;
            background: rgba(54, 207, 201, 0.1);
            border-radius: 30px;
            text-decoration: none;
            color: #e0e0e0;
            font-weight: 600;
            transition: all 0.3s ease;
            border: 1px solid rgba(54, 207, 201, 0.3);
        }
        
        .contact-link:hover {
            background: rgba(54, 207, 201, 0.2);
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(54, 207, 201, 0.2);
        }
        
        .footer {
            text-align: center;
            margin-top: 50px;
            padding: 20px;
            font-size: 1.1rem;
            color: #CCCCCC;
        }
        
        .typing-text {
            overflow: hidden;
            border-right: 2px solid #00FFFF;
            white-space: nowrap;
            margin: 0 auto;
            animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
        }
        
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #00FFFF }
        }
        
        @media (max-width: 768px) {
            h1 { font-size: 2.5rem; }
            .tagline { font-size: 1.2rem; }
            .section { padding: 20px; }
        }
        
        .pulse {
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
    </style>
</head>
<body>
    <div class="container">
        <header class="header">
            <h1 class="gradient-text">👋 Hi there, I'm <span style="color:#FF69B4;">Ahmed Gamal</span></h1>
            <p class="tagline typing-text">🚀 Software Developer & Quality Assurance Engineer</p>
            <div class="divider"></div>
        </header>
        
        <section class="section">
            <h2>🔥 About Me</h2>
            <ul>
                <li>🔭 I'm currently working on <strong style="color:#FFA500;">advanced web applications & automation testing frameworks</strong></li>
                <li>🌱 I'm currently learning <strong style="color:#00FF7F;">React Native</strong>, <strong style="color:#00FF7F;">TypeScript</strong>, and <strong style="color:#00FF7F;">advanced testing methodologies</strong></li>
                <li>💬 Ask me about <em>Web Development, Software Testing, Automation, APIs, and Open Source</em></li>
                <li>📫 How to reach me: <strong>ahmedgamalsayed.987@gmail.com</strong> or via <strong>LinkedIn</strong></li>
                <li>⚡ Fun fact: I love building side projects & exploring cutting-edge technologies 🔧</li>
            </ul>
        </section>
        
        <div class="divider"></div>
        
        <section class="section">
            <h2>🛠️ Tech Stack</h2>
            
            <h3>💻 Languages & Frameworks</h3>
            <div class="tech-stack">
                <span class="tech-badge">JavaScript</span>
                <span class="tech-badge">TypeScript</span>
                <span class="tech-badge">React</span>
                <span class="tech-badge">React Native</span>
                <span class="tech-badge">Next.js</span>
                <span class="tech-badge">Node.js</span>
                <span class="tech-badge">Express</span>
                <span class="tech-badge">Python</span>
                <span class="tech-badge">Java</span>
            </div>
            
            <h3>🗄️ Databases</h3>
            <div class="tech-stack">
                <span class="tech-badge">MongoDB</span>
                <span class="tech-badge">MySQL</span>
                <span class="tech-badge">PostgreSQL</span>
                <span class="tech-badge">Redis</span>
            </div>
            
            <h3>🧪 Testing & QA</h3>
            <div class="tech-stack">
                <span class="tech-badge">Selenium</span>
                <span class="tech-badge">Jest</span>
                <span class="tech-badge">Cypress</span>
                <span class="tech-badge">JUnit</span>
                <span class="tech-badge">TestNG</span>
                <span class="tech-badge">Postman</span>
                <span class="tech-badge">JMeter</span>
            </div>
            
            <h3>🛠️ Tools & Platforms</h3>
            <div class="tech-stack">
                <span class="tech-badge">Git</span>
                <span class="tech-badge">Docker</span>
                <span class="tech-badge">AWS</span>
                <span class="tech-badge">Jenkins</span>
                <span class="tech-badge">JIRA</span>
                <span class="tech-badge">Figma</span>
            </div>
        </section>
        
        <div class="divider"></div>
        
        <section class="section">
            <h2>📈 GitHub Analytics</h2>
            <div class="stats-container">
                <div class="stat-box">
                    <h3>Repository Stats</h3>
                    <p>Active Contributions & Project Metrics</p>
                </div>
                <div class="stat-box">
                    <h3>Top Languages</h3>
                    <p>JavaScript, TypeScript, Python, Java</p>
                </div>
            </div>
        </section>
        
        <div class="divider"></div>
        
        <section class="section">
            <h2>📫 Let's Connect</h2>
            <div class="contact-links">
                <a href="https://www.linkedin.com/in/ahmed-gamal-078838277" class="contact-link" target="_blank">
                    🔗 LinkedIn
                </a>
                <a href="https://github.com/ahmedgamal-dev" class="contact-link" target="_blank">
                    💻 GitHub
                </a>
                <a href="mailto:ahmedgamalsayed.987@gmail.com" class="contact-link">
                    📧 Email
                </a>
            </div>
        </section>
        
        <div class="footer">
            <p>⭐ Thanks for visiting my profile! Let's build something amazing together. ⭐</p>
        </div>
    </div>

    <script>
        // Dynamic typing effect
        document.addEventListener('DOMContentLoaded', function() {
            const texts = [
                "🚀 Software Developer & Quality Assurance Engineer",
                "💻 Full-Stack Developer & Automation Tester", 
                "🔧 Building Scalable Solutions & Robust Tests",
                "🎯 Passionate About Clean Code & Quality Software"
            ];
            
            let count = 0;
            let index = 0;
            let currentText = '';
            let letter = '';
            
            (function type() {
                if (count === texts.length) {
                    count = 0;
                }
                currentText = texts[count];
                letter = currentText.slice(0, ++index);
                
                document.querySelector('.typing-text').textContent = letter;
                if (letter.length === currentText.length) {
                    count++;
                    index = 0;
                    setTimeout(type, 2000);
                } else {
                    setTimeout(type, 100);
                }
            })();
            
            // Add pulse animation to tech badges on hover
            const badges = document.querySelectorAll('.tech-badge');
            badges.forEach(badge => {
                badge.addEventListener('mouseenter', function() {
                    this.classList.add('pulse');
                });
                badge.addEventListener('mouseleave', function() {
                    this.classList.remove('pulse');
                });
            });
        });
    </script>
</body>
</html>
