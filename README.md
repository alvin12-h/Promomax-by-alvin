<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Promomax Ads</title>
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Dancing+Script:wght@600&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* General Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        /* Body and Background */
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #00203F, #004e92);
            color: white;
            overflow-x: hidden;
        }

        /* Header */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 50px;
            background: rgba(0, 0, 30, 0.9);
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.7);
        }

        header img {
            width: 100px;
        }

        nav ul {
            list-style: none;
            display: flex;
        }

        nav ul li {
            margin-left: 30px;
        }

        nav ul li a {
            text-decoration: none;
            font-size: 18px;
            font-weight: 600;
            color: white;
            padding: 8px 15px;
            border-radius: 5px;
            transition: all 0.3s;
        }

        nav ul li a:hover {
            background: cyan;
            color: black;
        }

        /* Ensure offset for anchor links */
        section {
            scroll-margin-top: 80px;
        }

        /* Hero Section */
        .hero {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            text-align: center;
            height: 100vh;
            background: linear-gradient(135deg, rgba(0, 50, 80, 0.9), rgba(0, 30, 60, 0.9));
            color: white;
            background-image: url('pattern.png');
            background-size: cover;
            background-attachment: fixed;
        }

        .hero h1 {
            font-size: 150px;
            font-family: 'Pacifico', cursive;
            animation: pulse 2s infinite;
            text-shadow: 3px 3px 5px rgba(0, 0, 0, 0.7);
            color: cyan;
        }

        .hero p {
            font-size: 2rem;
            margin-top: 15px;
            max-width: 700px;
        }

        .hero .cta {
            margin-top: 30px;
            padding: 15px 30px;
            font-size: 1.1rem;
            background: cyan;
            color: black;
            text-decoration: none;
            border-radius: 50px;
            transition: background 0.3s, transform 0.2s;
        }

        .hero .cta:hover {
            background: white;
            transform: scale(1.05);
        }

        @keyframes pulse {
            0% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.05);
            }
            100% {
                transform: scale(1);
            }
        }

        /* About Section */
        .about {
            padding: 50px 20px;
            background: rgba(0, 10, 40, 0.9);
            text-align: center;
        }

        .about h2 {
            font-size: 3rem;
            font-family: 'Pacifico', cursive;
            margin-bottom: 20px;
            color: cyan;
        }

        .about p {
            max-width: 800px;
            margin: 0 auto;
            font-size: 1.2rem;
            line-height: 1.8;
        }

        /* Services Section */
        .services {
            padding: 50px 20px;
            background: rgba(0, 0, 50, 0.95);
            text-align: center;
        }

        .services h2 {
            font-size: 3rem;
            font-family: 'Pacifico', cursive;
            margin-bottom: 20px;
            color: cyan;
        }

        .services-box {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 40px;
            flex-wrap: wrap;
        }

        .services-box .box {
            background: linear-gradient(145deg, #004e92, #000428);
            color: white;
            padding: 30px;
            border-radius: 10px;
            width: 300px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.7);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .services-box .box:hover {
            transform: translateY(-10px) scale(1.05);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.9);
        }

        .services-box .box h3 {
            font-size: 1.8rem;
            margin-bottom: 10px;
            font-family: 'Dancing Script', cursive;
            color: cyan;
        }

        /* Get Started Section */
        .get-started {
            padding: 50px 20px;
            background: rgba(0, 0, 30, 0.9);
            text-align: center;
        }

        .get-started h2 {
            font-size: 3rem;
            font-family: 'Pacifico', cursive;
            margin-bottom: 20px;
            color: cyan;
        }

        .get-started p {
            font-size: 1.2rem;
            margin-bottom: 20px;
        }

        .get-started form {
            max-width: 700px;
            margin: 0 auto;
            text-align: left;
            background: rgba(0, 0, 60, 0.9);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.8);
        }

        .get-started label {
            font-size: 1.2rem;
            margin-bottom: 5px;
            display: block;
            color: white;
        }

        .get-started input, .get-started textarea {
            width: 100%;
            padding: 15px;
            margin: 10px 0 20px 0;
            border: 2px solid #004e92;
            border-radius: 5px;
            font-size: 1.2rem;
            background: rgba(0, 0, 60, 0.8);
            color: white;
            transition: border-color 0.3s, background-color 0.3s;
        }

        .get-started input:focus, .get-started textarea:focus {
            border-color: cyan;
            background-color: rgba(0, 0, 70, 0.8);
            outline: none;
        }

        .get-started button {
            padding: 15px 30px;
            background: cyan;
            color: black;
            font-size: 1.2rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s, transform 0.2s;
        }

        .get-started button:hover {
            background: white;
            transform: scale(1.05);
        }

        /* Footer */
        footer {
            background: rgba(0, 0, 40, 0.9);
            padding: 20px;
            text-align: center;
            font-size: 1rem;
            color: white;
            font-family: 'Poppins', sans-serif;
            border-top: 1px solid cyan;
        }

        footer p {
            font-size: 0.9rem;
        }

        footer p strong {
            color: cyan;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                text-align: center;
            }

            nav ul {
                flex-direction: column;
                margin-top: 15px;
            }

            nav ul li {
                margin: 10px 0;
            }

            .hero h1 {
                font-size: 4rem;
            }

            .services-box {
                flex-direction: column;
            }
        }
    
     .contact {
            padding: 50px 20px;
            background: rgba(0, 0, 30, 0.9);
            text-align: center;
        }

        .contact h2 {
            font-size: 3rem;
            font-family: 'Pacifico', cursive;
            margin-bottom: 20px;
            color: cyan;
        }

        .contact p {
            font-size: 1.2rem;
            margin-bottom: 40px;
            color: white;
        }

        .contact-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .contact-item {
            background: linear-gradient(145deg, #004e92, #000428);
            padding: 30px;
            border-radius: 10px;
            width: 300px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.7);
            transition: transform 0.3s, box-shadow 0.3s;
            text-align: center;
            color: white;
        }

        .contact-item:hover {
            transform: translateY(-10px) scale(1.05);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.9);
        }

        .contact-item h3 {
            font-size: 1.8rem;
            margin-bottom: 10px;
            font-family: 'Dancing Script', cursive;
            color: cyan;
        }

        .contact-item a {
            color: white;
            text-decoration: none;
            font-size: 1rem;
        }

        .contact-item a:hover {
            color: cyan;
            text-decoration: underline;
        }

    </style>
