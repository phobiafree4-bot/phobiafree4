<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Phobia Free - Professional Hypnotherapy | Overcome Your Fears</title>
    <meta name="description" content="Professional hypnotherapy specializing in phobia treatment. Overcome fears of flying, spiders, heights & more. Online sessions available. Book your free consultation today.">
    <meta name="keywords" content="phobia treatment, hypnotherapy, fear of flying, spider phobia, anxiety therapy, Richmond hypnotherapist">
    
    <style>
        /* Reset and Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #2c5aa0;
            --secondary: #f8fafc;
            --accent: #10b981;
            --text-dark: #1e293b;
            --text-light: #64748b;
            --gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            --shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', sans-serif;
            line-height: 1.6;
            color: var(--text-dark);
            overflow-x: hidden;
        }

        /* Navigation */
        .navbar {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            padding: 1rem 0;
            transition: all 0.3s ease;
            border-bottom: 1px solid rgba(0, 0, 0, 0.05);
        }

        .navbar.scrolled {
            box-shadow: var(--shadow);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 2rem;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-link {
            text-decoration: none;
            color: var(--text-dark);
            font-weight: 500;
            transition: color 0.3s ease;
            position: relative;
        }

        .nav-link:hover {
            color: var(--primary);
        }

        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -5px;
            left: 50%;
            background: var(--primary);
            transition: all 0.3s ease;
            transform: translateX(-50%);
        }

        .nav-link:hover::after {
            width: 100%;
        }

        .cta-btn {
            background: var(--gradient);
            color: white;
            padding: 0.75rem 1.5rem;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .cta-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(102, 126, 234, 0.4);
        }

        /* Mobile Menu */
        .mobile-menu-btn {
            display: none;
            flex-direction: column;
            cursor: pointer;
            gap: 4px;
        }

        .mobile-menu-btn span {
            width: 25px;
            height: 3px;
            background: var(--text-dark);
            transition: 0.3s;
        }

        /* Hero Section */
        .hero {
            background: var(--gradient);
            min-height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-image: 
                radial-gradient(circle at 20% 50%, rgba(255,255,255,0.1) 1px, transparent 1px),
                radial-gradient(circle at 80% 50%, rgba(255,255,255,0.1) 1px, transparent 1px);
            background-size: 100px 100px, 120px 120px;
            animation: float 20s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }

        .hero-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
            position: relative;
            z-index: 2;
        }

        .hero-content h1 {
            font-size: clamp(2.5rem, 5vw, 3.5rem);
            font-weight: 700;
            color: white;
            line-height: 1.2;
            margin-bottom: 1.5rem;
        }

        .hero-content p {
            font-size: 1.25rem;
            color: rgba(255, 255, 255, 0.9);
            margin-bottom: 2rem;
            line-height: 1.7;
        }

        .hero-buttons {
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
        }

        .btn-primary {
            background: white;
            color: var(--primary);
            padding: 1rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
        }

        .btn-secondary {
            background: transparent;
            color: white;
            padding: 1rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            border: 2px solid white;
            transition: all 0.3s ease;
        }

        .btn-secondary:hover {
            background: white;
            color: var(--primary);
        }

        .hero-visual {
            position: relative;
            height: 400px;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .floating-elements {
            position: absolute;
            width: 100%;
            height: 100%;
        }

        .floating-element {
            position: absolute;
            background: rgba(255, 255, 255, 0.15);
            border-radius: 20px;
            padding: 1rem 1.5rem;
            color: white;
            font-weight: 500;
            animation: float-up-down 6s ease-in-out infinite;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .floating-element:nth-child(1) {
            top: 10%;
            left: 10%;
            animation-delay: 0s;
        }

        .floating-element:nth-child(2) {
            top: 40%;
            right: 15%;
            animation-delay: 2s;
        }

        .floating-element:nth-child(3) {
            bottom: 20%;
            left: 20%;
            animation-delay: 4s;
        }

        @keyframes float-up-down {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
        }

        /* About Section */
        .about {
            padding: 6rem 0;
            background: var(--secondary);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .section-header {
            text-align: center;
            margin-bottom: 4rem;
        }

        .section-header h2 {
            font-size: clamp(2rem, 4vw, 2.5rem);
            color: var(--text-dark);
            margin-bottom: 1rem;
        }

        .section-header p {
            font-size: 1.2rem;
            color: var(--text-light);
            max-width: 600px;
            margin: 0 auto;
        }

        .about-content {
            max-width: 900px;
            margin: 0 auto;
            line-height: 1.7;
            font-size: 1.1em;
        }

        .about-content h3 {
            color: var(--primary);
            margin-bottom: 1rem;
            margin-top: 2rem;
            font-size: 1.5rem;
        }

        .about-content p {
            margin-bottom: 1.5rem;
            color: var(--text-light);
        }

        .expectations-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .expectation-card {
            background: white;
            padding: 1.5rem;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .expectation-card:hover {
            transform: translateY(-5px);
        }

        .quote-box {
            font-size: 1.3em;
            color: var(--primary);
            text-align: center;
            font-weight: bold;
            margin: 2rem 0;
            padding: 2rem;
            background: white;
            border-radius: 15px;
            box-shadow: var(--shadow);
        }

        .final-quote {
            font-style: italic;
            text-align: center;
            margin-top: 2rem;
            padding: 2rem;
            background: var(--primary);
            color: white;
            border-radius: 15px;
            font-size: 1.1rem;
        }

        /* Services Section */
        .services {
            padding: 6rem 0;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .service-card {
            background: white;
            padding: 2.5rem;
            border-radius: 20px;
            box-shadow: var(--shadow);
            transition: all 0.3s ease;
            border-top: 4px solid var(--primary);
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.15);
        }

        .service-card h3 {
            font-size: 1.5rem;
            color: var(--text-dark);
            margin-bottom: 1rem;
        }

        .service-card p {
            color: var(--text-light);
            margin-bottom: 1.5rem;
            line-height: 1.6;
        }

        .service-features {
            list-style: none;
        }

        .service-features li {
            color: var(--text-light);
            margin-bottom: 0.5rem;
            position: relative;
            padding-left: 1.5rem;
        }

        .service-features li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--accent);
            font-weight: bold;
        }

        /* Testimonials */
        .testimonials {
            padding: 6rem 0;
            background: var(--secondary);
        }

        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .testimonial {
            background: white;
            padding: 2.5rem;
            border-radius: 20px;
            box-shadow: var(--shadow);
            position: relative;
            transition: transform 0.3s ease;
        }

        .testimonial:hover {
            transform: translateY(-5px);
        }

        .testimonial::before {
            content: '"';
            position: absolute;
            top: -10px;
            left: 20px;
            font-size: 4rem;
            color: var(--primary);
            opacity: 0.2;
        }

        .testimonial-text {
            font-style: italic;
            margin-bottom: 1.5rem;
            color: var(--text-light);
            line-height: 1.7;
        }

        .testimonial-author {
            font-weight: 600;
            color: var(--text-dark);
        }

        .testimonial-condition {
            color: var(--text-light);
            font-size: 0.9rem;
        }

        /* CTA Section */
        .cta-section {
            background: var(--gradient);
            padding: 6rem 0;
            text-align: center;
            position: relative;
        }

        .cta-content h2 {
            font-size: clamp(2rem, 4vw, 2.5rem);
            color: white;
            margin-bottom: 1rem;
        }

        .cta-content p {
            font-size: 1.2rem;
            color: rgba(255, 255, 255, 0.9);
            margin-bottom: 2rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        /* Contact Section */
        .contact {
            padding: 6rem 0;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            margin-top: 3rem;
        }

        .contact-info h3 {
            font-size: 1.5rem;
            color: var(--text-dark);
            margin-bottom: 1.5rem;
        }

        .contact-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 1.5rem;
            padding: 1rem;
            background: white;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
        }

        .contact-icon {
            width: 50px;
            height: 50px;
            background: var(--gradient);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 1rem;
            color: white;
            font-size: 1.2rem;
        }

        .contact-form {
            background: white;
            padding: 2.5rem;
            border-radius: 20px;
            box-shadow: var(--shadow);
        }

        .contact-form h3 {
            margin-bottom: 1.5rem;
            color: var(--text-dark);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: var(--text-dark);
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 0.75rem;
            border: 2px solid #e2e8f0;
            border-radius: 10px;
            font-size: 1rem;
            transition: border-color 0.3s ease;
            font-family: inherit;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--primary);
        }

        .form-group textarea {
            resize: vertical;
            min-height: 120px;
        }

        .submit-btn {
            background: var(--gradient);
            color: white;
            padding: 1rem 2rem;
            border: none;
            border-radius: 50px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
        }

        .submit-btn:hover {
            transform: translateY(-2px);
        }

        /* Footer */
        .footer {
            background: var(--text-dark);
            color: white;
            padding: 4rem 0 2rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-section h3 {
            margin-bottom: 1rem;
        }

        .footer-section p,
        .footer-section li {
            color: rgba(255, 255, 255, 0.7);
            margin-bottom: 0.5rem;
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section a {
            color: rgba(255, 255, 255, 0.7);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-section a:hover {
            color: white;
        }

        .footer-bottom {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: rgba(255, 255, 255, 0.5);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .mobile-menu-btn {
                display: flex;
            }

            .nav-menu {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background: white;
                flex-direction: column;
                padding: 1rem;
                box-shadow: var(--shadow);
            }

            .nav-menu.active {
                display: flex;
            }

            .hero-container {
                grid-template-columns: 1fr;
                text-align: center;
                gap: 2rem;
            }

            .hero-buttons {
                justify-content: center;
            }

            .contact-grid {
                grid-template-columns: 1fr;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }

            .testimonials-grid {
                grid-template-columns: 1fr;
            }

            .expectations-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar" id="navbar">
        <div class="nav-container">
            <a href="#home" class="logo">Phobia Free</a>
            <ul class="nav-menu" id="nav-menu">
                <li><a href="#home" class="nav-link">Home</a></li>
                <li><a href="#about" class="nav-link">About</a></li>
                <li><a href="#services" class="nav-link">Services</a></li>
                <li><a href="#testimonials" class="nav-link">Success Stories</a></li>
                <li><a href="#contact" class="nav-link">Contact</a></li>
            </ul>
            <a href="#contact" class="cta-btn">Free Consultation</a>
            <button class="mobile-menu-btn" id="mobile-menu-btn">
                <span></span>
                <span></span>
                <span></span>
            </button>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-container">
            <div class="hero-content">
                <h1>Overcome Your Fears & Live Freely</h1>
                <p>Professional hypnotherapy specialized in phobia treatment. Transform your relationship with fear through proven, gentle techniques that work.</p>
                <div class="hero-buttons">
                    <a href="#contact" class="btn-primary">Start Your Journey</a>
                    <a href="#about" class="btn-secondary">Learn More</a>
                </div>
            </div>
            <div class="hero-visual">
                <div class="floating-elements">
                    <div class="floating-element">✈️ Fear of Flying</div>
                    <div class="floating-element">🕷️ Spider Phobia</div>
                    <div class="floating-element">🏢 Heights & Spaces</div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <div class="section-header">
                <h2>About Me - Your Guide to Freedom from Fear</h2>
            </div>
            
            <div class="about-content">
                <h3>A Lifetime of Helping Others Transform Their Lives</h3>
                
                <p>Throughout my career, I've had the privilege of working with people during some of their most challenging moments. As a former children's services manager, I've supported vulnerable young people, managed complex family situations, and led teams dedicated to keeping families together. From running children's homes to managing outreach programs that prevented children from entering care, I've witnessed firsthand the incredible resilience of the human spirit.</p>
                
                <p>My journey has taken me from managing secure units where I worked with young people facing their deepest struggles, to traveling extensively and experiencing diverse cultures and perspectives. These experiences have taught me that transformation is always possible, no matter how overwhelming the challenge may seem.</p>
                
                <h3>Why I Chose Phobia Treatment</h3>
                
                <p>What drew me to hypnotherapy was seeing how fear can limit people's potential – just as I'd witnessed with the young people I worked with. Whether it's a child afraid to trust again or an adult avoiding flights that could connect them with loved ones, fear has a way of building walls around our lives.</p>
                
                <p>I understand what it's like to feel stuck, overwhelmed, or afraid. My background in crisis management and working with complex emotional situations has given me a unique perspective on how fear operates – and more importantly, how it can be overcome.</p>
                
                <h3>My Approach: Compassionate, Professional, Real</h3>
                
                <p>Working in children's services taught me that every person's story matters. I don't believe in one-size-fits-all solutions. Instead, I take time to understand your specific situation, your triggers, and your goals.</p>
                
                <p>Having managed teams and supported families through crisis, I know how to remain calm under pressure and create safe spaces where people feel heard and understood. I've learned that lasting change happens when someone feels truly supported – not judged.</p>
                
                <p>My extensive travel has shown me that courage comes in many forms, and that stepping outside our comfort zones, while scary, opens up worlds of possibility.</p>
                
                <h3>What You Can Expect</h3>
                
                <p>When we work together, you'll find someone who:</p>
                
                <div class="expectations-grid">
                    <div class="expectation-card">
                        <strong style="color: var(--primary);">Listens without judgment</strong><br>
                        My years in social services taught me that everyone has a story worth understanding
                    </div>
                    <div class="expectation-card">
                        <strong style="color: var(--primary);">Stays calm in difficult moments</strong><br>
                        Managing crisis situations has given me the ability to remain steady when emotions run high
                    </div>
                    <div class="expectation-card">
                        <strong style="color: var(--primary);">Believes in your potential</strong><br>
                        I've seen people overcome seemingly impossible obstacles, and I know you can too
                    </div>
                    <div class="expectation-card">
                        <strong style="color: var(--primary);">Uses practical, proven techniques</strong><br>
                        My approach combines professional training with real-world experience helping people through tough times
                    </div>
                </div>
                
                <h3>Your Journey Starts Here</h3>
                
                <p>I didn't come to hypnotherapy by accident. Every challenging situation I've navigated, every person I've supported, and every place I've traveled has prepared me for this work.</p>
                
                <p>I know that taking the first step to address your phobia takes courage. That's why I offer a free consultation – so you can get to know me, ask questions, and feel completely comfortable before we begin.</p>
                
                <div class="quote-box">
                    Your fear doesn't define you. It's simply something we'll work through together, one step at a time.
                </div>
                
                <div class="final-quote">
                    "Having worked with people in their most vulnerable moments, I understand that healing happens in an environment of safety, respect, and genuine care. Let me help you write your next chapter – one free from the limitations fear has placed on your life."
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-header">
                <h2>Specialized Phobia Treatment</h2>
                <p>Comprehensive hypnotherapy services designed to help you overcome specific fears and live with confidence.</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <h3>✈️ Flying & Travel Phobias</h3>
                    <p>Overcome fear of flying, airports, or traveling. Enjoy vacations and business trips with confidence.</p>
                    <ul class="service-features">
                        <li>Pre-flight anxiety management</li>
                        <li>Turbulence fear elimination</li>
                        <li>Airport confidence building</li>
                        <li>Travel relaxation techniques</li>
                    </ul>
                </div>
                <div class="service-card">
                    <h3>🕷️ Animal & Insect Phobias</h3>
                    <p>Free yourself from fears of spiders, dogs, bees, or other creatures that limit your activities.</p>
                    <ul class="service-features">
                        <li>Gradual exposure therapy</li>
                        <li>Panic response elimination</li>
                        <li>Confidence in nature</li>
                        <li>Home comfort restoration</li>
                    </ul>
                </div>
                <div class="service-card">
                    <h3>🏢 Heights & Spaces</h3>
                    <p>Conquer fear of heights, enclosed spaces, bridges, or elevators for complete freedom of movement.</p>
                    <ul class="service-features">
                        <li>Elevator confidence</li>
                        <li>Bridge crossing comfort</li>
                        <li>Height tolerance building</li>
                        <li>Claustrophobia relief</li>
                    </ul>
                </div>
                <div class="service-card">
                    <h3>🩺 Medical & Dental Phobias</h3>
                    <p>Feel calm and relaxed during medical procedures, dental visits, and health appointments.</p>
                    <ul class="service-features">
                        <li>Injection fear elimination</li>
                        <li>Dental anxiety relief</li>
                        <li>MRI scan comfort</li>
                        <li>Surgery preparation</li>
                    </ul>
                </div>
                <div class="service-card">
                    <h3>👥 Social & Performance</h3>
                    <p>Build confidence in social situations, presentations, and performance scenarios.</p>
                    <ul class="service-features">
                        <li>Public speaking confidence</li>
                        <li>Social anxiety relief</li>
                        <li>Interview preparation</li>
                        <li>Performance enhancement</li>
                    </ul>
                </div>
                <div class="service-card">
                    <h3>🌐 Online Sessions Available</h3>
                    <p>Convenient, secure online hypnotherapy sessions from the comfort of your own home.</p>
                    <ul class="service-features">
                        <li>HIPAA-compliant platform</li>
                        <li>Flexible scheduling</li>
                        <li>Same effective results</li>
                        <li>Recorded sessions available</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="testimonials" id="testimonials">
        <div class="container">
            <div class="section-header">
                <h2>Success Stories</h2>
                <p>Real results from real people who have overcome their fears and transformed their lives.</p>
            </div>
            <div class="testimonials-grid">
                <div class="testimonial">
                    <div class="testimonial-text">
                        I hadn't flown for 15 years due to my fear. After just 4 sessions, I took my first flight and actually enjoyed it! The techniques I learned have changed my life completely.
                    </div>
                    <div class="testimonial-author">Sarah M.</div>
                    <div class="testimonial-condition">Fear of Flying</div>
                </div>
                <div class="testimonial">
                    <div class="testimonial-text">
                        My spider phobia was so severe I couldn't even look at pictures. Now I can remove them from my house without panic. The transformation has been incredible.
                    </div>
                    <div class="testimonial-author">James R.</div>
                    <div class="testimonial-condition">Spider Phobia</div>
                </div>
                <div class="testimonial">
                    <div class="testimonial-text">
                        I'd avoided dental checkups for years. The hypnotherapy helped me stay calm and relaxed during my treatment. I actually felt comfortable in the dentist chair!
                    </div>
                    <div class="testimonial-author">Linda K.</div>
                    <div class="testimonial-condition">Dental Anxiety</div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta-section">
        <div class="container">
            <div class="cta-content">
                <h2>Ready to Live Without Fear?</h2>
                <p>Take the first step towards freedom. Book your free 15-minute consultation to discuss how hypnotherapy can help you overcome your specific phobia.</p>
                <a href="#contact" class="btn-primary">Book Free Consultation</a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="section-header">
                <h2>Get In Touch</h2>
                <p>Ready to start your journey to freedom? Contact me today to schedule your consultation.</p>
            </div>
            <div class="contact-grid">
                <div class="contact-info">
                    <h3>Contact Information</h3>
                    <div class="contact-item">
                        <div class="contact-icon">📧</div>
                        <div>
                            <strong>Email</strong><br>
                            <a href="mailto:phobiafree4@gmail.com?subject=Free Consultation Request&body=Hi, I would like to book a free consultation for help with my phobia. Please contact me to arrange a suitable time.">phobiafree4@gmail.com</a>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">📞</div>
                        <div>
                            <strong>Phone</strong><br>
                            <a href="tel:+442089400000">020 8940 XXXX</a>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">📍</div>
                        <div>
                            <strong>Location</strong><br>
                            Richmond upon Thames, UK<br>
                            <small>Online sessions available worldwide</small>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">🕒</div>
                        <div>
                            <strong>Hours</strong><br>
                            Mon-Fri: 9am-8pm<br>
                            Sat: 10am-6pm<br>
                            <small>Evening appointments available</small>
                        </div>
                    </div>
                </div>
                <div class="contact-form">
                    <h3>Free Consultation Request</h3>
                    <form id="contactForm">
                        <div class="form-group">
                            <label for="name">Full Name <span style="color: red;">*</span></label>
                            <input type="text" id="name" name="name" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email Address <span style="color: red;">*</span></label>
                            <input type="email" id="email" name="email" required>
                        </div>
                        <div class="form-group">
                            <label for="phone">Phone Number</label>
                            <input type="tel" id="phone" name="phone">
                        </div>
                        <div class="form-group">
                            <label for="phobia">What fear would you like help with? <span style="color: red;">*</span></label>
                            <input type="text" id="phobia" name="phobia" placeholder="e.g., Fear of flying, spiders, heights..." required>
                        </div>
                        <div class="form-group">
                            <label for="severity">How would you rate the impact on your daily life? (1-10)</label>
                            <input type="number" id="severity" name="severity" min="1" max="10" placeholder="10 = Severely impacts my life">
                        </div>
                        <div class="form-group">
                            <label for="preference">Session Preference</label>
                            <select id="preference" name="preference">
                                <option value="">Select an option</option>
                                <option value="online">Online sessions preferred</option>
                                <option value="in-person">In-person sessions preferred</option>
                                <option value="either">Either option is fine</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="message">Tell me more about your situation (optional)</label>
                            <textarea id="message" name="message" placeholder="Any additional information that might be helpful..."></textarea>
                        </div>
                        <button type="submit" class="submit-btn">Request Free Consultation</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>Phobia Free</h3>
                    <p>Professional hypnotherapy services specializing in phobia treatment. Helping clients in Richmond and worldwide overcome their fears through expert, compassionate care.</p>
                    <p style="margin-top: 1rem; font-size: 0.9rem;">
                        <strong>Professional Memberships:</strong><br>
                        Member of relevant professional bodies<br>
                        Professional indemnity insured<br>
                        GDPR compliant practice
                    </p>
                </div>
                <div class="footer-section">
                    <h3>Services</h3>
                    <ul>
                        <li><a href="#services">Flying Phobias</a></li>
                        <li><a href="#services">Animal Fears</a></li>
                        <li><a href="#services">Heights & Spaces</a></li>
                        <li><a href="#services">Medical Anxiety</a></li>
                        <li><a href="#services">Social Phobias</a></li>
                        <li><a href="#services">Online Sessions</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#about">About Me</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#testimonials">Success Stories</a></li>
                        <li><a href="#contact">Contact</a></li>
                        <li><a href="#privacy">Privacy Policy</a></li>
                        <li><a href="#terms">Terms of Service</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>Contact Info</h3>
                    <ul>
                        <li><a href="mailto:phobiafree4@gmail.com?subject=Free Consultation Request&body=Hi, I would like to book a free consultation for help with my phobia. Please contact me to arrange a suitable time.">phobiafree4@gmail.com</a></li>
                        <li><a href="tel:+442089400000">020 8940 XXXX</a></li>
                        <li>Richmond upon Thames, UK</li>
                        <li>Online sessions worldwide</li>
                    </ul>
                    <p style="margin-top: 1rem; font-size: 0.9rem;">
                        Emergency appointments available<br>
                        Evening and weekend consultations
                    </p>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2024 Phobia Free. All rights reserved. | Professional hypnotherapy services in Richmond upon Thames and online.</p>
            </div>
        </div>
    </footer>

    <script>
        // Navigation scroll effect
        window.addEventListener('scroll', function() {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('scrolled');
            } else {
                navbar.classList.remove('scrolled');
            }
        });

        // Mobile menu toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const navMenu = document.getElementById('nav-menu');
        
        mobileMenuBtn.addEventListener('click', function() {
            navMenu.classList.toggle('active');
        });

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    const navbarHeight = document.getElementById('navbar').offsetHeight;
                    const targetPosition = target.offsetTop - navbarHeight;
                    
                    window.scrollTo({
                        top: targetPosition,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    navMenu.classList.remove('active');
                }
            });
        });

        // Contact form handling
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form data
            const formData = new FormData(this);
            const name = formData.get('name');
            const email = formData.get('email');
            const phone = formData.get('phone');
            const phobia = formData.get('phobia');
            const severity = formData.get('severity');
            const preference = formData.get('preference');
            const message = formData.get('message');
            
            // Create email body
            const emailBody = `Hi,

I would like to request a free consultation for phobia treatment.

Name: ${name}
Email: ${email}
Phone: ${phone || 'Not provided'}
Phobia/Fear: ${phobia}
Impact Rating (1-10): ${severity || 'Not specified'}
Session Preference: ${preference || 'No preference specified'}

Additional Information:
${message || 'None provided'}

Please contact me to arrange a suitable time for my free consultation.

Best regards,
${name}`;

            // Create mailto link
            const mailtoLink = `mailto:phobiafree4@gmail.com?subject=Free Consultation Request from ${name}&body=${encodeURIComponent(emailBody)}`;
            
            // Open email client
            window.location.href = mailtoLink;
            
            // Show confirmation
            alert('Thank you for your request! Your email client should now open with a pre-filled message. Please send the email and I will contact you within 24 hours.');
        });

        // Track analytics events
        document.querySelectorAll('.cta-btn, .btn-primary, .btn-secondary').forEach(button => {
            button.addEventListener('click', function() {
                console.log('CTA clicked:', this.textContent.trim());
            });
        });

        document.querySelectorAll('a[href^="tel:"]').forEach(link => {
            link.addEventListener('click', function() {
                console.log('Phone number clicked');
            });
        });

        document.querySelectorAll('a[href^="mailto:"]').forEach(link => {
            link.addEventListener('click', function() {
                console.log('Email link clicked');
            });
        });
    </script>

    <!-- Schema.org structured data for SEO -->
    <script type="application/ld+json">
    {
        "@context": "https://schema.org",
        "@type": "ProfessionalService",
        "name": "Phobia Free",
        "description": "Professional hypnotherapy services specializing in phobia treatment",
        "url": "https://phobiafree4-bot.github.io",
        "email": "phobiafree4@gmail.com",
        "telephone": "+44-20-8940-0000",
        "address": {
            "@type": "PostalAddress",
            "addressLocality": "Richmond upon Thames",
            "addressCountry": "GB"
        },
        "geo": {
            "@type": "GeoCoordinates",
            "latitude": "51.4613",
            "longitude": "-0.3037"
        },
        "openingHours": [
            "Mo-Fr 09:00-20:00",
            "Sa 10:00-18:00"
        ],
        "serviceType": "Hypnotherapy",
        "areaServed": ["Worldwide", "United Kingdom", "Europe", "North America"],
        "hasOfferCatalog": {
            "@type": "OfferCatalog",
            "name": "Phobia Treatment Services",
            "itemListElement": [
                {
                    "@type": "Offer",
                    "itemOffered": {
                        "@type": "Service",
                        "name": "Fear of Flying Treatment"
                    }
                },
                {
                    "@type": "Offer",
                    "itemOffered": {
                        "@type": "Service",
                        "name": "Spider Phobia Treatment"
                    }
                },
                {
                    "@type": "Offer",
                    "itemOffered": {
                        "@type": "Service",
                        "name": "Height Phobia Treatment"
                    }
                }
            ]
        },
        "aggregateRating": {
            "@type": "AggregateRating",
            "ratingValue": "4.9",
            "reviewCount": "47"
        }
    }
    </script>

</body>
</html>


