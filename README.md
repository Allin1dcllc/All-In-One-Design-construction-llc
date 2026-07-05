<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>All in One Design & Construction LLC</title>
    <style>
        :root {
            --primary: #1a1a1a;
            --accent: #b89265; /* Craft gold/bronze */
            --light-bg: #f9f9f9;
            --text: #333333;
            --white: #ffffff;
            --gray: #666666;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            color: var(--text);
            background-color: var(--white);
            line-height: 1.6;
        }

        /* Header & Navigation */
        header {
            background-color: var(--primary);
            color: var(--white);
            padding: 1rem 2rem;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.3);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-weight: 700;
            font-size: 1.4rem;
            letter-spacing: 1px;
        }

        .logo span {
            color: var(--accent);
        }

        .mhic-badge {
            font-size: 0.8rem;
            background: #333;
            padding: 4px 8px;
            border-radius: 4px;
            border: 1px solid var(--accent);
            color: var(--white);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.65), rgba(0,0,0,0.65)), url('https://images.unsplash.com/photo-1600585154340-be6161a56a0c?auto=format&fit=crop&w=1920&q=80') no-repeat center center/cover;
            height: 80vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: var(--white);
            padding: 0 1rem;
            margin-top: 60px;
        }

        .hero-content h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .hero-content p {
            font-size: 1.3rem;
            color: #dddddd;
            max-width: 800px;
            margin: 0 auto 2rem auto;
        }

        .cta-btn {
            background-color: var(--accent);
            color: var(--white);
            padding: 0.8rem 2rem;
            text-decoration: none;
            font-weight: 600;
            border-radius: 4px;
            transition: background 0.3s ease;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .cta-btn:hover {
            background-color: #a37f55;
        }

        /* Main Content Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 4rem 2rem;
        }

        .section-title {
            text-align: center;
            font-size: 2.2rem;
            margin-bottom: 3rem;
            position: relative;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background-color: var(--accent);
            margin: 10px auto 0 auto;
        }

        /* Specialties / Features Grid */
        .specialties {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2.5rem;
            margin-bottom: 4rem;
        }

        .spec-card {
            background: var(--light-bg);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }

        .spec-card:hover {
            transform: translateY(-5px);
        }

        .spec-img {
            height: 240px;
            background-size: cover;
            background-position: center;
        }

        .spec-info {
            padding: 1.5rem;
        }

        .spec-info h3 {
            margin-bottom: 0.5rem;
            color: var(--primary);
            font-size: 1.3rem;
        }

        /* Before/After Transformation Showcase */
        .transform-showcase {
            background-color: var(--light-bg);
            padding: 4rem 2rem;
            border-radius: 12px;
            margin-bottom: 4rem;
        }

        .transform-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
        }

        @media (max-width: 768px) {
            .transform-grid {
                grid-template-columns: 1fr;
            }
        }

        .transform-box {
            background: var(--white);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
        }

        .transform-header {
            background: var(--primary);
            color: var(--white);
            padding: 0.5rem 1rem;
            font-weight: 600;
            text-align: center;
            text-transform: uppercase;
            font-size: 0.9rem;
            letter-spacing: 1px;
        }

        .transform-header.after {
            background: var(--accent);
        }

        .transform-img {
            height: 350px;
            background-size: cover;
            background-position: center;
        }

        /* Footer & Business Info */
        footer {
            background-color: var(--primary);
            color: #bbbbbb;
            padding: 4rem 2rem 2rem 2rem;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            border-bottom: 1px solid #333;
            padding-bottom: 3rem;
            margin-bottom: 2rem;
        }

        .footer-section h4 {
            color: var(--white);
            margin-bottom: 1.2rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-size: 1.1rem;
        }

        .footer-section p {
            margin-bottom: 0.8rem;
        }

        .footer-section strong {
            color: var(--accent);
        }

        .footer-bottom {
            max-width: 1200px;
            margin: 0 auto;
            text-align: center;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <!-- Header Navigation -->
    <header>
        <div class="nav-container">
            <div class="logo">ALL IN ONE <span>DESIGN & CONSTRUCTION</span></div>
            <div class="mhic-badge">MHIC License #166439</div>
        </div>
    </header>

    <!-- Hero Showcase Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>Craftsmanship Without Compromise</h1>
            <p>From custom framing and precision drywall systems to high-end bathroom and kitchen transformations. We don't just build spaces—we design them to endure.</p>
            <a href="#contact" class="cta-btn">Discuss Your Project</a>
        </div>
    </section>

    <!-- Capabilities & Potential Section -->
    <main class="container">
        <h2 class="section-title">Specialized Capabilities</h2>
        
        <div class="specialties">
            <!-- Custom Bathrooms -->
            <div class="spec-card">
                <div class="spec-img" style="background-image: url('https://images.unsplash.com/photo-1620626011161-997e5a947d57?auto=format&fit=crop&w=600&q=80');"></div>
                <div class="spec-info">
                    <h3>Custom Bathroom Renovations</h3>
                    <p>High-end tiling, large-format custom installations, frameless glass features, and tub-to-shower conversions designed with perfection down to the grout lines.</p>
                </div>
            </div>

            <!-- Custom Kitchens -->
            <div class="spec-card">
                <div class="spec-img" style="background-image: url('https://images.unsplash.com/photo-1556911220-e15b29be8c8f?auto=format&fit=crop&w=600&q=80');"></div>
                <div class="spec-info">
                    <h3>Premium Kitchen Design</h3>
                    <p>Intelligent spatial layouts, professional utility rough-ins, solid surfaces, and structural updates configured to maximize workflow and timeless architectural character.</p>
                </div>
            </div>

            <!-- Drywall & Architectural Lighting -->
            <div class="spec-card">
                <div class="spec-img" style="background-image: url('https://images.unsplash.com/photo-1513694203232-719a280e022f?auto=format&fit=crop&w=600&q=80');"></div>
                <div class="spec-info">
                    <h3>Precision Drywall & Hidden LED Strips</h3>
                    <p>Flawless drywall systems integrated with contemporary lighting design. We specialize in flush-mount aluminum channels embedded directly into ceilings and walls for beautiful, hidden architectural LED illumination.</p>
                </div>
            </div>
        </div>

        <!-- Before/After Case Study Section -->
        <h2 class="section-title">Featured Transformation</h2>
        <div class="transform-showcase">
            <div class="transform-grid">
                <!-- Before Box -->
                <div class="transform-box">
                    <div class="transform-header">Before Project Base</div>
                    <div class="transform-img" style="background-image: url('https://images.unsplash.com/photo-1584622650111-993a426fbf0a?auto=format&fit=crop&w=800&q=80');"></div>
                </div>
                <!-- After Box -->
                <div class="transform-box">
                    <div class="transform-header after">Completed Design</div>
                    <div class="transform-img" style="background-image: url('https://images.unsplash.com/photo-1552321554-5fefe8c9ef14?auto=format&fit=crop&w=800&q=80');"></div>
                </div>
            </div>
        </div>
    </main>

    <!-- Footer & Detailed Business Information -->
    <footer id="contact">
        <div class="footer-content">
            <div class="footer-section">
                <h4>All in One Design & Construction LLC</h4>
                <p>Bringing structural excellence and sophisticated finish execution to every project. We operate under rigorous construction standards to deliver absolute reliability.</p>
            </div>
            <div class="footer-section">
                <h4>Licensing & Compliance</h4>
                <p><strong>Maryland Home Improvement Commission</strong></p>
                <p>MHIC License Number: <strong>166439</strong></p>
                <p>Fully Insured and Bonded Residential Improvement Contractor.</p>
            </div>
            <div class="footer-section">
                <h4>Let's Talk Concepts</h4>
                <p>Ready to push your property to its maximum potential? Contact us to review blueprints, structural challenges, or custom tile and lighting layouts.</p>
                <p>Email: <strong>contact@allinonedesignconstruction.com</strong></p>
            </div>
        </div>
        <div class="footer-bottom">
            &copy; 2026 All in One Design & Construction LLC. All Rights Reserved.
        </div>
    </footer>

</body>
</html>