</head>
<body>
    <!-- HEADER -->
    <header>
        <img src="1.png" alt="Promomax Ads Logo">
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact Us</a></li>
                <li><a href="#get-started">Get Started</a></li>
            </ul>
        </nav>
    </header>

    <!-- HERO -->
    <section id="home" class="hero">
        <h1>Welcome to Promomax Ads</h1>
        <p>Unlock your brand's potential with Promomax Ads! Let us take your business to new heights with effective advertising strategies.</p>
        <a href="#about" class="cta">Learn More</a>
    </section>

    <!-- ABOUT -->
    <section id="about" class="about">
        <h2>About Us</h2>
        <p>Promomax Ads is a leading advertising agency specializing in creating powerful marketing strategies tailored to your business needs.</p>
    </section>

    <!-- SERVICES -->
    <section id="services" class="services">
        <h2>Our Services</h2>
        <div class="services-box">
            <div class="box">
                <h3>Digital Advertising</h3>
                <p>Expand your reach with targeted digital ads.</p>
            </div>
            <div class="box">
                <h3>Brand Strategy</h3>
                <p>Let’s craft a winning strategy for your brand.</p>
            </div>
            <div class="box">
                <h3>Social Media Management</h3>
                <p>Grow and engage your audience on all platforms.</p>
            </div>
            <div class="box">
                <h3>Content Marketing</h3>
                <p>Captivate your audience with compelling content.</p>
            </div>
            <div class="box">
                <h3>SEO Optimization</h3>
                <p>Boost your online visibility with SEO.</p>
            </div>
            <div class="box">
                <h3>Market Analysis</h3>
                <p>Gain insights and stay ahead of competitors.</p>
            </div>
        </div>
    </section>

    <!-- GET STARTED -->
    <section id="get-started" class="get-started">
        <h2>Get Started</h2>
        <p>To try our services, please fill out this form.</p>
        <form>
            <label for="name">Name</label>
            <input type="text" id="name" name="name" placeholder="Your Full Name" required>
            <label for="email">Email</label>
            <input type="email" id="email" name="email" placeholder="Your Email Address" required>
            <label for="message">Message</label>
            <textarea id="message" name="message" rows="5" placeholder="Your Message" required></textarea>
            <button type="submit">Submit</button>
        </form>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>We’d love to hear from you! Reach out to us via any of the following:</p>
        <div class="contact-container">
            <div class="contact-item">
                <h3>Email</h3>
                <p><a href="mailto:alvindelacruz@gmail.com">alvindelacruz@gmail.com</a></p>
            </div>
            <div class="contact-item">
                <h3>Phone</h3>
                <p><a href="tel:+639756067872">+63 975 606 7872</a></p>
            </div>
            <div class="contact-item">
                <h3>Location</h3>
                <p>Mabalacat, Pampanga</p>
            </div>
        </div>
    </section>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <p>&copy; 2024 Promomax Ads. All rights reserved.</p>
        <p>Designed with care by <strong>Promomax Ads Team</strong>.</p>
    </footer>
</body>
</html>
