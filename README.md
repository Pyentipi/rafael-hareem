[Uploading arafat.html…]()
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
    <title>Hareem Junior School - Nakasajja</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-green: #2E8B57;
            --light-green: #E8F5E9;
            --accent-green: #4CAF50;
            --white: #FFFFFF;
            --dark-text: #333333;
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: var(--dark-text);
            overflow-x: hidden;
            background-color: #f9f9f9;
        }

        img, video {
            max-width: 100%;
            height: auto;
            display: block;
        }

        /* Header Styles */
        header {
            background-color: var(--white);
            box-shadow: var(--shadow);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            transition: var(--transition);
        }

        header.scrolled {
            background-color: rgba(255, 255, 255, 0.95);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .header-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
        }

        .logo {
            display: flex;
            align-items: center;
            flex: 1 1 300px;
            transition: var(--transition);
        }

        .logo img {
            height: 60px;
            width: auto;
            margin-right: 15px;
            transition: var(--transition);
        }

        .logo-text h1 {
            margin: 0;
            font-size: 1.5rem;
            color: var(--primary-green);
            font-weight: 700;
        }

        .logo-text p {
            margin: 5px 0 0;
            font-size: 0.8rem;
            color: var(--dark-text);
        }

        nav {
            flex: 1 1 auto;
        }

        nav ul {
            display: flex;
            flex-wrap: wrap;
            list-style: none;
            justify-content: flex-end;
        }

        nav ul li {
            margin: 0 0 0 1.5rem;
        }

        nav ul li a {
            color: var(--dark-text);
            text-decoration: none;
            font-weight: 500;
            padding: 0.5rem 0;
            position: relative;
            transition: var(--transition);
            font-size: 0.95rem;
        }

        nav ul li a:after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            background: var(--accent-green);
            bottom: 0;
            left: 0;
            transition: var(--transition);
        }

        nav ul li a:hover:after {
            width: 100%;
        }

        nav ul li a:hover {
            color: var(--primary-green);
        }

        /* Hero Section */
        .hero {
            position: relative;
            height: 100vh;
            min-height: 600px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--white);
            overflow: hidden;
            margin-top: 80px;
        }

        .hero-video {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: -1;
        }

        .hero-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(46, 139, 87, 0.7);
            z-index: -1;
        }

        .hero-content {
            max-width: 800px;
            padding: 2rem;
            animation: fadeInUp 1s ease;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            font-weight: 700;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.2);
        }

        .btn {
            display: inline-block;
            background-color: var(--accent-green);
            color: var(--white);
            padding: 0.8rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: var(--transition);
            box-shadow: 0 4px 15px rgba(76, 175, 80, 0.4);
            border: 2px solid transparent;
        }

        .btn:hover {
            background-color: transparent;
            border-color: var(--white);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(76, 175, 80, 0.6);
        }

        .btn-secondary {
            background-color: transparent;
            border: 2px solid var(--white);
            margin-left: 1rem;
        }

        .btn-secondary:hover {
            background-color: var(--accent-green);
            border-color: var(--accent-green);
        }

        /* Section Styles */
        .section {
            padding: 5rem 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
        }

        .section-title h2 {
            font-size: 2.2rem;
            color: var(--primary-green);
            font-weight: 700;
            display: inline-block;
            margin-bottom: 1rem;
        }

        .section-title h2:after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background: var(--accent-green);
            margin: 0.5rem auto 0;
        }

        .section-title p {
            color: #666;
            max-width: 700px;
            margin: 0 auto;
        }

        /* About Section */
        .about {
            background-color: var(--white);
        }

        .about-content {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 3rem;
        }

        .about-text {
            flex: 1 1 50%;
        }

        .about-text p {
            margin-bottom: 1.5rem;
            color: #555;
        }

        .about-image {
            flex: 1 1 40%;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            position: relative;
        }

        .about-image img {
            transition: transform 0.5s ease;
            width: 100%;
        }

        .about-image:hover img {
            transform: scale(1.05);
        }

        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .feature-card {
            background: var(--white);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: var(--transition);
            text-align: center;
        }

        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }

        .feature-card i {
            font-size: 2.5rem;
            color: var(--primary-green);
            margin-bottom: 1.5rem;
        }

        .feature-card h3 {
            margin-bottom: 1rem;
            color: var(--primary-green);
        }

        /* Video Section */
        .video-section {
            background: linear-gradient(135deg, var(--light-green) 0%, var(--white) 100%);
            position: relative;
            overflow: hidden;
        }

        .video-container {
            max-width: 800px;
            margin: 0 auto;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
            position: relative;
        }

        .video-container video {
            width: 100%;
            display: block;
        }

        .video-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background: rgba(0, 0, 0, 0.3);
            color: white;
            opacity: 0;
            transition: var(--transition);
        }

        .video-container:hover .video-overlay {
            opacity: 1;
        }

        .video-overlay i {
            font-size: 3rem;
            margin-bottom: 1rem;
            color: var(--white);
        }

        .video-caption {
            max-width: 700px;
            margin: 2rem auto 0;
            text-align: center;
            color: #555;
        }

        /* Gallery Section */
        .gallery {
            background-color: var(--white);
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .gallery-item {
            position: relative;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            aspect-ratio: 4/3;
        }

        .gallery-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .gallery-item:hover img {
            transform: scale(1.1);
        }

        .gallery-caption {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(to top, rgba(46, 139, 87, 0.9), transparent);
            color: var(--white);
            padding: 1.5rem 1rem;
            transform: translateY(100%);
            transition: var(--transition);
        }

        .gallery-item:hover .gallery-caption {
            transform: translateY(0);
        }

        /* Testimonials */
        .testimonials {
            background: linear-gradient(135deg, var(--primary-green) 0%, var(--accent-green) 100%);
            color: var(--white);
            text-align: center;
        }

        .testimonials .section-title h2 {
            color: var(--white);
        }

        .testimonials .section-title h2:after {
            background: var(--white);
        }

        .testimonial-slider {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
        }

        .testimonial {
            padding: 2rem;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            margin: 0 1rem;
            backdrop-filter: blur(5px);
        }

        .testimonial-content {
            font-style: italic;
            margin-bottom: 1.5rem;
            position: relative;
        }

        .testimonial-content:before,
        .testimonial-content:after {
            content: '"';
            font-size: 3rem;
            color: rgba(255, 255, 255, 0.2);
            position: absolute;
        }

        .testimonial-content:before {
            top: -1rem;
            left: -1rem;
        }

        .testimonial-content:after {
            bottom: -2rem;
            right: -1rem;
        }

        .testimonial-author {
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .author-img {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            overflow: hidden;
            margin-right: 1rem;
            border: 3px solid rgba(255, 255, 255, 0.3);
        }

        .author-info h4 {
            margin-bottom: 0.2rem;
            font-weight: 600;
        }

        .author-info p {
            font-size: 0.9rem;
            opacity: 0.8;
        }

        /* Contact Section */
        .contact-info {
            background-color: var(--light-green);
        }

        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .contact-card {
            background-color: var(--white);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: var(--shadow);
            text-align: center;
            transition: var(--transition);
        }

        .contact-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }

        .contact-card i {
            font-size: 2.5rem;
            color: var(--primary-green);
            margin-bottom: 1.5rem;
        }

        .contact-card h3 {
            color: var(--primary-green);
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        .contact-form {
            max-width: 800px;
            margin: 3rem auto 0;
            background: var(--white);
            padding: 2rem;
            border-radius: 10px;
            box-shadow: var(--shadow);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
            color: var(--primary-green);
        }

        .form-control {
            width: 100%;
            padding: 0.8rem 1rem;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-family: inherit;
            transition: var(--transition);
        }

        .form-control:focus {
            outline: none;
            border-color: var(--accent-green);
            box-shadow: 0 0 0 3px rgba(76, 175, 80, 0.2);
        }

        textarea.form-control {
            min-height: 150px;
            resize: vertical;
        }

        .submit-btn {
            background-color: var(--accent-green);
            color: white;
            border: none;
            padding: 0.8rem 2rem;
            font-size: 1rem;
            border-radius: 50px;
            cursor: pointer;
            transition: var(--transition);
            display: inline-block;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(76, 175, 80, 0.4);
        }

        .submit-btn:hover {
            background-color: var(--primary-green);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(76, 175, 80, 0.6);
        }

        /* Footer */
        footer {
            background-color: var(--primary-green);
            color: var(--white);
            padding: 4rem 0 2rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .footer-col h3 {
            font-size: 1.3rem;
            margin-bottom: 1.5rem;
            position: relative;
            padding-bottom: 0.5rem;
        }

        .footer-col h3:after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 50px;
            height: 2px;
            background: var(--white);
        }

        .footer-col p {
            margin-bottom: 1rem;
            opacity: 0.9;
        }

        .footer-links li {
            margin-bottom: 0.8rem;
            list-style: none;
        }

        .footer-links a {
            color: var(--white);
            text-decoration: none;
            transition: var(--transition);
            opacity: 0.9;
        }

        .footer-links a:hover {
            opacity: 1;
            padding-left: 5px;
        }

        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 1.5rem;
        }

        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: var(--white);
            transition: var(--transition);
        }

        .social-links a:hover {
            background: var(--white);
            color: var(--primary-green);
            transform: translateY(-3px);
        }

        .footer-bottom {
            text-align: center;
            padding-top: 2rem;
            margin-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .animate {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease, transform 0.6s ease;
        }

        .animate.animated {
            opacity: 1;
            transform: translateY(0);
        }

        /* Responsive Styles */
        @media (max-width: 992px) {
            .hero h2 {
                font-size: 2.5rem;
            }
            
            .about-content {
                flex-direction: column;
            }
            
            .about-text, .about-image {
                flex: 1 1 100%;
            }
        }

        @media (max-width: 768px) {
            .header-container {
                padding: 1rem;
            }
            
            .hero {
                min-height: 500px;
                margin-top: 70px;
            }
            
            .hero h2 {
                font-size: 2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .section {
                padding: 3rem 0;
            }
            
            .section-title h2 {
                font-size: 1.8rem;
            }
            
            nav ul {
                justify-content: center;
                margin-top: 1rem;
            }
            
            nav ul li {
                margin: 0 0.5rem;
            }
            
            .btn {
                padding: 0.7rem 1.5rem;
                font-size: 0.9rem;
            }
        }

        @media (max-width: 576px) {
            .logo {
                flex-basis: 100%;
                justify-content: center;
                margin-bottom: 1rem;
            }
            
            .logo img {
                height: 50px;
            }
            
            .logo-text h1 {
                font-size: 1.3rem;
            }
            
            nav ul {
                width: 100%;
                justify-content: space-around;
            }
            
            nav ul li {
                margin: 0;
            }
            
            .hero {
                min-height: 400px;
            }
            
            .hero h2 {
                font-size: 1.8rem;
            }
            
            .btn-group {
                display: flex;
                flex-direction: column;
                gap: 1rem;
            }
            
            .btn {
                width: 100%;
                margin: 0 !important;
            }
            
            .gallery-grid {
                grid-template-columns: 1fr;
            }
            
            .footer-content {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header id="header">
        <div class="header-container">
            <div class="logo">
                <img src="school badge.jpg" alt="Hareem Junior School Logo">
                <div class="logo-text">
                    <h1>Hareem Junior School</h1>
                    <p>Nakasajja | Tel: +256 200947118</p>
                </div>
            </div>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#academics">Academics</a></li>
                    <li><a href="#gallery">Gallery</a></li>
                    <li><a href="#contact">Contact</a></li>
                    
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <video class="hero-video" autoplay loop muted playsinline>
            <source src="hero-video.mp4" type="video/mp4">
            <source src="hero-video.webm" type="video/webm">
            <!-- Fallback image if video doesn't load -->
            <img src="school-building.jpg" alt="Hareem Junior School">
        </video>
        <div class="hero-overlay"></div>
        <div class="hero-content">
            <h2>Inspiring Excellence Everyday</h2>
            <p>At Hareem Junior School Nakasajja, we nurture young minds to become responsible, creative, and successful individuals in our community.</p>
            <div class="btn-group">
                <a href="enrollment.html" class="btn">Enroll Now</a>
                <a href="#about" class="btn btn-secondary">Learn More</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="section about" id="about">
        <div class="container">
            <div class="section-title animate">
                <h2>About Our School</h2>
                <p>Discover what makes Hareem Junior School the perfect place for your child's education</p>
            </div>
            <div class="about-content">
                <div class="about-text animate">
                    <p>Founded in 2025 with a strong Islamic foundation, Hareem Junior School is committed to providing quality education that nurtures both academic excellence and moral values.</p>
                    <p>Located in the heart of Nakasajja, our school serves as a beacon of education and community development. We welcome children from all backgrounds and strive to make quality education accessible to all.</p>
                    <p>Our modern facilities, dedicated teachers, and holistic approach to education create an environment where every child can thrive and reach their full potential.</p>
                </div>
                <div class="about-image animate">
                    <img src="students in class.jpg" alt="Students at Hareem Junior School">
                </div>
            </div>
            <div class="features">
                <div class="feature-card animate">
                    <i class="fas fa-graduation-cap"></i>
                    <h3>Quality Education</h3>
                    <p>Our curriculum is designed to meet international standards while maintaining local relevance.</p>
                </div>
                <div class="feature-card animate">
                    <i class="fas fa-heart"></i>
                    <h3>Islamic Values</h3>
                    <p>We integrate Islamic principles with modern education for balanced development.</p>
                </div>
                <div class="feature-card animate">
                    <i class="fas fa-users"></i>
                    <h3>Experienced Staff</h3>
                    <p>Our qualified teachers are passionate about nurturing young minds.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Video Section -->
    <section class="section video-section">
        <div class="container">
            <div class="section-title animate">
                <h2>Our Happy Students</h2>
                <p>See our students in action and experience the vibrant life at Hareem Junior School</p>
            </div>
            <div class="video-container animate">
                <video autoplay loop muted playsinline>
                    <source src="sample vid.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                </video>
                <div class="video-overlay">
                    <i class="fas fa-play"></i>
                    <p>Watch our students at play</p>
                </div>
            </div>
            <div class="video-caption animate">
                <p>At Hareem Junior School, we believe in balanced development. Watch our students enjoying their playtime while developing social and physical skills that complement their academic growth.</p>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="section gallery" id="gallery">
        <div class="container">
            <div class="section-title animate">
                <h2>Our School Gallery</h2>
                <p>A glimpse into life at Hareem Junior School</p>
            </div>
            <div class="gallery-grid">
                <div class="gallery-item animate">
                    <img src="students in class.jpg" alt="Students learning in class">
                    <div class="gallery-caption">Interactive Classroom Learning</div>
                </div>
                <div class="gallery-item animate">
                    <img src="block 2.jpg" alt="School building">
                    <div class="gallery-caption">Our Modern Facilities</div>
                </div>
                <div class="gallery-item animate">
                    <img src="quaters.jpg" alt="School compound">
                    <div class="gallery-caption">Beautiful School Grounds</div>
                </div>
                <div class="gallery-item animate">
                    <img src="admin block.jpg" alt="Administration block">
                    <div class="gallery-caption">Administration Block</div>
                </div>
                <div class="gallery-item animate">
                    <img src="students in class.jpg" alt="Science lab">
                    <div class="gallery-caption">Science Laboratory</div>
                </div>
                <div class="gallery-item animate">
                    <img src="block 2.jpg" alt="Library">
                    <div class="gallery-caption">School Library</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="section testimonials">
        <div class="container">
            <div class="section-title animate">
                <h2>A word from our director</h2>
                <p>Hear from our satisfied parents and guardians</p>
            </div>
            <div class="testimonial-slider">
                <div class="testimonial animate">
                    <div class="testimonial-content">
                        "My child has shown remarkable improvement since joining Hareem Junior School. The teachers are caring and the Islamic values align perfectly with our family's principles."
                    </div>
                    <div class="testimonial-author">
                        <div class="author-img">
                            <img src="parent1.jpg" alt="Parent">
                        </div>
                        <div class="author-info">
                            <h4>Mr. Mahmood ssebunya</h4>
                            <p>Director</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="section contact-info" id="contact">
        <div class="container">
            <div class="section-title animate">
                <h2>Contact Us</h2>
                <p>We'd love to hear from you. Reach out for more information or to schedule a visit.</p>
            </div>
            <div class="contact-container">
                <div class="contact-card animate">
                    <i class="fas fa-map-marker-alt"></i>
                    <h3>Location</h3>
                    <p>Plot 42, Nakasajja Road<br>Nakasajja, Uganda</p>
                </div>
                <div class="contact-card animate">
                    <i class="fas fa-phone"></i>
                    <h3>Phone</h3>
                    <p>+256 200947118<br>+256 200947119</p>
                </div>
                <div class="contact-card animate">
                    <i class="fas fa-envelope"></i>
                    <h3>Email</h3>
                    <p>info@hareemjuniorschool.edu.ug<br>admissions@hareemjunior</p>
                    
                </div>
                  <div class="contact-card animate">
                    <i class="fab fa-whatsapp"></i>
                    <h3>whatsapp group</h3>
                    <p>info@hareemjuniorschool.edu.ug<br>admissions@hareemjunior</p>
            </div>
           <div class="contact-card animate">
                    <i class="fab fa-tiktok"></i>
                    <h3>whatsapp group</h3>
                    <p>info@hareemjuniorschool.edu.ug<br>admissions@hareemjunior</p>
            </div>
             <div class="contact-card animate">
                    <i class="fab fa-youtube"></i>
                    <h3>whatsapp group</h3>
                    <p>info@hareemjuniorschool.edu.ug<br>admissions@hareemjunior</p>
            </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-col animate">
                <h3>About Us</h3>
                <p>Hareem Junior School is a premier educational institution in Nakasajja, providing quality education grounded in Islamic values since 2025.</p>
                <div class="social-links">
                    <a href="#"><i class="fab fa-facebook-f"></i></a>
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-youtube"></i></a>
                    <a href="#"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>
            <div class="footer-col animate">
                <h3>Quick Links</h3>
                <ul class="footer-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#academics">Academics</a></li>
                    <li><a href="#gallery">Gallery</a></li>
                    <li><a href="#contact">Contact</a></li>
                    <li><a href="enrollment.html">Admissions</a></li>
                </ul>
            </div>
            <div class="footer-col animate">
                <h3>School Hours</h3>
                <ul class="footer-links">
                    <li>Monday - Friday: 7:30 AM - 5:00 PM</li>
                    <li>Saturday: 9:00 AM - 1:00 PM</li>
                    <li>Sunday: Closed</li>
                </ul>
                <h3 style="margin-top: 1.5rem;">Newsletter</h3>
                <form>
                    <div class="form-group">
                        <input type="email" class="form-control" placeholder="Your Email" required>
                    </div>
                    <button type="submit" class="submit-btn">Subscribe</button>
                </form>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2025 Hareem Junior School, Nakasajja. All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        // Header scroll effect
        window.addEventListener('scroll', function() {
            const header = document.getElementById('header');
            if (window.scrollY > 50) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });

        // Animation on scroll
        function animateOnScroll() {
            const elements = document.querySelectorAll('.animate');
            elements.forEach(element => {
                const elementPosition = element.getBoundingClientRect().top;
                const screenPosition = window.innerHeight / 1.2;
                
                if (elementPosition < screenPosition) {
                    element.classList.add('animated');
                }
            });
        }

        window.addEventListener('scroll', animateOnScroll);
        window.addEventListener('load', animateOnScroll);
    </script>
</body>
</html>
