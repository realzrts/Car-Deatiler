[index.html](https://github.com/user-attachments/files/29061140/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Weekend Ready Detail | Premium Car Wash & Detailing</title>
    <!-- Google Fonts for Modern Typography -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Antonio:wght@700&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
    
    <style>
        /* Base Reset & Brand Colors */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        :root {
            --bg-dark: #0b0c10;
            --bg-card: #1f2833;
            --text-light: #ffffff;
            --text-muted: #c5a880; /* Subtle Gold/Champagne accent for luxury detailing look */
            --accent-blue: #45f3ff; /* Electric blue representing fresh water/clean finish */
            --border-line: #2d3748;
        }
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg-dark);
            color: var(--text-light);
            line-height: 1.6;
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 5%;
            background: rgba(11, 12, 16, 0.95);
            border-bottom: 1px solid var(--border-line);
            position: sticky;
            top: 0;
            z-index: 100;
            backdrop-filter: blur(10px);
        }
        .logo {
            font-family: 'Antonio', sans-serif;
            font-size: 1.6rem;
            letter-spacing: 1px;
            color: var(--text-light);
            text-transform: uppercase;
        }
        .logo span {
            color: var(--text-muted);
        }
        .nav-btn {
            background: var(--text-light);
            color: var(--bg-dark);
            padding: 10px 20px;
            border: none;
            font-weight: 700;
            cursor: pointer;
            text-decoration: none;
            font-size: 0.85rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            transition: all 0.2s ease;
        }
        .nav-btn:hover {
            background: var(--text-muted);
            color: var(--text-light);
        }

        /* Hero Section */
        .hero {
            padding: 50px 5% 30px 5%;
            max-width: 800px;
            margin: 0 auto;
            text-align: left;
        }
        .rating-badge {
            color: #ffb703; /* Gold stars */
            font-size: 0.9rem;
            margin-bottom: 12px;
            display: flex;
            align-items: center;
            gap: 6px;
            font-weight: 600;
        }
        .rating-count {
            color: #a0aec0;
            font-size: 0.8rem;
            letter-spacing: 0.5px;
        }
        h1 {
            font-family: 'Antonio', sans-serif;
            font-size: 3.8rem;
            line-height: 1.05;
            text-transform: uppercase;
            margin-bottom: 20px;
            letter-spacing: -0.5px;
        }
        .tagline {
            font-size: 1.15rem;
            color: #e2e8f0;
            margin-bottom: 25px;
            max-width: 650px;
        }
        
        /* Badges Row */
        .badge-container {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 35px;
        }
        .badge {
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid var(--border-line);
            padding: 6px 14px;
            font-size: 0.8rem;
            font-weight: 600;
            border-radius: 50px;
            color: #cbd5e1;
        }

        .hero-img-box {
            width: 100%;
            height: 350px;
            border-radius: 8px;
            overflow: hidden;
            margin-bottom: 40px;
            border: 1px solid var(--border-line);
        }
        .hero-img-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        /* Services Menu Section */
        .services-section {
            background-color: rgba(255, 255, 255, 0.02);
            border-top: 1px solid var(--border-line);
            border-bottom: 1px solid var(--border-line);
            padding: 60px 5%;
        }
        .section-container {
            max-width: 800px;
            margin: 0 auto;
        }
        .services-section h2 {
            font-family: 'Antonio', sans-serif;
            font-size: 2.2rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 10px;
            color: var(--text-muted);
        }
        .section-subtitle {
            color: #a0aec0;
            margin-bottom: 30px;
            font-size: 0.95rem;
        }
        .service-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            border-bottom: 1px solid var(--border-line);
        }
        .service-name {
            font-size: 1.1rem;
            font-weight: 600;
            letter-spacing: 0.3px;
        }
        .estimate-link {
            color: var(--accent-blue);
            text-transform: uppercase;
            font-size: 0.85rem;
            font-weight: 700;
            letter-spacing: 1px;
            text-decoration: none;
            transition: opacity 0.2s;
        }
        .estimate-link:hover {
            text-decoration: underline;
        }

        /* Business Overview & Info */
        .info-section {
            padding: 60px 5%;
            max-width: 800px;
            margin: 0 auto;
        }
        .info-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
        }
        .info-block h3 {
            font-family: 'Antonio', sans-serif;
            font-size: 1.5rem;
            text-transform: uppercase;
            margin-bottom: 20px;
            letter-spacing: 0.5px;
            color: var(--text-muted);
        }
        .info-block p {
            color: #cbd5e1;
            margin-bottom: 8px;
            font-size: 1rem;
        }
        .highlight-text {
            color: var(--accent-blue) !important;
            font-weight: 600;
        }

        /* Reviews Section */
        .reviews-section {
            padding: 20px 5% 120px 5%;
            max-width: 800px;
            margin: 0 auto;
        }
        .reviews-section h3 {
            font-family: 'Antonio', sans-serif;
            font-size: 1.5rem;
            text-transform: uppercase;
            margin-bottom: 25px;
            letter-spacing: 0.5px;
        }
        .review-card {
            background: rgba(255, 255, 255, 0.02);
            border: 1px solid var(--border-line);
            padding: 25px;
            margin-bottom: 20px;
            border-radius: 6px;
        }
        .review-quote {
            font-style: italic;
            font-size: 1.1rem;
            color: #f1f5f9;
            margin-bottom: 12px;
            line-height: 1.5;
        }
        .review-meta {
            font-size: 0.8rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            color: #a0aec0;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        .review-meta span {
            color: #ffb703;
        }

        /* Sticky Action Button */
        .sticky-action {
            position: fixed;
            bottom: 25px;
            left: 50%;
            transform: translateX(-50%);
            width: 92%;
            max-width: 500px;
            background-color: var(--text-light);
            color: var(--bg-dark);
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 18px 28px;
            text-decoration: none;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-size: 0.95rem;
            box-shadow: 0 15px 35px rgba(0,0,0,0.6);
            border-radius: 4px;
            z-index: 1000;
            transition: all 0.2s ease;
        }
        .sticky-action:hover {
            background-color: var(--text-muted);
            color: var(--text-light);
            transform: translate(-50%, -2px);
        }
        .sticky-action span:last-child {
            font-size: 1.2rem;
        }

        /* Responsive Breakpoints */
        @media (max-width: 680px) {
            h1 { font-size: 2.8rem; }
            .info-grid { grid-template-columns: 1fr; gap: 30px; }
            .hero-img-box { height: 220px; }
        }
    </style>
