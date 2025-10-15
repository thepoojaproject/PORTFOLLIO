
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minimal Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #fafafa;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            padding: 30px 0;
            border-bottom: 1px solid #eee;
            position: sticky;
            top: 0;
            background-color: rgba(250, 250, 250, 0.95);
            backdrop-filter: blur(5px);
            z-index: 100;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-weight: 600;
            font-size: 1.5rem;
            color: #222;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav li {
            margin-left: 30px;
        }
        
        nav a {
            text-decoration: none;
            color: #555;
            font-weight: 400;
            transition: color 0.3s;
        }
        
        nav a:hover {
            color: #222;
        }
        
        /* Hero Section */
        .hero {
            padding: 100px 0;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3rem;
            font-weight: 500;
            margin-bottom: 20px;
            color: #222;
        }
        
        .hero p {
            font-size: 1.2rem;
            color: #666;
            max-width: 600px;
            margin: 0 auto 30px;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 30px;
            background-color: #222;
            color: white;
            text-decoration: none;
            border-radius: 4px;
            font-weight: 500;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #444;
        }
        
        /* About Section */
        .about {
            padding: 100px 0;
            border-top: 1px solid #eee;
        }
        
        .section-title {
            font-size: 1.8rem;
            font-weight: 500;
            margin-bottom: 40px;
            color: #222;
        }
        
        .about-content {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 50px;
            align-items: center;
        }
        
        .about-text p {
            margin-bottom: 20px;
            color: #555;
        }
        
        /* Projects Section */
        .projects {
            padding: 100px 0;
            border-top: 1px solid #eee;
        }
        
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .project-card {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .project-info {
            padding: 25px;
        }
        
        .project-title {
            font-size: 1.2rem;
            font-weight: 500;
            margin-bottom: 10px;
            color: #222;
        }
        
        .project-desc {
            color: #666;
            font-size: 0.95rem;
        }
        
        /* Contact Section */
        .contact {
            padding: 100px 0;
            border-top: 1px solid #eee;
        }
        
        .contact-form {
            max-width: 500px;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: #444;
        }
        
        .form-control {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-family: 'Inter', sans-serif;
            font-size: 1rem;
            transition: border-color 0.3s;
        }
        
        .form-control:focus {
            outline: none;
            border-color: #222;
        }
        
        textarea.form-control {
            min-height: 150px;
            resize: vertical;
        }
        
        /* Footer */
        footer {
            padding: 40px 0;
            border-top: 1px solid #eee;
            text-align: center;
            color: #777;
            font-size: 0.9rem;
        }
        
        .heart {
            color: #e74c3c;
            display: inline-block;
            animation: heartbeat 1.5s infinite;
        }
        
        @keyframes heartbeat {
            0% {
                transform: scale(1);
            }
            5% {
                transform: scale(1.1);
            }
            10% {
                transform: scale(1);
            }
            15% {
                transform: scale(1.2);
            }
            50% {
                transform: scale(1);
            }
            100% {
                transform: scale(1);
            }
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 20px;
            }
            
            nav li {
                margin: 0 15px;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .about-content {
                grid-template-columns: 1fr;
                gap: 30px;
            }
            
            .project-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">Portfolio</div>
                <nav>
                    <ul>
                        <li><a href="#about">About</a></li>
                        <li><a href="#projects">Projects</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Minimal & Effective Design</h1>
            <p>I create clean, functional websites with focus on user experience and performance.</p>
            <a href="#projects" class="btn">View Projects</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <div class="container">
            <h2 class="section-title">About Me</h2>
            <div class="about-content">
                <div>
                    <svg width="200" height="200" viewBox="0 0 200 200" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <circle cx="100" cy="100" r="90" fill="#f0f0f0" stroke="#ddd" stroke-width="2"/>
                        <circle cx="100" cy="80" r="25" fill="#ddd"/>
                        <path d="M60 140 C60 120, 140 120, 140 140" stroke="#ddd" stroke-width="8" stroke-linecap="round" fill="none"/>
                    </svg>
                </div>
                <div class="about-text">
                    <p>I'm a web developer with a passion for creating clean, functional interfaces. My approach focuses on simplicity, usability, and performance.</p>
                    <p>With expertise in modern web technologies, I build digital experiences that are both beautiful and effective.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects">
        <div class="container">
            <h2 class="section-title">Projects</h2>
            <div class="project-grid">
                <div class="project-card">
                    <div class="project-info">
                        <h3 class="project-title">Minimal E-commerce</h3>
                        <p class="project-desc">A clean online store with focus on user experience and conversion optimization.</p>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-info">
                        <h3 class="project-title">Portfolio Website</h3>
                        <p class="project-desc">A personal portfolio showcasing work with elegant design and smooth interactions.</p>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-info">
                        <h3 class="project-title">Task Management App</h3>
                        <p class="project-desc">A productivity tool with intuitive interface and powerful organization features.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title">Get in Touch</h2>
            <form class="contact-form">
                <div class="form-group">
                    <label for="name">Name</label>
                    <input type="text" id="name" class="form-control" placeholder="Your name">
                </div>
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" class="form-control" placeholder="Your email">
                </div>
                <div class="form-group">
                    <label for="message">Message</label>
                    <textarea id="message" class="form-control" placeholder="Your message"></textarea>
                </div>
                <button type="submit" class="btn">Send Message</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>Made in <span class="heart">💖</span> By Armeen</p>
        </div>
    </footer>

    <script>
        // Simple form submission handler
        document.querySelector('.contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message. I will get back to you soon.');
            this.reset();
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                window.scrollTo({
                    top: targetElement.offsetTop - 80,
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
