<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apraizrr - Find the Best Car Deals on Facebook Marketplace</title>
    <style>
        :root {
            --primary-color: #4285F4;
            --secondary-color: #34A853;
            --accent-color: #EA4335;
            --dark-color: #1E1E1E;
            --light-color: #F9F9F9;
            --white: #FFFFFF;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light-color);
            color: var(--dark-color);
            line-height: 1.6;
        }
        
        header {
            background-color: var(--white);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            padding: 1.5rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary-color);
        }
        
        .logo span {
            color: var(--secondary-color);
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .hero {
            padding: 10rem 0 5rem;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            text-align: center;
        }
        
        h1 {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            color: var(--dark-color);
        }
        
        .subtitle {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto 2.5rem;
            color: #555;
        }
        
        .cta-button {
            display: inline-block;
            background-color: var(--primary-color);
            color: var(--white);
            padding: 0.8rem 2rem;
            font-size: 1rem;
            font-weight: 600;
            border-radius: 5px;
            text-decoration: none;
            transition: all 0.3s ease;
            margin-top: 1rem;
        }
        
        .cta-button:hover {
            background-color: #3367d6;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .chrome-badge {
            margin-top: 2rem;
            max-width: 200px;
        }
        
        .features {
            padding: 5rem 0;
            background-color: var(--white);
        }
        
        .section-title {
            text-align: center;
            font-size: 2.2rem;
            margin-bottom: 3rem;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            grid-gap: 2rem;
        }
        
        .feature-card {
            background-color: var(--light-color);
            border-radius: 10px;
            padding: 2rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
        }
        
        .feature-icon {
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
        }
        
        .feature-title {
            font-size: 1.4rem;
            margin-bottom: 1rem;
        }
        
        .how-it-works {
            padding: 5rem 0;
            background-color: var(--light-color);
        }
        
        .step-container {
            text-align: center;
            margin-bottom: 3rem;
        }
        
        .step-content {
            max-width: 600px;
            margin: 0 auto;
            padding: 0 2rem;
        }
        
        .step-number {
            font-size: 4rem;
            font-weight: 700;
            color: var(--primary-color);
            opacity: 0.2;
            margin-bottom: 1rem;
        }
        
        .step-title {
            font-size: 1.8rem;
            margin-bottom: 1rem;
        }
        
        .waitlist {
            padding: 5rem 0;
            background-color: var(--primary-color);
            color: var(--white);
            text-align: center;
        }
        
        .waitlist-title {
            font-size: 2.2rem;
            margin-bottom: 1.5rem;
        }
        
        .waitlist-subtitle {
            max-width: 600px;
            margin: 0 auto 2.5rem;
            font-size: 1.1rem;
        }
        
        .subscription-form {
            max-width: 500px;
            margin: 0 auto;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1rem;
        }
        
        .subscription-input {
            flex: 1;
            min-width: 200px;
            padding: 0.8rem 1rem;
            font-size: 1rem;
            border: none;
            border-radius: 5px;
        }
        
        .subscription-button {
            padding: 0.8rem 1.5rem;
            background-color: var(--secondary-color);
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .subscription-button:hover {
            background-color: #2d8f49;
        }
        
        footer {
            padding: 3rem 0;
            background-color: var(--dark-color);
            color: var(--white);
            text-align: center;
        }
        
        .footer-logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--white);
            margin-bottom: 1rem;
        }
        
        .footer-logo span {
            color: var(--secondary-color);
        }
        
        .footer-links {
            margin-bottom: 1.5rem;
        }
        
        .footer-links a {
            color: var(--white);
            margin: 0 1rem;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-links a:hover {
            color: var(--primary-color);
        }
        
        .copyright {
            font-size: 0.9rem;
            opacity: 0.7;
        }
        
        /* Mobile Responsiveness */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.2rem;
            }
            
            .subscription-form {
                flex-direction: column;
            }
            
            .subscription-input, .subscription-button {
                width: 100%;
            }
        }
    </style>
