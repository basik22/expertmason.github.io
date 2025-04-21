# expertmason.github.io<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Expert Mason - Professional Masonry Services</title>
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --text-color: #333;
            --white: #ffffff;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            color: var(--text-color);
            line-height: 1.6;
        }
        
        a {
            text-decoration: none;
            color: inherit;
        }
        
        h1, h2, h3 {
            margin-bottom: 15px;
            color: var(--primary-color);
        }
        
        ul {
            list-style: none;
        }
        
        /* Header */
        header {
            background-color: var(--primary-color);
            color: var(--white);
            padding: 1rem 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: relative;
        }
        
        .top-contact {
            background-color: var(--secondary-color);
            padding: 0.5rem 0;
            text-align: center;
            font-weight: bold;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .logo-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            display: flex;
            align-items: center;
            color: var(--white);
        }
        
        .logo span {
            color: var(--secondary-color);
        }
        
        .mobile-toggle {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        nav ul {
            display: flex;
        }
        
        nav ul li {
            padding: 0 15px;
        }
        
        nav ul li a {
            color: var(--white);
            font-weight: 500;
            transition: color 0.3s ease;
        }
        
        nav ul li a:hover {
            color: var(--secondary-color);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('/api/placeholder/1200/600') center/cover no-repeat;
            height: 80vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--white);
            position: relative;
        }
        
        .hero-content {
            max-width: 800px;
            padding: 0 20px;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            color: var(--white);
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 30px;
            background-color: var(--secondary-color);
            color: var(--white);
            border: none;
            border-radius: 5px;
            font-weight: bold;
            text-transform: uppercase;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        
        .btn:hover {
            background-color: #c0392b;
        }
        
        /* Services Section */
        .services {
            padding: 5rem 0;
            background-color: var(--light-color);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2.5rem;
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background-color: var(--white);
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
        }
        
        .service-icon {
            font-size: 2.5rem;
            color: var(--secondary-color);
            margin-bottom: 20px;
        }
        
        .service-title {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }
        
        /* About Section */
        .about {
            padding: 5rem 0;
        }
        
        .about-flex {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .about-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
        }
        
        .about-image img {
            width: 100%;
            display: block;
        }
        
        .about-content {
            flex: 1;
        }
        
        .about-title {
            font-size: 2.2rem;
            margin-bottom: 20px;
        }
        
        .about-text {
            margin-bottom: 25px;
        }
        
        /* Testimonials */
        .testimonials {
            padding: 5rem 0;
            background-color: var(--light-color);
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background-color: var(--white);
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .client-info {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .client-image {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            overflow: hidden;
            margin-right: 15px;
        }
        
        .client-image img {
            width: 100%;
        }
        
        .client-details h4 {
            margin-bottom: 5px;
        }
        
        .star-rating {
            color: #f1c40f;
            margin-bottom: 15px;
        }
        
        /* CTA Section */
        .cta {
            padding: 5rem 0;
            background: linear-gradient(rgba(0,0,0,0.8), rgba(0,0,0,0.8)), url('/api/placeholder/1200/400') center/cover no-repeat;
            color: var(--white);
            text-align: center;
        }
        
        .cta-title {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: var(--white);
        }
        
        .cta-text {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        /* Contact */
        .contact {
            padding: 5rem 0;
        }
        
        .contact-flex {
            display: flex;
            gap: 50px;
        }
        
        .contact-form {
            flex: 1;
        }
        
        .contact-info {
            flex: 1;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-control {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        
        textarea.form-control {
            height: 150px;
            resize: none;
        }
        
        .contact-method {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .contact-icon {
            font-size: 1.5rem;
            background-color: var(--secondary-color);
            color: var(--white);
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: var(--white);
            padding: 3rem 0;
        }
        
        .footer-flex {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 30px;
        }
        
        .footer-col {
            flex: 1;
            min-width: 250px;
        }
        
        .footer-title {
            color: var(--white);
            margin-bottom: 20px;
            font-size: 1.3rem;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a:hover {
            color: var(--secondary-color);
        }
        
        .social-links {
            display: flex;
            gap: 15px;
        }
        
        .social-icon {
            width: 40px;
            height: 40px;
            background-color: rgba(255,255,255,0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: background-color 0.3s ease;
        }
        
        .social-icon:hover {
            background-color: var(--secondary-color);
        }
        
        .copyright {
            text-align: center;
            padding-top: 30px;
            margin-top: 30px;
            border-top: 1px solid rgba(255,255,255,0.1);
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .mobile-toggle {
                display: block;
            }
            
            nav {
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background-color: var(--primary-color);
                display: none;
                padding: 20px 0;
                box-shadow: 0 5px 10px rgba(0,0,0,0.1);
                z-index: 100;
            }
            
            nav.active {
                display: block;
            }
            
            nav ul {
                flex-direction: column;
            }
            
            nav ul li {
                padding: 10px 0;
                text-align: center;
            }
            
            .about-flex, .contact-flex {
                flex-direction: column;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Top Contact Info -->
    <div class="top-contact">
        <div class="container">
            Call Now: 07920079349 | Free Estimates
        </div>
    </div>
    
    <!-- Header -->
    <header>
        <div class="container">
            <div class="logo-container">
                <a href="#" class="logo"><span>Expert</span> Mason</a>
                <div class="mobile-toggle">☰</div>
                <nav>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#about">About</a></li>
                        <li><a href="#testimonials">Testimonials</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
    
    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>Professional Masonry Services of the Highest Quality</h1>
            <p>We offer comprehensive building and masonry services across the country. We guarantee reliability, timeliness, and competitive pricing.</p>
            <a href="#contact" class="btn">Free Estimate</a>
        </div>
    </section>
    
    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <h2 class="section-title">Our Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">🏗️</div>
                    <h3 class="service-title">Wall Construction</h3>
                    <p>We specialize in building walls with various materials, ensuring precision and durability in every project.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🧱</div>
                    <h3 class="service-title">Renovation Work</h3>
                    <p>We offer professional renovation services, including repair and restoration of masonry, plastering, and much more.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🏠</div>
                    <h3 class="service-title">Foundation Building</h3>
                    <p>We construct solid foundations that serve as the basis for every durable building structure.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🪨</div>
                    <h3 class="service-title">Facades</h3>
                    <p>We design and create aesthetic facades that not only look beautiful but are also durable and functional.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🏛️</div>
                    <h3 class="service-title">Decorative Architecture</h3>
                    <p>We create decorative architectural elements that give buildings character and unique appearance.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🔧</div>
                    <h3 class="service-title">Technical Consulting</h3>
                    <p>We offer professional advice on construction technologies and masonry materials.</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <div class="about-flex">
                <div class="about-image">
                    <img src="/api/placeholder/600/400" alt="Our team at work">
                </div>
                <div class="about-content">
                    <h2 class="about-title">About Our Company</h2>
                    <p class="about-text">With over 15 years of experience in the construction industry, we are experts in all types of masonry work. Our company was founded with a passion for solid construction and a pursuit of perfection in every detail.</p>
                    <p class="about-text">Our team consists of highly qualified specialists who regularly enhance their skills to deliver services of the highest standard. We use only the best quality materials, which translates into the durability and reliability of our projects.</p>
                    <p class="about-text">Customer satisfaction is our priority, which is why we treat each project individually, adapting to specific needs and expectations.</p>
                    <a href="#contact" class="btn">Contact Us</a>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Testimonials -->
    <section class="testimonials" id="testimonials">
        <div class="container">
            <h2 class="section-title">What Our Clients Say</h2>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <div class="client-info">
                        <div class="client-image">
                            <img src="/api/placeholder/100/100" alt="Client">
                        </div>
                        <div class="client-details">
                            <h4>John Smith</h4>
                            <p>London</p>
                        </div>
                    </div>
                    <div class="star-rating">★★★★★</div>
                    <p>"I am extremely satisfied with Expert Mason's services. They performed a comprehensive renovation of my house that exceeded my expectations. Professionalism, timeliness, and quality at the highest level!"</p>
                </div>
                <div class="testimonial-card">
                    <div class="client-info">
                        <div class="client-image">
                            <img src="/api/placeholder/100/100" alt="Client">
                        </div>
                        <div class="client-details">
                            <h4>Sarah Johnson</h4>
                            <p>Manchester</p>
                        </div>
                    </div>
                    <div class="star-rating">★★★★★</div>
                    <p>"The construction of my dream home was in good hands. Expert Mason is a team of true professionals who can advise and perform any task with precision. I recommend them to everyone!"</p>
                </div>
                <div class="testimonial-card">
                    <div class="client-info">
                        <div class="client-image">
                            <img src="/api/placeholder/100/100" alt="Client">
                        </div>
                        <div class="client-details">
                            <h4>Peter Williams</h4>
                            <p>Birmingham</p>
                        </div>
                    </div>
                    <div class="star-rating">★★★★★</div>
                    <p>"Working with Expert Mason was a pure pleasure. The company renovated an old building for me, preserving its historical character. The result exceeded my wildest expectations!"</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- CTA Section -->
    <section class="cta">
        <div class="container">
            <h2 class="cta-title">Ready to Start Your Project?</h2>
            <p class="cta-text">Contact us today to receive a free estimate and consultation. Our experts are ready to help you realize your construction dreams.</p>
            <a href="#contact" class="btn">Contact Us Now</a>
        </div>
    </section>
    
    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <h2 class="section-title">Contact Us</h2>
            <div class="contact-flex">
                <div class="contact-form">
                    <form>
                        <div class="form-group">
                            <input type="text" class="form-control" placeholder="Full Name" required>
                        </div>
                        <div class="form-group">
                            <input type="email" class="form-control" placeholder="Email" required>
                        </div>
                        <div class="form-group">
                            <input type="tel" class="form-control" placeholder="Phone">
                        </div>
                        <div class="form-group">
                            <textarea class="form-control" placeholder="Message" required></textarea>
                        </div>
                        <button type="submit" class="btn">Send Message</button>
                    </form>
                </div>
                <div class="contact-info">
                    <div class="contact-method">
                        <div class="contact-icon">📱</div>
                        <div>
                            <h4>Phone</h4>
                            <p>07920079349</p>
                        </div>
                    </div>
                    <div class="contact-method">
                        <div class="contact-icon">✉️</div>
                        <div>
                            <h4>Email</h4>
                            <p>chrisservice35.gmail.com</p>
                        </div>
                    </div>
                    <div class="contact-method">
                        <div class="contact-icon">🏢</div>
                        <div>
                            <h4>Address</h4>
                            <p>HA29HA Harrow</p>
                        </div>
                    </div>
                    <div class="contact-method">
                        <div class="contact-icon">⏰</div>
                        <div>
                            <h4>Working Hours</h4>
                            <p>Monday - Friday: 8:00 - 18:00<br>Saturday: 9:00 - 14:00</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-flex">
                <div class="footer-col">
                    <h3 class="footer-title">Expert Mason</h3>
                    <p>Professional masonry services for individual clients and businesses. We operate throughout the UK, ensuring the highest quality of work.</p>
                    <div class="social-links">
                        <a href="#" class="social-icon">f</a>
                        <a href="#" class="social-icon">in</a>
                        <a href="#" class="social-icon">ig</a>
                    </div>
                </div>
                <div class="footer-col">
                    <h3 class="footer-title">Quick Links</h3>
                    <ul class="footer-links">
                        <li><a href="#">Home</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#about">About</a></li>
                        <li><a href="#testimonials">Testimonials</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3 class="footer-title">Areas Served</h3>
                    <ul class="footer-links">
                        <li>Harrow</li>
                        <li>London</li>
                        <li>Birmingham</li>
                        <li>Manchester</li>
                        <li>Liverpool</li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2025 Expert Mason. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const mobileToggle = document.querySelector('.mobile-toggle');
        const nav = document.querySelector('nav');
        
        mobileToggle.addEventListener('click', () => {
            nav.classList.toggle('active');
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    window.scrollTo({
                        top: target.offsetTop - 100,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    if (nav.classList.contains('active')) {
                        nav.classList.remove('active');
                    }
                }
            });
        });
    </script>
</body>
</html>