</head>
<body>

    <!-- Navigation Bar -->
    <nav>
        <div class="logo">Weekend Ready<span>.</span></div>
        <a href="tel:9727298958" class="nav-btn">Call Now</a>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <div class="rating-badge">
            <span>★★★★★ 4.9</span>
            <span class="rating-count">(189 GOOGLE REVIEWS)</span>
        </div>
        <h1>Weekend Ready Detailing</h1>
        <p class="tagline">
            Premium car wash and professional detailing services serving Plano and nearby areas. 3+ years of trusted, detail-oriented care to leave your vehicle looking brand new.
        </p>
        
        <!-- Trust Badges From Google Info -->
        <div class="badge-container">
            <div class="badge">✓ Google Verified</div>
            <div class="badge">✓ Locally-Owned & Operated</div>
            <div class="badge">✓ Free Estimates</div>
            <div class="badge">✓ Military Discount Available</div>
            <div class="badge">✓ Accepts Insurance</div>
        </div>
        
        <div class="hero-img-box">
            <!-- Sleek dark vehicle image matching the theme -->
            <img src="https://images.unsplash.com/photo-1607860108855-64acf2078ed9?auto=format&fit=crop&w=1200&q=80" alt="Luxury car detailing finish">
        </div>
    </section>

    <!-- Service Menu Section -->
    <section class="services-section">
        <div class="section-container">
            <h2>Our Services</h2>
            <p class="section-subtitle">Known across the area for unmatched precision and attention to detail.</p>
            
            <div class="service-row">
                <span class="service-name">Interior Detailing</span>
                <a href="#" class="estimate-link">Free Estimate</a>
            </div>
            <div class="service-row">
                <span class="service-name">Exterior Washing & Paint Care</span>
                <a href="#" class="estimate-link">Free Estimate</a>
            </div>
            <div class="service-row">
                <span class="service-name">Waxing & Ceramic Coating</span>
                <a href="#" class="estimate-link">Free Estimate</a>
            </div>
            <div class="service-row">
                <span class="service-name">Engine Detailing</span>
                <a href="#" class="estimate-link">Free Estimate</a>
            </div>
            <div class="service-row">
                <span class="service-name">Tire & Wheel Cleaning</span>
                <a href="#" class="estimate-link">Free Estimate</a>
            </div>
        </div>
    </section>

    <!-- Location & Booking Details Section -->
    <section class="info-section">
        <div class="info-grid">
            <div class="info-block">
                <h3>Contact & Area</h3>
                <p class="highlight-text">📍 Serves Plano & Nearby Areas</p>
                <p>📞 (972) 729-8958</p>
                <p>🌐 www.weekendreadydetail.com</p>
            </div>

            <div class="info-block">
                <h3>Hours & Response</h3>
                <p><strong>Open Now</strong> — Closes 6:00 PM</p>
                <p style="margin-top: 10px; color: #a0aec0; font-size: 0.9rem;">
                    💬 Message response time: <span style="color: var(--accent-blue);">Typically 30 mins</span>
                </p>
            </div>
        </div>
    </section>

    <!-- Reviews Section -->
    <section class="reviews-section">
        <h3>Word on the street</h3>
        
        <div class="review-card">
            <p class="review-quote">"Always leaves my truck looking brand new."</p>
            <div class="review-meta"><span>★★★★★</span> Google Review</div>
        </div>
        <div class="review-card">
            <p class="review-quote">"Easy drop off and great communication 👌"</p>
            <div class="review-meta"><span>★★★★★</span> Google Review</div>
        </div>
        <div class="review-card">
            <p class="review-quote">"Thank you again for such a great job. Reviews mention attention to detail."</p>
            <div class="review-meta"><span>★★★★★</span> Google Review</div>
        </div>
    </section>

    <!-- Floating Sticky Action Button -->
    <a href="tel:9727298958" class="sticky-action">
        <span>Message Business</span>
        <span>→</span>
    </a>

</body>
</html>
