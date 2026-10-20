<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta name="description" content="BM Public School - Inspiring young minds through quality education, creativity and innovation.">
    <title>BM Public School | Learn. Grow. Succeed.</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        :root {
            --primary: #123c69;
            --secondary: #f5a623;
            --light: #f5f8fc;
            --dark: #172b4d;
            --text: #637083;
        }

        body {
            font-family: 'Poppins', sans-serif;
            color: var(--dark);
            background: #fff;
            line-height: 1.7;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        button, input, textarea {
            font-family: inherit;
        }

        .container {
            width: min(1150px, 90%);
            margin: auto;
        }

        /* TOP BAR */

        .topbar {
            background: var(--primary);
            color: white;
            padding: 9px 0;
            font-size: 12px;
        }

        .topbar .container {
            display: flex;
            justify-content: space-between;
            gap: 15px;
            flex-wrap: wrap;
        }

        /* NAVIGATION */

        header {
            background: white;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 3px 20px #102d4b0d;
        }

        nav {
            min-height: 82px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 20px;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo-icon {
            width: 49px;
            height: 49px;
            border-radius: 14px;
            background: var(--primary);
            color: white;
            display: grid;
            place-items: center;
            font-size: 18px;
            font-weight: 800;
        }

        .logo h2 {
            font-size: 19px;
            line-height: 1.3;
            color: var(--primary);
        }

        .logo span {
            font-size: 10px;
            letter-spacing: 2px;
            color: var(--text);
        }

        .nav-links {
            display: flex;
            align-items: center;
            gap: 27px;
            list-style: none;
        }

        .nav-links a {
            font-size: 13px;
            font-weight: 500;
            transition: .3s;
        }

        .nav-links a:hover {
            color: #f0a020;
        }

        .nav-cta {
            background: var(--secondary);
            color: #172b4d !important;
            padding: 12px 20px;
            border-radius: 8px;
            font-weight: 700 !important;
        }

        .menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 27px;
            cursor: pointer;
        }

        /* HERO */

        .hero {
            min-height: 590px;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
            color: white;
            background:
                linear-gradient(90deg, #102d52 0%, #102d52ed 45%, #102d5270 100%),
                url('https://images.unsplash.com/photo-1503676260728-1c00da094a0b?auto=format&fit=crop&w=1800&q=85')
                center/cover;
        }

        .hero-content {
            max-width: 690px;
            padding: 90px 0;
            animation: appear 1s ease;
        }

        .eyebrow {
            display: inline-block;
            padding: 7px 15px;
            border: 1px solid #ffffff50;
            border-radius: 30px;
            font-size: 12px;
            margin-bottom: 22px;
            color: #ffcb73;
        }

        .hero h1 {
            font-size: clamp(38px, 5vw, 66px);
            line-height: 1.15;
            letter-spacing: -2px;
            margin-bottom: 24px;
        }

        .hero h1 span {
            color: var(--secondary);
        }

        .hero p {
            max-width: 560px;
            font-size: 15px;
            color: #e0e8f4;
            margin-bottom: 32px;
        }

        .btn {
            display: inline-block;
            padding: 14px 24px;
            border-radius: 8px;
            font-size: 13px;
            font-weight: 700;
            transition: .3s;
            border: none;
            cursor: pointer;
        }

        .btn-primary {
            background: var(--secondary);
            color: #172b4d;
        }

        .btn-outline {
            color: white;
            border: 1px solid #ffffff70;
            margin-left: 10px;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px #0002;
        }

        /* STATS */

        .stats {
            position: relative;
            margin-top: -45px;
            z-index: 2;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            background: white;
            border-radius: 15px;
            padding: 30px 15px;
            box-shadow: 0 15px 50px #18365a12;
        }

        .stat {
            text-align: center;
            padding: 10px;
            border-right: 1px solid #e9edf4;
        }

        .stat:last-child {
            border: none;
        }

        .stat h2 {
            color: var(--primary);
            font-size: 32px;
        }

        .stat p {
            font-size: 12px;
            color: var(--text);
        }

        /* COMMON SECTIONS */

        section {
            scroll-margin-top: 90px;
        }

        .section {
            padding: 100px 0;
        }

        .section-heading {
            text-align: center;
            max-width: 650px;
            margin: 0 auto 50px;
        }

        .section-heading span,
        .mini-title {
            color: #d88c10;
            text-transform: uppercase;
            font-weight: 700;
            letter-spacing: 2px;
            font-size: 11px;
        }

        .section-heading h2 {
            font-size: clamp(28px, 4vw, 40px);
            line-height: 1.3;
            margin: 12px 0;
        }

        .section-heading p {
            font-size: 14px;
            color: var(--text);
        }

        /* ABOUT */

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            align-items: center;
            gap: 65px;
        }

        .about-image {
            position: relative;
        }

        .about-image img {
            width: 100%;
            height: 420px;
            object-fit: cover;
            border-radius: 18px;
        }

        .image-label {
            position: absolute;
            bottom: 20px;
            left: -18px;
            background: var(--secondary);
            padding: 20px;
            border-radius: 12px;
            font-size: 13px;
            font-weight: 700;
            box-shadow: 0 10px 25px #0002;
        }

        .about-text h2 {
            font-size: 36px;
            line-height: 1.3;
            margin: 12px 0 20px;
        }

        .about-text p {
            color: var(--text);
            font-size: 14px;
            margin-bottom: 16px;
        }

        .check-list {
            list-style: none;
            margin: 25px 0;
        }

        .check-list li {
            margin: 12px 0;
            font-size: 13px;
            font-weight: 500;
        }

        .check-list li::before {
            content: "✓";
            display: inline-grid;
            place-items: center;
            width: 23px;
            height: 23px;
            border-radius: 50%;
            color: #13734a;
            background: #dcf7e9;
            margin-right: 10px;
        }

        /* PROGRAMS */

        .programs {
            background: var(--light);
        }

        .program-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 24px;
        }

        .program-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            transition: .3s;
            border: 1px solid #e9edf4;
        }

        .program-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 40px #19385812;
        }

        .program-card img {
            width: 100%;
            height: 210px;
            object-fit: cover;
            display: block;
        }

        .program-content {
            padding: 25px;
        }

        .program-content .number {
            color: #d88c10;
            font-size: 11px;
            font-weight: 700;
        }

        .program-content h3 {
            font-size: 20px;
            margin: 6px 0 10px;
        }

        .program-content p {
            color: var(--text);
            font-size: 13px;
            margin-bottom: 18px;
        }

        .text-link {
            color: var(--primary);
            font-size: 13px;
            font-weight: 700;
        }

        /* FACILITIES */

        .facility-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .facility {
            padding: 28px;
            border: 1px solid #e9edf4;
            border-radius: 13px;
            transition: .3s;
        }

        .facility:hover {
            border-color: #f5a623;
            background: #fffaf0;
            transform: translateY(-4px);
        }

        .facility-icon {
            width: 54px;
            height: 54px;
            border-radius: 13px;
            background: #eaf1fc;
            display: grid;
            place-items: center;
            font-size: 25px;
            margin-bottom: 20px;
        }

        .facility h3 {
            font-size: 17px;
            margin-bottom: 8px;
        }

        .facility p {
            color: var(--text);
            font-size: 13px;
        }

        /* ADMISSION CTA */

        .admission {
            background: linear-gradient(110deg, #123c69, #1c568d);
            color: white;
            padding: 65px 0;
        }

        .admission-inner {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 25px;
        }

        .admission h2 {
            font-size: clamp(26px, 4vw, 38px);
            line-height: 1.3;
            margin: 10px 0;
        }

        .admission p {
            font-size: 13px;
            color: #dbe8f7;
        }

        /* CONTACT */

        .contact-grid {
            display: grid;
            grid-template-columns: .8fr 1.2fr;
            gap: 50px;
        }

        .contact-info h2 {
            font-size: 34px;
            line-height: 1.3;
            margin: 12px 0 20px;
        }

        .contact-info > p {
            color: var(--text);
            font-size: 14px;
            margin-bottom: 25px;
        }

        .contact-item {
            margin: 20px 0;
            font-size: 13px;
        }

        .contact-item strong {
            display: block;
            color: var(--primary);
            margin-bottom: 4px;
        }

        .contact-form {
            background: var(--light);
            padding: 32px;
            border-radius: 15px;
        }

        .contact-form h3 {
            margin-bottom: 20px;
            font-size: 21px;
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }

        .contact-form input,
        .contact-form select,
        .contact-form textarea {
            width: 100%;
            padding: 13px;
            border: 1px solid #dfe5ee;
            border-radius: 7px;
            outline: none;
            margin-bottom: 15px;
            background: white;
            font-size: 12px;
        }

        .contact-form input:focus,
        .contact-form select:focus,
        .contact-form textarea:focus {
            border-color: var(--primary);
        }

        .contact-form textarea {
            min-height: 110px;
            resize: vertical;
        }

        .contact-form .btn {
            width: 100%;
        }

        #form-message {
            font-size: 12px;
            color: #13734a;
            margin-top: 12px;
        }

        /* FOOTER */

        footer {
            background: #0d2440;
            color: white;
            padding: 55px 0 20px;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: 1.4fr 1fr 1fr;
            gap: 40px;
            padding-bottom: 35px;
        }

        .footer-about p {
            font-size: 12px;
            color: #bdc9d8;
            max-width: 320px;
            margin-top: 18px;
        }

        footer h3 {
            font-size: 15px;
            margin-bottom: 17px;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin: 9px 0;
            font-size: 12px;
            color: #bdc9d8;
        }

        .footer-links a:hover {
            color: var(--secondary);
        }

        .copyright {
            border-top: 1px solid #ffffff20;
            padding-top: 20px;
            text-align: center;
            font-size: 11px;
            color: #bdc9d8;
        }

        /* ANIMATION */

        @keyframes appear {
            from {
                opacity: 0;
                transform: translateY(25px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* RESPONSIVE DESIGN */

        @media (max-width: 900px) {
            .nav-links {
                gap: 15px;
            }

            .nav-links a {
                font-size: 11px;
            }

            .about-grid {
                gap: 35px;
            }

            .program-grid,
            .facility-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 700px) {
            .topbar .container {
                justify-content: center;
                text-align: center;
            }

            nav {
                min-height: 72px;
            }

            .menu-btn {
                display: block;
            }

            .nav-links {
                display: none;
                position: absolute;
                top: 72px;
                left: 0;
                width: 100%;
                background: white;
                padding: 20px 5%;
                flex-direction: column;
                align-items: stretch;
                gap: 0;
                box-shadow: 0 10px 15px #0001;
            }

            .nav-links.active {
                display: flex;
            }

            .nav-links li a {
                display: block;
                padding: 12px 0;
                font-size: 13px;
            }

            .nav-links .nav-cta {
                text-align: center;
                padding: 12px;
                margin-top: 10px;
            }

            .hero {
                min-height: 520px;
                background-position: center;
            }

            .hero-content {
                padding: 70px 0;
            }

            .hero h1 {
                letter-spacing: -1px;
            }

            .btn {
                padding: 12px 16px;
            }

            .stats-grid {
                grid-template-columns: repeat(2, 1fr);
                padding: 15px;
            }

            .stat:nth-child(2) {
                border-right: none;
            }

            .stat:nth-child(-n+2) {
                border-bottom: 1px solid #e9edf4;
            }

            .section {
                padding: 70px 0;
            }

            .about-grid,
            .contact-grid {
                grid-template-columns: 1fr;
            }

            .about-image img {
                height: 300px;
            }

            .image-label {
                left: 10px;
            }

            .about-text h2 {
                font-size: 30px;
            }

            .program-grid,
            .facility-grid {
                grid-template-columns: 1fr;
            }

            .admission-inner {
                align-items: flex-start;
                flex-direction: column;
            }

            .footer-grid {
                grid-template-columns: 1fr;
                gap: 30px;
            }
        }

        @media (max-width: 400px) {
            .logo h2 {
                font-size: 16px;
            }

            .logo-icon {
                width: 42px;
                height: 42px;
            }

            .form-row {
                grid-template-columns: 1fr;
                gap: 0;
            }

            .btn-outline {
                margin: 12px 0 0;
            }
        }
    </style>
</head>

<body>

    <div class="topbar">
        <div class="container">
            <span>✉ Welcome to BM Public School</span>
            <span>Admissions Information Available Now</span>
        </div>
    </div>

    <header>
        <nav class="container">
            <a href="#home" class="logo">
                <div class="logo-icon">BM</div>
                <div>
                    <h2>BM PUBLIC SCHOOL</h2>
                    <span>LEARN • GROW • SUCCEED</span>
                </div>
            </a>

            <button class="menu-btn" id="menu-btn"
                    aria-label="Toggle navigation"
                    aria-expanded="false">☰</button>

            <ul class="nav-links" id="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#programs">Academics</a></li>
                <li><a href="#facilities">Facilities</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#contact" class="nav-cta">Apply Now ↗</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <!-- HERO SECTION -->

        <section class="hero" id="home">
            <div class="container">
                <div class="hero-content">
                    <span class="eyebrow">✦ Education for a Brighter Future</span>

                    <h1>Where Young Minds <span>Become Great Leaders.</span></h1>

                    <p>
                        At BM Public School, we believe every student has the
                        potential to achieve something extraordinary. Discover
                        a learning environment built around knowledge,
                        creativity, confidence and character.
                    </p>

                    <a href="#contact" class="btn btn-primary">
                        Explore Admissions →
                    </a>

                    <a href="#about" class="btn btn-outline">
                        Discover Our School
                    </a>
                </div>
            </div>
        </section>

        <!-- SCHOOL STATISTICS -->

        <section class="stats">
            <div class="container">
                <div class="stats-grid">
                    <div class="stat">
                        <h2>01</h2>
                        <p>A Place to Learn</p>
                    </div>
                    <div class="stat">
                        <h2>360°</h2>
                        <p>Holistic Development</p>
                    </div>
                    <div class="stat">
                        <h2>100%</h2>
                        <p>Focus on Growth</p>
                    </div>
                    <div class="stat">
                        <h2>∞</h2>
                        <p>Possibilities Ahead</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- ABOUT SECTION -->

        <section class="section" id="about">
            <div class="container">
                <div class="about-grid">

                    <div class="about-image">
                        <img
                            src="https://images.unsplash.com/photo-1509062522246-3755977927d7?auto=format&fit=crop&w=1000&q=85"
                            alt="Students learning together in a classroom"
                            loading="lazy">

                        <div class="image-label">
                            Building Tomorrow's Leaders
                        </div>
                    </div>

                    <div class="about-text">
                        <span class="mini-title">About Our School</span>

                        <h2>Education That Goes Beyond the Classroom.</h2>

                        <p>
                            BM Public School aims to provide students with
                            a supportive environment where curiosity is
                            encouraged, ideas are explored and learning
                            becomes a lifelong journey.
                        </p>

                        <p>
                            Our approach combines academic learning with
                            practical experiences, creative activities
                            and opportunities to develop essential life skills.
                        </p>

                        <ul class="check-list">
                            <li>Student-focused learning environment</li>
                            <li>Academic and personal development</li>
                            <li>Sports, creativity and teamwork</li>
                            <li>Values, discipline and responsibility</li>
                        </ul>

                        <a href="#facilities" class="btn btn-primary">
                            Explore Our Facilities →
                        </a>
                    </div>

                </div>
            </div>
        </section>

        <!-- ACADEMICS -->

        <section class="section programs" id="programs">
            <div class="container">
                <div class="section-heading">
                    <span>Our Academics</span>
                    <h2>A Strong Foundation for Every Future</h2>
                    <p>
                        Learning opportunities designed to support students
                        at different stages of their educational journey.
                    </p>
                </div>

                <div class="program-grid">

                    <article class="program-card">
                        <img
                            src="https://images.unsplash.com/photo-1503454537195-1dcabb73ffb9?auto=format&fit=crop&w=800&q=80"
                            alt="Young students learning"
                            loading="lazy">

                        <div class="program-content">
                            <span class="number">01 / FOUNDATION</span>
                            <h3>Primary Education</h3>
                            <p>
                                Encourage curiosity, literacy, numeracy
                                and creativity through engaging learning
                                experiences.
                            </p>
                            <a href="#contact" class="text-link">
                                Enquire Now →
                            </a>
                        </div>
                    </article>

                    <article class="program-card">
                        <img
                            src="https://images.unsplash.com/photo-1427504494785-3a9ca7044f45?auto=format&fit=crop&w=800&q=80"
                            alt="Students working together"
                            loading="lazy">

                        <div class="program-content">
                            <span class="number">02 / DEVELOPMENT</span>
                            <h3>Middle Education</h3>
                            <p>
                                Build stronger subject knowledge, critical
                                thinking, communication and problem-solving
                                skills.
                            </p>
                            <a href="#contact" class="text-link">
                                Enquire Now →
                            </a>
                        </div>
                    </article>

                    <article class="program-card">
                        <img
                            src="https://images.unsplash.com/photo-1523050854058-8df90110c9f1?auto=format&fit=crop&w=800&q=80"
                            alt="Students celebrating their education"
                            loading="lazy">

                        <div class="program-content">
                            <span class="number">03 / FUTURE READY</span>
                            <h3>Senior Education</h3>
                            <p>
                                Support academic goals, independent thinking
                                and preparation for future educational
                                opportunities.
                            </p>
                            <a href="#contact" class="text-link">
                                Enquire Now →
                            </a>
                        </div>
                    </article>

                </div>
            </div>
        </section>

        <!-- FACILITIES -->

        <section class="section" id="facilities">
            <div class="container">

                <div class="section-heading">
                    <span>Life at BM</span>
                    <h2>More Than Just Classrooms</h2>
                    <p>
                        A well-rounded educational experience encourages
                        students to explore their interests and discover
                        their strengths.
                    </p>
                </div>

                <div class="facility-grid">

                    <div class="facility">
                        <div class="facility-icon">📚</div>
                        <h3>Learning Resources</h3>
                        <p>
                            Encourage reading, research and independent
                            learning through educational resources.
                        </p>
                    </div>

                    <div class="facility">
                        <div class="facility-icon">🔬</div>
                        <h3>Practical Learning</h3>
                        <p>
                            Explore scientific ideas through experiments,
                            demonstrations and hands-on activities.
                        </p>
                    </div>

                    <div class="facility">
                        <div class="facility-icon">💻</div>
                        <h3>Digital Education</h3>
                        <p>
                            Develop digital awareness and technology skills
                            for an increasingly connected world.
                        </p>
                    </div>

                    <div class="facility">
                        <div class="facility-icon">⚽</div>
                        <h3>Sports & Fitness</h3>
                        <p>
                            Build teamwork, confidence, discipline and
                            healthy habits through physical activities.
                        </p>
                    </div>

                    <div class="facility">
                        <div class="facility-icon">🎨</div>
                        <h3>Arts & Creativity</h3>
                        <p>
                            Give students opportunities to express themselves
                            through art, music and creative projects.
                        </p>
                    </div>

                    <div class="facility">
                        <div class="facility-icon">🌱</div>
                        <h3>Personal Growth</h3>
                        <p>
                            Encourage kindness, leadership, responsibility
                            and respect for others.
                        </p>
                    </div>

                </div>
            </div>
        </section>

        <!-- ADMISSION CTA -->

        <section class="admission">
            <div class="container">
                <div class="admission-inner">
                    <div>
                        <span class="mini-title">Your Future Starts Here</span>
                        <h2>Give Your Child a Brighter Tomorrow.</h2>
                        <p>
                            Contact our school to learn about admissions,
                            academic programmes and enrolment requirements.
                        </p>
                    </div>

                    <a href="#contact" class="btn btn-primary">
                        Enquire About Admission ↗
                    </a>
                </div>
            </div>
        </section>

        <!-- CONTACT -->

        <section class="section" id="contact">
            <div class="container">
                <div class="contact-grid">

                    <div class="contact-info">
                        <span class="mini-title">Get In Touch</span>
                        <h2>Let's Start Your Child's Journey.</h2>

                        <p>
                            Have questions about our school or admissions?
                            Send an enquiry and let us know how we can help.
                        </p>

                        <div class="contact-item">
                            <strong>📍 School Address</strong>
                            Garhi Harsaru, Gurugram, Haryana
                        </div>

                        <div class="contact-item">
                            <strong>✉ Email</strong>
                            Add the school's official email here
                        </div>

                        <div class="contact-item">
                            <strong>☎ Phone</strong>
                            Add the school's official phone number here
                        </div>
                    </div>

                    <form class="contact-form" id="contact-form">
                        <h3>Send an Enquiry</h3>

                        <div class="form-row">
                            <input type="text" name="parent"
                                   placeholder="Parent's Name" required>

                            <input type="tel" name="phone"
                                   placeholder="Phone Number"
                                   pattern="[0-9+\s()-]{7,20}" required>
                        </div>

                        <input type="email" name="email"
                               placeholder="Email Address" required>

                        <select name="class" required>
                            <option value="">Select Class of Interest</option>
                            <option>Primary Classes</option>
                            <option>Middle Classes</option>
                            <option>Secondary Classes</option>
                            <option>Senior Secondary Classes</option>
                            <option>Other Enquiry</option>
                        </select>

                        <textarea name="message"
                                  placeholder="Write your message..."
                                  required></textarea>

                        <button type="submit" class="btn btn-primary">
                            Submit Enquiry →
                        </button>

                        <p id="form-message" aria-live="polite"></p>
                    </form>

                </div>
            </div>
        </section>
    </main>

    <!-- FOOTER -->

    <footer>
        <div class="container">

            <div class="footer-grid">

                <div class="footer-about">
                    <a href="#home" class="logo">
                        <div class="logo-icon"
                             style="background:#f5a623;color:#172b4d;">
                            BM
                        </div>

                        <div>
                            <h2 style="color:white;">BM PUBLIC SCHOOL</h2>
                            <span style="color:#bdc9d8;">
                                LEARN • GROW • SUCCEED
                            </span>
                        </div>
                    </a>

                    <p>
                        Inspiring students to learn with curiosity,
                        grow with confidence and succeed with purpose.
                    </p>
                </div>

                <div>
                    <h3>Quick Links</h3>
                    <ul class="footer-links">
                        <li><a href="#home">Home</a></li>
                        <li><a href="#about">About Us</a></li>
                        <li><a href="#programs">Academics</a></li>
                        <li><a href="#facilities">Facilities</a></li>
                        <li><a href="#contact">Admissions</a></li>
                    </ul>
                </div>

                <div>
                    <h3>Contact Information</h3>
                    <ul class="footer-links">
                        <li>Garhi Harsaru, Gurugram</li>
                        <li>Haryana, India</li>
                        <li>Official email: Add here</li>
                        <li>School phone: Add here</li>
                    </ul>
                </div>

            </div>

            <div class="copyright">
                © <span id="year"></span> BM Public School.
                All rights reserved.
            </div>
        </div>
    </footer>

    <script>
        // Mobile navigation

        const menuBtn = document.getElementById("menu-btn");
        const navLinks = document.getElementById("nav-links");

        menuBtn.addEventListener("click", function () {
            const isOpen = navLinks.classList.toggle("active");

            menuBtn.textContent = isOpen ? "✕" : "☰";
            menuBtn.setAttribute("aria-expanded", isOpen);
        });

        // Close menu after clicking a link

        document.querySelectorAll(".nav-links a").forEach(function (link) {
            link.addEventListener("click", function () {
                navLinks.classList.remove("active");
                menuBtn.textContent = "☰";
                menuBtn.setAttribute("aria-expanded", "false");
            });
        });

        // Automatically update copyright year

        document.getElementById("year").textContent =
            new Date().getFullYear();

        // Contact form demonstration

        document.getElementById("contact-form")
            .addEventListener("submit", function (event) {
                event.preventDefault();

                document.getElementById("form-message").textContent =
                    "Your form is working in demo mode. Connect a form service or backend to receive enquiries.";

                this.reset();
            });
    </script>

</body>
</html>
