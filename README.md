<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aryan Saini - GitHub Profile</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0f0f23 0%, #1a1a2e 50%, #16213e 100%);
            color: #ffffff;
            min-height: 100vh;
            padding: 2rem;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .header {
            text-align: center;
            padding: 3rem 0;
            position: relative;
        }
        
        .glowing-text {
            font-size: 3.5rem;
            font-weight: 700;
            background: linear-gradient(45deg, #00bfff, #0080ff, #00bfff);
            background-size: 200% 200%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: gradient 3s ease infinite;
            margin-bottom: 1rem;
        }
        
        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .subtitle {
            font-size: 1.5rem;
            color: #a0a0c0;
            margin-bottom: 2rem;
        }
        
        .animated-gif {
            width: 300px;
            height: 200px;
            border-radius: 20px;
            margin: 2rem auto;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 191, 255, 0.3);
        }
        
        .stats {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin: 2rem 0;
            flex-wrap: wrap;
        }
        
        .stat-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 1rem 2rem;
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: transform 0.3s ease;
            text-align: center;
        }
        
        .stat-item:hover {
            transform: translateY(-5px);
        }
        
        .section {
            background: rgba(255, 255, 255, 0.05);
            margin: 2rem 0;
            padding: 2rem;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .section-title {
            font-size: 2rem;
            margin-bottom: 1.5rem;
            text-align: center;
            color: #00bfff;
        }
        
        .about-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }
        
        .about-item {
            background: rgba(255, 255, 255, 0.08);
            padding: 1.5rem;
            border-radius: 15px;
            border-left: 4px solid #00bfff;
        }
        
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            justify-content: center;
        }
        
        .tech-item {
            background: linear-gradient(45deg, #00bfff, #0080ff);
            padding: 0.8rem 1.5rem;
            border-radius: 25px;
            font-weight: 600;
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .tech-item:hover {
            transform: scale(1.1);
            box-shadow: 0 5px 15px rgba(0, 191, 255, 0.4);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1rem;
            flex-wrap: wrap;
        }
        
        .social-btn {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 1rem 2rem;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50px;
            text-decoration: none;
            color: white;
            font-weight: 600;
            transition: all 0.3s ease;
            border: 2px solid transparent;
        }
        
        .social-btn:hover {
            background: rgba(0, 191, 255, 0.2);
            border-color: #00bfff;
            transform: translateY(-3px);
        }
        
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        
        .stat-card {
            background: rgba(255, 255, 255, 0.05);
            padding: 1.5rem;
            border-radius: 15px;
            text-align: center;
            transition: transform 0.3s ease;
        }
        
        .stat-card:hover {
            transform: translateY(-5px);
        }
        
        .quote {
            text-align: center;
            font-style: italic;
            font-size: 1.2rem;
            color: #a0a0c0;
            margin: 2rem 0;
            padding: 2rem;
            border-left: 4px solid #00bfff;
            border-right: 4px solid #00bfff;
            background: rgba(0, 191, 255, 0.1);
            border-radius: 15px;
        }
        
        .github-stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        
        .github-stat {
            background: rgba(255, 255, 255, 0.05);
            padding: 1.5rem;
            border-radius: 15px;
            text-align: center;
        }
        
        .github-stat img {
            width: 100%;
            border-radius: 10px;
        }
        
        .loading {
            text-align: center;
            color: #00bfff;
            font-size: 1.2rem;
        }
        
        @media (max-width: 768px) {
            .glowing-text {
                font-size: 2.5rem;
            }
            
            .subtitle {
                font-size: 1.2rem;
            }
            
            .animated-gif {
                width: 250px;
                height: 150px;
            }
            
            .stats-container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header Section -->
        <div class="header">
            <h1 class="glowing-text">👋 Hello, I'm Aryan Saini</h1>
            <p class="subtitle">🚀 Passionate Application Developer from India 🇮🇳</p>
            
            <div class="animated-gif">
                <img src="https://i.gifer.com/JXA0.gif" alt="Coding Animation" style="width: 100%; height: 100%; object-fit: cover;">
            </div>
            
            <div class="stats">
                <div class="stat-item">
                    <strong>🎯 Focus Area</strong>
                    <div>Mobile & Web Apps</div>
                </div>
                <div class="stat-item">
                    <strong>💻 Status</strong>
                    <div>Coding Right Now</div>
                </div>
                <div class="stat-item">
                    <strong>🚀 Learning</strong>
                    <div>Flutter & Unity</div>
                </div>
            </div>
        </div>

        <!-- About Me Section -->
        <div class="section">
            <h2 class="section-title">💡 About Me</h2>
            <div class="about-grid">
                <div class="about-item">
                    <strong>🔭 Currently Working On</strong>
                    <p>Mobile & Web Applications with cutting-edge technologies</p>
                </div>
                <div class="about-item">
                    <strong>🌱 Currently Learning</strong>
                    <p>Advanced Flutter, Unity & Backend Development</p>
                </div>
                <div class="about-item">
                    <strong>💬 Ask Me About</strong>
                    <p>Android, Flutter, Unity, Firebase, or C#</p>
                </div>
                <div class="about-item">
                    <strong>📫 Reach Me At</strong>
                    <p>Freeestudio7@gmail.com</p>
                </div>
                <div class="about-item">
                    <strong>⚡ Fun Fact</strong>
                    <p>Coding is fun — until you meet that one stubborn bug 😅</p>
                </div>
            </div>
        </div>

        <!-- Tech Stack Section -->
        <div class="section">
            <h2 class="section-title">🛠️ Tech Stack</h2>
            <div class="tech-stack">
                <div class="tech-item">Android Studio</div>
                <div class="tech-item">Kotlin</div>
                <div class="tech-item">Java</div>
                <div class="tech-item">Dart</div>
                <div class="tech-item">Flutter</div>
                <div class="tech-item">Unity</div>
                <div class="tech-item">C#</div>
                <div class="tech-item">C++</div>
                <div class="tech-item">C</div>
                <div class="tech-item">HTML</div>
                <div class="tech-item">CSS</div>
                <div class="tech-item">Git</div>
                <div class="tech-item">Firebase</div>
            </div>
        </div>

        <!-- GitHub Analytics Section -->
        <div class="section">
            <h2 class="section-title">📊 GitHub Analytics</h2>
            <div class="github-stats">
                <div class="github-stat">
                    <h3>GitHub Stats</h3>
                    <img src="https://github-readme-stats.vercel.app/api?username=freestudio7&show_icons=true&theme=radical&hide_border=true&count_private=true" 
                         alt="GitHub Stats" onerror="this.style.display='none'">
                </div>
                <div class="github-stat">
                    <h3>Streak Stats</h3>
                    <img src="https://github-readme-streak-stats.herokuapp.com/?user=freestudio7&theme=radical&hide_border=true" 
                         alt="GitHub Streak" onerror="this.style.display='none'">
                </div>
                <div class="github-stat">
                    <h3>Top Languages</h3>
                    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=freestudio7&layout=compact&theme=radical&hide_border=true&langs_count=8" 
                         alt="Top Languages" onerror="this.style.display='none'">
                </div>
                <div class="github-stat">
                    <h3>Activity Graph</h3>
                    <img src="https://github-readme-activity-graph.vercel.app/graph?username=freestudio7&theme=react-dark&bg_color=1a1a2e&color=00bfff&line=00bfff&point=ffffff&area=true&hide_border=true" 
                         alt="Activity Graph" onerror="this.style.display='none'">
                </div>
            </div>
            
            <!-- Alternative GitHub Stats using GitHub API -->
            <div id="githubStats" class="stats-container" style="display: none;">
                <div class="stat-card">
                    <h3>📈 Repository Stats</h3>
                    <div id="repoCount" class="loading">Loading...</div>
                </div>
                <div class="stat-card">
                    <h3>⭐ Total Stars</h3>
                    <div id="totalStars" class="loading">Loading...</div>
                </div>
                <div class="stat-card">
                    <h3>📚 Languages Used</h3>
                    <div id="languages" class="loading">Loading...</div>
                </div>
            </div>
        </div>

        <!-- Connect Section -->
        <div class="section">
            <h2 class="section-title">🤝 Connect With Me</h2>
            <div class="social-links">
                <a href="mailto:Freeestudio7@gmail.com" class="social-btn">
                    📧 Gmail
                </a>
                <a href="https://linkedin.com/in/" class="social-btn">
                    💼 LinkedIn
                </a>
                <a href="https://twitter.com/" class="social-btn">
                    🐦 Twitter
                </a>
                <a href="https://www.instagram.com/" class="social-btn">
                    📷 Instagram
                </a>
            </div>
        </div>

        <!-- Quote Section -->
        <div class="quote">
            ✨ "Building ideas into apps — one line of code at a time." ✨
        </div>
    </div>

    <script>
        // GitHub API Integration for real-time stats
        async function fetchGitHubStats() {
            const username = 'freestudio7';
            
            try {
                // Fetch user data
                const userResponse = await fetch(`https://api.github.com/users/${username}`);
                const userData = await userResponse.json();
                
                // Fetch repositories
                const reposResponse = await fetch(`https://api.github.com/users/${username}/repos?per_page=100`);
                const reposData = await reposResponse.json();
                
                // Calculate stats
                const repoCount = reposData.length;
                const totalStars = reposData.reduce((acc, repo) => acc + repo.stargazers_count, 0);
                const totalForks = reposData.reduce((acc, repo) => acc + repo.forks_count, 0);
                
                // Get languages
                const languages = {};
                for (const repo of reposData) {
                    if (repo.language) {
                        languages[repo.language] = (languages[repo.language] || 0) + 1;
                    }
                }
                
                const topLanguages = Object.entries(languages)
                    .sort((a, b) => b[1] - a[1])
                    .slice(0, 5)
                    .map(([lang, count]) => `${lang}: ${count}`)
                    .join(', ');
                
                // Update DOM
                document.getElementById('repoCount').innerHTML = `
                    <div style="font-size: 2rem; color: #00bfff; margin: 0.5rem 0;">${repoCount}</div>
                    <div>Public Repositories</div>
                `;
                
                document.getElementById('totalStars').innerHTML = `
                    <div style="font-size: 2rem; color: #00bfff; margin: 0.5rem 0;">${totalStars}</div>
                    <div>Total Stars Earned</div>
                    <div style="margin-top: 0.5rem; font-size: 0.9rem; color: #a0a0c0;">Forks: ${totalForks}</div>
                `;
                
                document.getElementById('languages').innerHTML = `
                    <div style="font-size: 1.2rem; color: #00bfff; margin: 0.5rem 0;">${topLanguages}</div>
                    <div>Most Used Languages</div>
                `;
                
                // Show the stats container
                document.getElementById('githubStats').style.display = 'grid';
                
            } catch (error) {
                console.error('Error fetching GitHub data:', error);
                document.getElementById('repoCount').innerHTML = 'Failed to load';
                document.getElementById('totalStars').innerHTML = 'Failed to load';
                document.getElementById('languages').innerHTML = 'Failed to load';
            }
        }
        
        // Add interactive features
        document.addEventListener('DOMContentLoaded', function() {
            // Fetch GitHub stats
            fetchGitHubStats();
            
            // Add hover effects to tech stack items
            const techItems = document.querySelectorAll('.tech-item');
            techItems.forEach(item => {
                item.addEventListener('mouseenter', function() {
                    this.style.background = 'linear-gradient(45deg, #ff6b6b, #ffa500)';
                });
                item.addEventListener('mouseleave', function() {
                    this.style.background = 'linear-gradient(45deg, #00bfff, #0080ff)';
                });
            });
            
            // Animate sections on scroll
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };
            
            const observer = new IntersectionObserver(function(entries) {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, observerOptions);
            
            // Observe all sections for animation
            document.querySelectorAll('.section').forEach(section => {
                section.style.opacity = '0';
                section.style.transform = 'translateY(20px)';
                section.style.transition = 'all 0.6s ease';
                observer.observe(section);
            });
            
            // Add click effects to social buttons
            const socialBtns = document.querySelectorAll('.social-btn');
            socialBtns.forEach(btn => {
                btn.addEventListener('click', function(e) {
                    // Add ripple effect
                    const ripple = document.createElement('span');
                    const rect = this.getBoundingClientRect();
                    const size = Math.max(rect.width, rect.height);
                    const x = e.clientX - rect.left - size / 2;
                    const y = e.clientY - rect.top - size / 2;
                    
                    ripple.style.cssText = `
                        position: absolute;
                        border-radius: 50%;
                        background: rgba(255, 255, 255, 0.6);
                        transform: scale(0);
                        animation: ripple 0.6s linear;
                        width: ${size}px;
                        height: ${size}px;
                        left: ${x}px;
                        top: ${y}px;
                    `;
                    
                    this.style.position = 'relative';
                    this.style.overflow = 'hidden';
                    this.appendChild(ripple);
                    
                    setTimeout(() => {
                        ripple.remove();
                    }, 600);
                });
            });
        });
        
        // Add ripple animation
        const style = document.createElement('style');
        style.textContent = `
            @keyframes ripple {
                to {
                    transform: scale(4);
                    opacity: 0;
                }
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>