<script type="text/javascript" nonce="8fd1418b33f544d1aacd534ac50" src="//local.adguard.org?ts=1746296013173&amp;type=content-script&amp;dmn=mail-attachment.googleusercontent.com&amp;url=https%3A%2F%2Fmail-attachment.googleusercontent.com%2Fattachment%2Fu%2F0%2F%3Fui%3D2%26ik%3Dee1f0e19e7%26attid%3D0.1%26permmsgid%3Dmsg-a%3Ar-05%26th%3D196924321e06459b%26view%3Datt%26zw%26disp%3Dsafe%26saddbat%3DANGjdJ8_lwbupurDACho-58h3Rj0ucagBWe05g3JWcp99MlKN7RCCkmx4D9tLyvZYbvIz4IQrY5KbCzFWcvdg7PvzP_ObW6D0i27YducqMQkY4YPbEhM9agwagJhBTjxOB7E44uBv4nqVCXT7is-45XNswaJPPSJdjRfga50hhHiW9iBvH0-G2iv421L9nXYxAsBlzoTyWBYygEh3xD5jXze4Jf2IPCVkT_3sHYDyQkZsaSsmk6BYp_MpwR3bW3Q0RtkPuK4AS_QShGTRK4zDUoUBqg1V8gLeK2nFDvF7dpbevwocM6JxcUWc6NIEbThkJgNwFkv0VzWPmOFwPvXF2ICzP0hpRim-4PcSnGcDvEgHS5STJvTIF2fPuyEChehRQH7zR0OTFyw0uIKVtl6dbTAW_6p8hoByar_QSP5HL_Yw5gnUhvLn4ZsCR3gjAw6H0WHbpVMxIBKFvQtQe_LS6crdqksqlY2uFls-kwv4TV70CnC1IVXbbPX-NwOZNv3vPfs-1HKpzg_slVI-VQLYwR-kihhfwH7gajMqeRh0ySygu9JMd6T25UonzfHv9Eq9liExDTxKEDJimLBzzMLgMngfy3vkz1A6gz8jO5NaUiUoO1Zsngv01XFeeNcHLIXQiZLyASdWBI5qGOw_X7w3X9EBLP2EjnhNWT711LYQaynkZm08FW0tBH_539TXM_m-CxIgnybFRj5L7Lw3UWYqVHt52OdfJFrB__kWiguIWHK9hP2e77WlY-hjAvZvc2g6eOVDl6EoFazvc2j7pt2MCDaEPkRIMQcVXDr5uagxBqpSgrI3U_8oykvEwd-4yN6Ef9qV99wOLahEdlPtzzFsyqj5oyoGFWcP0NhRBiDx_92d-VuMKgMpULjbWYgNxgXx_l2klel0NFLIFJJAQ42Laq15b3sY7db_s0f58JLyL_XgUYWgKwnJNm3BImIQ5f0qETPJtnYeaROTXX0S5e-SHrkJWHPNICMy65SioByUxuH6PUVoukJ7pU0OFfaIOrJY50ffoRZw8Bg72sRrVpumKOOZDbcREUXiTO8KSnHew&amp;app=chrome.exe&amp;css=3&amp;js=1&amp;rel=1&amp;rji=1&amp;sbe=0&amp;stealth=1&amp;st-dnt"></script>
<script type="text/javascript" nonce="8fd1418b33f544d1aacd534ac50" src="//local.adguard.org?ts=1746296013173&amp;name=AdGuard%20Extra&amp;name=AdGuard%20Popup%20Blocker&amp;type=user-script"></script></head>
<body>
    <header>
        <div class="container">
            <nav>
                <div class="logo">Aprai<span>zrr</span></div>
            </nav>
        </div>
    </header>

    <section class="hero">
        <div class="container">
            <h1>Is That Facebook Marketplace Car Actually a Good Deal?</h1>
            <p class="subtitle">Stop second-guessing car listings. Apraizrr instantly shows you if that car is overpriced, a hidden gem, or potentially a scam—all while you browse Facebook Marketplace.</p>
            <a href="#waitlist" class="cta-button">Stop Overpaying for Cars</a>
            <div>
                <img src="/api/placeholder/200/60" alt="Coming soon to Chrome Web Store" class="chrome-badge">
            </div>
        </div>
    </section>

    <section class="features">
        <div class="container">
            <h2 class="section-title">Why Use Apraizrr?</h2>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">💰</div>
                    <h3 class="feature-title">Never Overpay Again</h3>
                    <p>Instantly see if a car is overpriced or a steal compared to similar models in your area. Know the fair value before messaging the seller.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">⚠️</div>
                    <h3 class="feature-title">Spot Red Flags & Scams</h3>
                    <p>Get immediate alerts about suspicious listings, potential odometer rollbacks, accident history, and other issues that sellers might not disclose.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">⏱️</div>
                    <h3 class="feature-title">Shop With Confidence</h3>
                    <p>Make informed decisions with all the vehicle data you need right on the listing page. No more endless research or driving to see cars that aren't worth your time.</p>
                </div>
            </div>
        </div>
    </section>

    <section class="how-it-works">
        <div class="container">
            <h2 class="section-title">How It Works</h2>
            
            <div class="step-container">
                <div class="step-content">
                    <div class="step-number">01</div>
                    <h3 class="step-title">Install Apraizrr (Takes 5 Seconds)</h3>
                    <p>Add the free extension to Chrome with one click. No account creation or complicated setup required.</p>
                </div>
            </div>
            
            <div class="step-container">
                <div class="step-content">
                    <div class="step-number">02</div>
                    <h3 class="step-title">Browse Cars on Facebook Marketplace</h3>
                    <p>Continue your car search as usual. Apraizrr works silently in the background without slowing down your browsing.</p>
                </div>
            </div>
            
            <div class="step-container">
                <div class="step-content">
                    <div class="step-number">03</div>
                    <h3 class="step-title">See What the Seller Isn't Telling You</h3>
                    <p>Apraizrr automatically reveals fair market value, price comparison, potential issues, and deal rating for each listing you view.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="waitlist" class="waitlist">
        <div class="container">
            <h2 class="waitlist-title">Don't Get Ripped Off On Your Next Car Purchase</h2>
            <p class="waitlist-subtitle">Join our waitlist to be the first to get Apraizrr when it launches. You'll also receive our exclusive guide on "5 Hidden Scams to Watch for on Facebook Marketplace Car Listings."</p>
            
            <form class="subscription-form">
                <input type="text" class="subscription-input" placeholder="Your Name">
                <input type="email" class="subscription-input" placeholder="Your Email">
                <button type="submit" class="subscription-button">Protect My Car Search</button>
            </form>
        </div>
    </section>

    <footer>
        <div class="container">
            <div class="footer-logo">Aprai<span>zrr</span></div>
            <div class="footer-links">
                <a href="#">Privacy Policy</a>
                <a href="#">Terms of Service</a>
                <a href="#">Contact Us</a>
            </div>
            <p class="copyright">© 2025 Apraizrr. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
