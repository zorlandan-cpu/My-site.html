<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NBA Court Kings 2025 - Ultimate Basketball Game</title>
    <style>
        :root {
            --primary: #FF6B00;
            --secondary: #0057B8;
            --dark: #1A1A2E;
            --light: #F8F9FA;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, var(--dark) 0%, #16213E 100%);
            color: var(--light);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            background: rgba(26, 26, 46, 0.95);
            backdrop-filter: blur(10px);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.3);
        }
        
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
        }
        
        .logo img {
            height: 50px;
        }
        
        .nav-links {
            display: flex;
            gap: 30px;
            list-style: none;
        }
        
        .nav-links a {
            color: var(--light);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
            font-size: 1.1rem;
        }
        
        .nav-links a:hover {
            color: var(--primary);
        }
        
        .cta-button {
            background: var(--primary);
            color: white;
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            transition: transform 0.3s, box-shadow 0.3s;
            display: inline-block;
        }
        
        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(255, 107, 0, 0.3);
        }
        
        /* Hero Section */
        .hero {
            padding: 180px 0 100px;
            text-align: center;
            background: linear-gradient(rgba(26, 26, 46, 0.9), rgba(26, 26, 46, 0.9)),
                        url('https://images.unsplash.com/photo-1546519638-68e109498ffc?ixlib=rb-4.0.3&auto=format&fit=crop&w=2000&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }
        
        .hero h1 {
            font-size: 4rem;
            margin-bottom: 20px;
            background: linear-gradient(90deg, var(--primary), #FFD166);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
        }
        
        .hero p {
            font-size: 1.5rem;
            margin-bottom: 40px;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
            color: rgba(255, 255, 255, 0.9);
        }
        
        .store-badges {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 40px;
        }
        
        .store-badge {
            height: 60px;
            transition: transform 0.3s;
        }
        
        .store-badge:hover {
            transform: scale(1.05);
        }
        
        /* Features Section */
        .features {
            padding: 100px 0;
            background: rgba(22, 33, 62, 0.8);
        }
        
        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 60px;
            color: var(--primary);
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
            margin-top: 60px;
        }
        
        .feature-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px 30px;
            text-align: center;
            transition: transform 0.3s, background 0.3s;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            background: rgba(255, 107, 0, 0.1);
        }
        
        .feature-icon {
            font-size: 3rem;
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        .feature-card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }
        
        /* Screenshots Section */
        .screenshots {
            padding: 100px 0;
        }
        
        .screenshot-slider {
            display: flex;
            gap: 20px;
            overflow-x: auto;
            padding: 20px 0;
            scrollbar-width: thin;
            scrollbar-color: var(--primary) rgba(255, 255, 255, 0.1);
        }
        
        .screenshot-slider::-webkit-scrollbar {
            height: 8px;
        }
        
        .screenshot-slider::-webkit-scrollbar-track {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
        }
        
        .screenshot-slider::-webkit-scrollbar-thumb {
            background: var(--primary);
            border-radius: 10px;
        }
        
        .screenshot {
            flex: 0 0 auto;
            width: 300px;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s;
        }
        
        .screenshot:hover {
            transform: scale(1.05);
        }
        
        .screenshot img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        /* Download Section */
        .download {
            padding: 100px 0;
            text-align: center;
            background: linear-gradient(135deg, rgba(255, 107, 0, 0.1) 0%, rgba(0, 87, 184, 0.1) 100%);
        }
        
        .download h2 {
            font-size: 3rem;
            margin-bottom: 20px;
        }
        
        .download p {
            font-size: 1.2rem;
            margin-bottom: 40px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }
        
        /* Footer */
        footer {
            background: rgba(0, 0, 0, 0.5);
            padding: 80px 0 40px;
            margin-top: 100px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 60px;
        }
        
        .footer-column h3 {
            color: var(--primary);
            margin-bottom: 20px;
            font-size: 1.3rem;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: rgba(255, 255, 255, 0.7);
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: var(--primary);
        }
        
        .social-links {
            display: flex;
            gap: 20px;
            margin-top: 20px;
        }
        
        .social-icon {
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-decoration: none;
            transition: background 0.3s, transform 0.3s;
        }
        
        .social-icon:hover {
            background: var(--primary);
            transform: translateY(-3px);
        }
        
        .copyright {
            text-align: center;
            padding-top: 40px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: rgba(255, 255, 255, 0.5);
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                gap: 20px;
            }
            
            .nav-links {
                flex-wrap: wrap;
                justify-content: center;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero p {
                font-size: 1.2rem;
            }
            
            .store-badges {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav class="navbar">
                <div class="logo">
                    <i class="fas fa-basketball-ball"></i>
                    <span>NBA Court Kings</span>
                </div>
                <ul class="nav-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#features">Features</a></li>
                    <li><a href="#screenshots">Screenshots</a></li>
                    <li><a href="#download">Download</a></li>
                    <li><a href="#store">Store</a></li>
                    <li><a href="#support">Support</a></li>
                </ul>
                <a href="https://play.google.com/store/apps/details?id=com.yourcompany.nbacourtkings" class="cta-button">
                    <i class="fab fa-google-play"></i> PLAY NOW
                </a>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>NBA Court Kings 2025</h1>
            <p>Experience the ultimate 3D basketball simulation with real NBA players, stunning graphics, and intense gameplay. Build your dream team and dominate the court!</p>
            <a href="https://play.google.com/store/apps/details?id=com.yourcompany.nbacourtkings" class="cta-button" style="font-size: 1.2rem; padding: 15px 40px;">
                <i class="fab fa-google-play"></i> DOWNLOAD FREE
            </a>
            <div class="store-badges">
                <a href="https://play.google.com/store/apps/details?id=com.yourcompany.nbacourtkings">
                    <img src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png" alt="Get it on Google Play" class="store-badge">
                </a>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features" id="features">
        <div class="container">
            <h2 class="section-title">Game Features</h2>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-users"></i>
                    </div>
                    <h3>Real NBA Players</h3>
                    <p>450+ real NBA players with accurate stats, heights, ages, and signature moves</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-basketball-ball"></i>
                    </div>
                    <h3>3D Gameplay</h3>
                    <p>Stunning 3D graphics with realistic physics, animations, and court environments</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-shopping-cart"></i>
                    </div>
                    <h3>Player Store</h3>
                    <p>Buy, collect, and upgrade NBA players. Build your ultimate dream team</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-trophy"></i>
                    </div>
                    <h3>Multiple Modes</h3>
                    <p>Quick Play, Season Mode, Tournaments, Online Multiplayer & Career Mode</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <h3>Legendary Players</h3>
                    <p>Unlock basketball legends: Michael Jordan, Kobe Bryant, LeBron James & more</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-gamepad"></i>
                    </div>
                    <h3>Advanced Controls</h3>
                    <p>Dribble moves, crossovers, dunks, blocks, steals - complete control system</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Screenshots Section -->
    <section class="screenshots" id="screenshots">
        <div class="container">
            <h2 class="section-title">Screenshots</h2>
            <div class="screenshot-slider">
                <div class="screenshot">
                    <img src="https://images.unsplash.com/photo-1546519638-68e109498ffc?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" alt="Gameplay 1">
                </div>
                <div class="screenshot">
                    <img src="https://images.unsplash.com/photo-1519861531473-920034658307?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" alt="Gameplay 2">
                </div>
                <div class="screenshot">
                    <img src="https://images.unsplash.com/photo-1504450758481-7338eba7524a?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" alt="Gameplay 3">
                </div>
                <div class="screenshot">
                    <img src="https://images.unsplash.com/photo-1511895426328-dc8714191300?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" alt="Gameplay 4">
                </div>
                <div class="screenshot">
                    <img src="https://images.unsplash.com/photo-1542751371-adc38448a05e?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" alt="Gameplay 5">
                </div>
            </div>
        </div>
    </section>

    <!-- Download Section -->
    <section class="download" id="download">
        <div class="container">
            <h2>Ready to Play?</h2>
            <p>Download NBA Court Kings 2025 now for free and start building your basketball legacy!</p>
            <a href="https://play.google.com/store/apps/details?id=com.yourcompany.nbacourtkings" class="cta-button" style="font-size: 1.3rem; padding: 18px 50px;">
                <i class="fab fa-google-play"></i> DOWNLOAD NOW
            </a>
            <p style="margin-top: 20px; font-size: 0.9rem; opacity: 0.7;">
                Free to play • In-app purchases • 500MB download • Android 8.0+
            </p>
        </div>
    </section>

    <!-- Footer -->
    <footer id="support">
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>NBA Court Kings</h3>
                    <p>The ultimate mobile basketball experience with real NBA players and 3D gameplay.</p>
                    <div class="social-links">
                        <a href="https://twitter.com/NBACourtKings" class="social-icon">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="https://instagram.com/NBACourtKings" class="social-icon">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="https://facebook.com/NBACourtKings" class="social-icon">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="https://youtube.com/@NBACourtKings" class="social-icon">
                            <i class="fab fa-youtube"></i>
                        </a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul class="footer-links">
                        <li><a href="#home">Home</a></li>
                        <li><a href="#features">Features</a></li>
                        <li><a href="#screenshots">Screenshots</a></li>
                        <li><a href="#download">Download</a></li>
                        <li><a href="https://www.nbacourtkings.com/privacy">Privacy Policy</a></li>
                        <li><a href="https://www.nbacourtkings.com/terms">Terms of Service</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Support</h3>
                    <ul class="footer-links">
                        <li><a href="mailto:support@nbacourtkings.com">Contact Support</a></li>
                        <li><a href="https://www.nbacourtkings.com/faq">FAQ</a></li>
                        <li><a href="https://www.nbacourtkings.com/refunds">Refund Policy</a></li>
                        <li><a href="https://www.nbacourtkings.com/in-app-purchases">IAP Information</a></li>
                        <li><a href="https://www.nbacourtkings.com/community">Community</a></li>
                        <li><a href="https://www.nbacourtkings.com/updates">Update Notes</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Contact Us</h3>
                    <ul class="footer-links">
                        <li><i class="fas fa-envelope"></i> support@nbacourtkings.com</li>
                        <li><i class="fas fa-globe"></i> www.nbacourtkings.com</li>
                        <li><i class="fas fa-map-marker-alt"></i> Game Studio Inc.</li>
                        <li style="margin-top: 20px;">
                            <a href="https://play.google.com/store/apps/details?id=com.yourcompany.nbacourtkings" class="cta-button" style="padding: 8px 20px; font-size: 0.9rem;">
                                <i class="fab fa-google-play"></i> Rate Us
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2024 NBA Court Kings. All rights reserved. NBA is a registered trademark. This game is not affiliated with the NBA.</p>
                <p style="margin-top: 10px; font-size: 0.8rem;">
                    Player names and likenesses are used under license | Age Rating: 12+ | Contains in-app purchases
                </p>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Parallax effect for hero section
        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const hero = document.querySelector('.hero');
            hero.style.backgroundPositionY = scrolled * 0.5 + 'px';
        });

        // Auto-scroll screenshots
        const slider = document.querySelector('.screenshot-slider');
        let scrollAmount = 0;
        let scrollTimer;

        function autoScroll() {
            if(scrollAmount >= slider.scrollWidth - slider.clientWidth) {
                scrollAmount = 0;
            } else {
                scrollAmount += 300;
            }
            slider.scrollTo({
                left: scrollAmount,
                behavior: 'smooth'
            });
        }

        // Start auto-scroll
        scrollTimer = setInterval(autoScroll, 3000);

        // Pause auto-scroll on hover
        slider.addEventListener('mouseenter', () => {
            clearInterval(scrollTimer);
        });

        slider.addEventListener('mouseleave', () => {
            scrollTimer = setInterval(autoScroll, 3000);
        });
    </script>
</body>
</html># My-site.html
