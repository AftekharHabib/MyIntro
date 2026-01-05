<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aftekhar Habib | Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #00d2ff;
            --secondary: #3a7bd5;
            --bg: #0f172a;
            --card-bg: rgba(30, 41, 59, 0.7);
            --text: #f1f5f9;
            --text-muted: #94a3b8;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg);
            background-image: radial-gradient(circle at 50% 50%, #1e293b 0%, #0f172a 100%);
            color: var(--text);
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 40px auto;
        }

        /* Profile Header */
        header {
            text-align: center;
            margin-bottom: 50px;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 10px;
            background: linear-gradient(to right, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .subtitle {
            font-size: 1.2rem;
            color: var(--text-muted);
            letter-spacing: 1px;
        }

        /* Glass Cards */
        .card {
            background: var(--card-bg);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 16px;
            padding: 30px;
            margin-bottom: 30px;
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        h2 {
            font-size: 1.5rem;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
            color: var(--primary);
        }

        /* Skills Tags */
        .skills-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .skill-tag {
            background: rgba(0, 210, 255, 0.1);
            border: 1px solid var(--primary);
            color: var(--primary);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 500;
        }

        /* Projects Section */
        .project-item {
            border-left: 3px solid var(--secondary);
            padding-left: 20px;
            margin-bottom: 25px;
        }

        .project-item h3 {
            color: var(--text);
            margin-bottom: 5px;
        }

        .project-link {
            color: var(--primary);
            text-decoration: none;
            font-size: 0.9rem;
            display: inline-block;
            margin-bottom: 8px;
        }

        .project-link:hover {
            text-decoration: underline;
        }

        /* Contact Section */
        .contact-links {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 15px;
            color: var(--text);
            text-decoration: none;
            padding: 10px;
            border-radius: 8px;
            background: rgba(255, 255, 255, 0.05);
        }

        .contact-item:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        .contact-item i {
            color: var(--primary);
            font-size: 1.2rem;
        }

        @media (max-width: 600px) {
            h1 { font-size: 2rem; }
            .card { padding: 20px; }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Aftekhar Habib</h1>
            <p class="subtitle">FULL-STACK DEVELOPER • BACKEND ARCHITECT</p>
        </header>

        <section class="card">
            <h2><i class="fas fa-user"></i> About Me</h2>
            <p>I am a final-year Computer Science & Engineering student at <b>Varendra University</b>. I specialize in bridging the gap between complex backend logic and intuitive user interfaces. Whether it’s architecting RESTful APIs with <b>Django</b> or crafting responsive mobile experiences with <b>React Native</b>, I focus on writing clean, efficient, and maintainable code.</p>
        </section>

        <section class="card">
            <h2><i class="fas fa-code"></i> Technical Toolkit</h2>
            <div class="skills-grid">
                <span class="skill-tag">Python</span>
                <span class="skill-tag">Django</span>
                <span class="skill-tag">Django REST Framework</span>
                <span class="skill-tag">JavaScript (ES6+)</span>
                <span class="skill-tag">React.js</span>
                <span class="skill-tag">React Native</span>
                <span class="skill-tag">Node.js</span>
                <span class="skill-tag">MongoDB</span>
                <span class="skill-tag">PostgreSQL</span>
                <span class="skill-tag">Git & GitHub</span>
            </div>
        </section>

        <section class="card">
            <h2><i class="fas fa-project-diagram"></i> Featured Impact</h2>
            
            <div class="project-item">
                <h3>Babymeal.shop | E-commerce Ecosystem</h3>
                <a href="http://www.babymeal.shop" class="project-link">Visit Website <i class="fas fa-external-link-alt"></i></a>
                <p>Built a production-ready store using Django. Integrated automated product management, secure user authentication, and a customized admin dashboard to streamline sales.</p>
            </div>

            <div class="project-item">
                <h3>Geo-Fencing Smart Attendance</h3>
                <span class="project-link" style="color: var(--text-muted);">Academic Innovation</span>
                <p>Engineered a mobile solution using React Native and GPS APIs to automate attendance verification within specific geographic radii, ensuring 100% accuracy for institutions.</p>
            </div>
        </section>

        <section class="card">
            <h2><i class="fas fa-graduation-cap"></i> Education</h2>
            <p><b>B.Sc. in Computer Science & Engineering</b></p>
            <p style="color: var(--text-muted);">Varendra University | 2022 – Present</p>
        </section>

        <section class="card">
            <h2><i class="fas fa-envelope"></i> Let's Connect</h2>
            <div class="contact-links">
                <a href="mailto:rouhithmini1@gmail.com" class="contact-item">
                    <i class="fas fa-envelope"></i>
                    rouhithmini1@gmail.com
                </a>
                <a href="https://github.com/AftekharHabib" target="_blank" class="contact-item">
                    <i class="fab fa-github"></i>
                    GitHub Profile
                </a>
                <a href="#" class="contact-item">
                    <i class="fas fa-map-marker-alt"></i>
                    Rajshahi, Bangladesh
                </a>
                <a href="tel:01783570142" class="contact-item">
                    <i class="fas fa-phone"></i>
                    01783570142
                </a>
            </div>
        </section>
    </div>

</body>
</html>
