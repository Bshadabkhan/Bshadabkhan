<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shadab Khan B | AI & ML Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            position: relative;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 20px;
            animation: fadeInUp 1s ease;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .typing-text {
            font-size: 1.5rem;
            margin-bottom: 30px;
            min-height: 50px;
            color: #ffd700;
            animation: fadeInUp 1s ease 0.3s both;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            line-height: 1.8;
            margin-bottom: 40px;
            animation: fadeInUp 1s ease 0.6s both;
        }

        .social-links {
            display: flex;
            gap: 20px;
            animation: fadeInUp 1s ease 0.9s both;
        }

        .social-btn {
            padding: 15px 30px;
            background: rgba(255,255,255,0.2);
            border: 2px solid #fff;
            border-radius: 50px;
            color: #fff;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .social-btn:hover {
            background: #fff;
            color: #667eea;
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }

        /* About Section */
        .section {
            padding: 80px 20px;
            animation: fadeIn 1s ease;
        }

        .section-title {
            font-size: 3rem;
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 100px;
            height: 4px;
            background: #ffd700;
            margin: 20px auto;
        }

        .about-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .about-card {
            background: rgba(255,255,255,0.1);
            padding: 30px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
            transition: all 0.3s ease;
        }

        .about-card:hover {
            transform: translateY(-10px);
            background: rgba(255,255,255,0.2);
            box-shadow: 0 20px 40px rgba(0,0,0,0.3);
        }

        .about-card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: #ffd700;
        }

        /* Skills Section */
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }

        .skill-category {
            background: rgba(255,255,255,0.1);
            padding: 30px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
        }

        .skill-category h3 {
            font-size: 1.8rem;
            margin-bottom: 25px;
            color: #ffd700;
        }

        .skill-item {
            margin-bottom: 20px;
        }

        .skill-name {
            display: flex;
            justify-content: space-between;
            margin-bottom: 8px;
            font-size: 1.1rem;
        }

        .skill-bar {
            background: rgba(255,255,255,0.2);
            height: 10px;
            border-radius: 10px;
            overflow: hidden;
        }

        .skill-progress {
            height: 100%;
            background: linear-gradient(90deg, #ffd700, #ffed4e);
            border-radius: 10px;
            animation: skillLoad 1.5s ease-out;
        }

        @keyframes skillLoad {
            from { width: 0; }
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
        }

        .project-card {
            background: rgba(255,255,255,0.1);
            border-radius: 20px;
            overflow: hidden;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.4);
        }

        .project-icon {
            font-size: 4rem;
            padding: 40px;
            text-align: center;
            background: rgba(255,255,255,0.1);
        }

        .project-content {
            padding: 30px;
        }

        .project-content h3 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            color: #ffd700;
        }

        .project-content p {
            line-height: 1.6;
            margin-bottom: 15px;
        }

        .tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }

        .tech-tag {
            padding: 5px 15px;
            background: rgba(255,255,255,0.2);
            border-radius: 20px;
            font-size: 0.9rem;
        }

        /* Contact Section */
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .contact-card {
            background: rgba(255,255,255,0.1);
            padding: 30px;
            border-radius: 20px;
            text-align: center;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
            transition: all 0.3s ease;
            text-decoration: none;
            color: #fff;
        }

        .contact-card:hover {
            background: rgba(255,255,255,0.2);
            transform: scale(1.05);
        }

        .contact-icon {
            font-size: 3rem;
            margin-bottom: 15px;
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        /* Floating particles */
        .particle {
            position: fixed;
            width: 10px;
            height: 10px;
            background: rgba(255,255,255,0.3);
            border-radius: 50%;
            pointer-events: none;
            animation: float 15s infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0) translateX(0); }
            25% { transform: translateY(-100px) translateX(50px); }
            50% { transform: translateY(-200px) translateX(-50px); }
            75% { transform: translateY(-100px) translateX(100px); }
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2.5rem; }
            .typing-text { font-size: 1.2rem; }
            .section-title { font-size: 2rem; }
            .social-links { flex-direction: column; }
        }
    </style>
</head>
<body>
    <!-- Floating Particles -->
    <div class="particle" style="top: 10%; left: 10%; animation-delay: 0s;"></div>
    <div class="particle" style="top: 20%; left: 80%; animation-delay: 2s;"></div>
    <div class="particle" style="top: 50%; left: 20%; animation-delay: 4s;"></div>
    <div class="particle" style="top: 70%; left: 70%; animation-delay: 6s;"></div>
    <div class="particle" style="top: 40%; left: 90%; animation-delay: 8s;"></div>

    <!-- Hero Section -->
    <section class="hero">
        <h1>Hi There! 👋 I'm Shadab Khan B</h1>
        <div class="typing-text" id="typing"></div>
        <p>Passionate about AI, Machine Learning, Generative AI, and Full-Stack Python Development. I build automation tools, AI agents, OCR pipelines, RAG systems, and developer tools.</p>
        <div class="social-links">
            <a href="mailto:shadabkhanbenki@gmail.com" class="social-btn">📧 Email</a>
            <a href="https://www.linkedin.com/in/shadab-khan-b-41b6a8270" target="_blank" class="social-btn">💼 LinkedIn</a>
            <a href="https://github.com/Bshadabkhan" target="_blank" class="social-btn">💻 GitHub</a>
        </div>
    </section>

    <!-- About Section -->
    <section class="section">
        <div class="container">
            <h2 class="section-title">🚀 About Me</h2>
            <div class="about-grid">
                <div class="about-card">
                    <h3>🔭 Current Work</h3>
                    <p>Working on AI Voice Assistants, RAG Chatbots, and Resume AI Tools</p>
                </div>
                <div class="about-card">
                    <h3>🌱 Learning</h3>
                    <p>DeepSeek Fine-tuning, CrewAI, and Agentic Workflows</p>
                </div>
                <div class="about-card">
                    <h3>🧩 Passion</h3>
                    <p>Solving real-world problems using AI & Python</p>
                </div>
                <div class="about-card">
                    <h3>💬 Expertise</h3>
                    <p>AI, ML, Python, Automation, Streamlit</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section class="section" style="background: rgba(0,0,0,0.2);">
        <div class="container">
            <h2 class="section-title">🛠️ Tech Stack</h2>
            <div class="skills-container">
                <div class="skill-category">
                    <h3>🤖 AI & Machine Learning</h3>
                    <div class="skill-item">
                        <div class="skill-name"><span>Python</span><span>95%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 95%"></div></div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name"><span>OpenAI GPT / LangChain</span><span>90%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 90%"></div></div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name"><span>TensorFlow / PyTorch</span><span>85%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 85%"></div></div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name"><span>RAG Systems</span><span>90%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 90%"></div></div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name"><span>NLP / Computer Vision</span><span>85%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 85%"></div></div>
                    </div>
                </div>

                <div class="skill-category">
                    <h3>⚙️ Backend & APIs</h3>
                    <div class="skill-item">
                        <div class="skill-name"><span>FastAPI</span><span>90%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 90%"></div></div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name"><span>Flask / Django</span><span>85%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 85%"></div></div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name"><span>REST APIs</span><span>90%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 90%"></div></div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name"><span>WebSockets</span><span>80%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 80%"></div></div>
                    </div>
                </div>

                <div class="skill-category">
                    <h3>🗄️ Database & Tools</h3>
                    <div class="skill-item">
                        <div class="skill-name"><span>PostgreSQL / MongoDB</span><span>85%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 85%"></div></div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name"><span>ChromaDB / Pinecone</span><span>90%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 90%"></div></div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name"><span>Docker</span><span>80%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 80%"></div></div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name"><span>Git / GitHub</span><span>90%</span></div>
                        <div class="skill-bar"><div class="skill-progress" style="width: 90%"></div></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section class="section">
        <div class="container">
            <h2 class="section-title">⭐ Featured Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-icon">🎤</div>
                    <div class="project-content">
                        <h3>AccessGpt Voice</h3>
                        <p>Real-time AI voice assistant with Speech-to-Text, Text-to-Speech, and GPT integration for seamless voice interactions.</p>
                        <div class="tech-tags">
                            <span class="tech-tag">Python</span>
                            <span class="tech-tag">Realtime STT</span>
                            <span class="tech-tag">OpenAI</span>
                            <span class="tech-tag">Speech Pipeline</span>
                        </div>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-icon">📄</div>
                    <div class="project-content">
                        <h3>ATS Resume Analysis</h3>
                        <p>ATS-powered Resume Analyzer using AI to match skills with job requirements and provide optimization suggestions.</p>
                        <div class="tech-tags">
                            <span class="tech-tag">Streamlit</span>
                            <span class="tech-tag">NLP</span>
                            <span class="tech-tag">Skill Extraction</span>
                            <span class="tech-tag">Job Matching</span>
                        </div>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-icon">🎧</div>
                    <div class="project-content">
                        <h3>Podcast Generator</h3>
                        <p>Local AI podcast generator using Large Language Models to create engaging audio content with automated voice synthesis.</p>
                        <div class="tech-tags">
                            <span class="tech-tag">Python</span>
                            <span class="tech-tag">LLM</span>
                            <span class="tech-tag">Audio Generation</span>
                        </div>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-icon">📑</div>
                    <div class="project-content">
                        <h3>OCR Automated Toolkit</h3>
                        <p>Advanced OCR system with AI-powered Q&A chatbot for PDFs and images using Retrieval-Augmented Generation.</p>
                        <div class="tech-tags">
                            <span class="tech-tag">Tesseract</span>
                            <span class="tech-tag">Poppler</span>
                            <span class="tech-tag">ChromaDB</span>
                            <span class="tech-tag">RAG</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="section" style="background: rgba(0,0,0,0.2);">
        <div class="container">
            <h2 class="section-title">📫 Let's Connect</h2>
            <div class="contact-grid">
                <a href="mailto:shadabkhanbenki@gmail.com" class="contact-card">
                    <div class="contact-icon">📧</div>
                    <h3>Email</h3>
                    <p>shadabkhanbenki@gmail.com</p>
                </a>
                <a href="https://www.linkedin.com/in/shadab-khan-b-41b6a8270" target="_blank" class="contact-card">
                    <div class="contact-icon">💼</div>
                    <h3>LinkedIn</h3>
                    <p>Connect with me</p>
                </a>
                <a href="https://github.com/Bshadabkhan" target="_blank" class="contact-card">
                    <div class="contact-icon">💻</div>
                    <h3>GitHub</h3>
                    <p>View my projects</p>
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <section class="section" style="text-align: center; padding: 40px 20px;">
        <p style="font-size: 1.2rem;">⭐ Thanks for visiting! Feel free to explore and collaborate! ⭐</p>
    </section>

    <script>
        // Typing animation
        const texts = [
            "Python Developer 🐍",
            "AI & ML Engineer 🤖",
            "Full Stack Developer 💻",
            "Automation Expert ⚙️",
            "RAG Systems Builder 🔗"
        ];
        let textIndex = 0;
        let charIndex = 0;
        let isDeleting = false;
        const typingElement = document.getElementById('typing');

        function type() {
            const currentText = texts[textIndex];
            
            if (isDeleting) {
                typingElement.textContent = currentText.substring(0, charIndex - 1);
                charIndex--;
            } else {
                typingElement.textContent = currentText.substring(0, charIndex + 1);
                charIndex++;
            }

            if (!isDeleting && charIndex === currentText.length) {
                setTimeout(() => isDeleting = true, 2000);
            } else if (isDeleting && charIndex === 0) {
                isDeleting = false;
                textIndex = (textIndex + 1) % texts.length;
            }

            const speed = isDeleting ? 50 : 100;
            setTimeout(type, speed);
        }

        type();

        // Smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth' });
                }
            });
        });

        // Intersection Observer for animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -100px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animation = 'fadeInUp 1s ease forwards';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.about-card, .project-card, .skill-category, .contact-card').forEach(el => {
            observer.observe(el);
        });
    </script>
</body>
</html>
