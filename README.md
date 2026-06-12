<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hair by Queen Liz | Premium Luxury Styling Atlanta</title>
    <meta name="description" content="Professional hair styling services in Atlanta. Book your luxury experience online with Hair by Queen Liz. Specializing in braids, installs, and natural hair treatment.">
    
    <style>
        /* --- DESIGN SYSTEM & CSS VARIABLES --- */
        :root {
            --primary: #0f0f1a;         /* Deep Rich Velvet Night */
            --primary-light: #1e1e2f;   /* Sleek Accent Dark */
            --accent: #e5c158;          /* Burnished Royalty Gold */
            --accent-hover: #c9a33b;    /* Deep Gold Shadow */
            --bg-light: #f6f6f9;        /* Clean Pearl Gray Base */
            --white: #ffffff;
            --text: #12121c;            /* Contrast Midnight */
            --text-muted: #6c757d;      /* Slate Gray Text */
            --border: #e2e8f0;          /* Modern Minimalist Border */
            --success: #10b981;         /* Emerald Status Green */
            --error: #ef4444;           /* Crimson Alert */
            --gold-gradient: linear-gradient(135deg, #f3d078 0%, #d4af37 50%, #aa7c11 100%);
            --dark-gradient: linear-gradient(135deg, #141423 0%, #08080f 100%);
            --glass: rgba(255, 255, 255, 0.85);
            --shadow-sm: 0 4px 6px -1px rgba(0,0,0,0.05);
            --shadow-md: 0 10px 15px -3px rgba(0,0,0,0.08), 0 4px 6px -2px rgba(0,0,0,0.04);
            --shadow-lg: 0 20px 25px -5px rgba(0,0,0,0.12), 0 10px 10px -5px rgba(0,0,0,0.04);
            --radius-sm: 8px;
            --radius-md: 16px;
            --radius-lg: 24px;
        }

        /* --- GLOBAL RESET & SCROLLBARS --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Cinzel', 'Playfair Display', 'Segoe UI', serif;
            letter-spacing: 0.3px;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg-light);
            color: var(--text);
            line-height: 1.7;
            font-size: 16px;
            padding-top: 80px;
            overflow-x: hidden;
        }

        /* Custom Scrollbar for Luxury Aesthetics */
        ::-webkit-scrollbar {
            width: 10px;
        }
        ::-webkit-scrollbar-track {
            background: var(--primary);
        }
        ::-webkit-scrollbar-thumb {
            background: var(--gold-gradient);
            border-radius: var(--radius-sm);
        }

        /* --- TYPOGRAPHY HIGHLIGHTS --- */
        h1, h2, h3, h4, .logo {
            font-family: 'Playfair Display', serif;
            font-weight: 700;
        }

        /* --- STICKY GLASSMORPHIC NAVIGATION --- */
        nav {
            background: var(--glass);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(226, 232, 240, 0.8);
            padding: 1.2rem 8%;
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: var(--shadow-sm);
        }

        .logo {
            font-size: 1.6rem;
            color: var(--primary);
            text-decoration: none;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-weight: 900;
            position: relative;
        }

        .logo span {
            color: var(--accent);
            background: var(--gold-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .nav-links {
            display: flex;
            gap: 2.5rem;
            list-style: none;
            align-items: center;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text);
            font-weight: 600;
            font-size: 0.95rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s ease;
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -4px;
            left: 0;
            background: var(--gold-gradient);
            transition: width 0.3s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .nav-links a:hover {
            color: var(--accent-hover);
        }

        .book-btn {
            background: var(--gold-gradient);
            color: var(--primary);
            padding: 0.75rem 2rem;
            border-radius: var(--radius-lg);
            font-weight: 700;
            font-size: 0.85rem;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            text-decoration: none;
            box-shadow: var(--shadow-md);
            transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
        }

        .book-btn:hover {
            transform: translateY(-3px) scale(1.02);
            box-shadow: 0 12px 20px rgba(212, 175, 55, 0.3);
        }

        /* --- HERO SPLASH SECTION WITH PARALLAX GLOW --- */
        .hero {
            background: linear-gradient(to right, rgba(15,15,26,0.95) 30%, rgba(15,15,26,0.4) 100%),
                        url('https://images.unsplash.com/photo-1560066984-138dadb629c2?w=1600') center/cover no-repeat;
            min-height: 90vh;
            display: flex;
            align-items: center;
            padding: 4rem 8%;
            color: var(--white);
            position: relative;
        }

        .hero::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 100px;
            background: linear-gradient(to top, var(--bg-light), transparent);
        }

        .hero-content {
            max-width: 700px;
            animation: fadeInUp 1s ease-out;
        }

        .hero-content h1 {
            font-size: 4.5rem;
            line-height: 1.1;
            margin-bottom: 1rem;
            text-transform: uppercase;
            letter-spacing: -1px;
        }

        .hero-tagline {
            font-size: 1.8rem;
            margin-bottom: 1.5rem;
            font-weight: 400;
            letter-spacing: 4px;
            text-transform: uppercase;
            background: var(--gold-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 2.5rem;
            opacity: 0.85;
            line-height: 1.8;
            font-family: 'Segoe UI', sans-serif;
        }

        .btn-primary {
            background: var(--gold-gradient);
            color: var(--primary);
            padding: 1.2rem 3rem;
            border-radius: var(--radius-lg);
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-size: 0.95rem;
            text-decoration: none;
            box-shadow: var(--shadow-lg);
            transition: all 0.4s ease;
            display: inline-block;
        }

        .btn-primary:hover {
            transform: translateY(-4px);
            box-shadow: 0 15px 30px rgba(229, 193, 88, 0.4);
        }

        /* --- FEATURE BANNER BAR --- */
        .features {
            background: var(--dark-gradient);
            padding: 3.5rem 8%;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 3rem;
            border-bottom: 4px solid var(--accent);
            box-shadow: var(--shadow-lg);
        }

        .feature {
            text-align: center;
            color: var(--white);
            transition: transform 0.3s ease;
        }

        .feature:hover {
            transform: translateY(-5px);
        }

        .feature-icon {
            font-size: 2.8rem;
            margin-bottom: 0.8rem;
            background: var(--gold-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .feature-title {
            font-weight: 700;
            font-size: 1.2rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 0.3rem;
        }

        .feature p {
            font-size: 0.9rem;
            color: #a0a0b0;
            font-family: 'Segoe UI', sans-serif;
        }

        /* --- STRUCTURAL SECTION SETUP --- */
        section {
            padding: 7rem 8%;
        }

        .section-title {
            text-align: center;
            margin-bottom: 4.5rem;
        }

        .section-title h2 {
            font-size: 3rem;
            color: var(--primary);
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-bottom: 0.8rem;
            position: relative;
            display: inline-block;
        }

        .section-title h2::after {
            content: '👑';
            position: absolute;
            font-size: 1.2rem;
            top: -25px;
            left: 50%;
            transform: translateX(-50%);
        }

        .section-title p {
            color: var(--text-muted);
            font-size: 1.2rem;
            font-family: 'Segoe UI', sans-serif;
            max-width: 600px;
            margin: 0 auto;
        }

        /* --- ABOUT EDITORIAL INTERFACE --- */
        .about {
            background: var(--white);
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1.2fr;
            gap: 5rem;
            max-width: 1200px;
            margin: 0 auto;
            align-items: center;
        }

        .about-img-frame {
            position: relative;
        }

        .about-img {
            width: 100%;
            height: 500px;
            background: var(--dark-gradient);
            border-radius: var(--radius-md);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: var(--accent);
            box-shadow: var(--shadow-lg);
            position: relative;
            z-index: 2;
            border: 1px solid rgba(229, 193, 88, 0.2);
        }

        .about-img-frame::before {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            border: 3px solid var(--accent);
            border-radius: var(--radius-md);
            top: 20px;
            left: -20px;
            z-index: 1;
        }

        .about-img .crown {
            font-size: 9rem;
            filter: drop-shadow(0 10px 15px rgba(0,0,0,0.5));
            animation: pulseGlow 3s infinite ease-in-out;
        }

        .about-content h3 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
        }

        .about-content p {
            color: var(--text-muted);
            margin-bottom: 1.5rem;
            font-family: 'Segoe UI', sans-serif;
            font-size: 1.05rem;
        }

        .policy-alert-box {
            background: #fffdf4;
            border: 1px solid #f1e4b8;
            border-left: 5px solid var(--accent);
            padding: 1.5rem;
            border-radius: var(--radius-sm);
            margin-top: 2rem;
        }

        /* --- SERVICE SELECTION CATALOG CARDS --- */
        .services {
            background: var(--bg-light);
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2.5rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .service-card {
            background: var(--white);
            border-radius: var(--radius-md);
            overflow: hidden;
            box-shadow: var(--shadow-sm);
            transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
            cursor: pointer;
            border: 2px solid transparent;
            display: flex;
            flex-direction: column;
        }

        .service-card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-lg);
            border-color: rgba(229, 193, 88, 0.4);
        }

        .service-card.selected {
            border-color: var(--accent);
            background: #fffef9;
            box-shadow: 0 0 0 4px rgba(229, 193, 88, 0.15), var(--shadow-lg);
        }

        .service-img {
            width: 100%;
            height: 180px;
            background: var(--dark-gradient);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4.5rem;
            position: relative;
        }

        .service-img::after {
            content: '';
            position: absolute;
            bottom: 0;
            width: 100%;
            height: 40px;
            background: linear-gradient(to top, rgba(0,0,0,0.2), transparent);
        }

        .service-content {
            padding: 2rem;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .service-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 0.5rem;
        }

        .service-content h4 {
            font-size: 1.4rem;
            color: var(--primary);
        }

        .service-price {
            background: var(--gold-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-size: 1.8rem;
            font-weight: 900;
        }

        .service-content p {
            color: var(--text-muted);
            font-size: 0.95rem;
            font-family: 'Segoe UI', sans-serif;
            margin-bottom: 1.5rem;
        }

        .service-meta {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-size: 0.85rem;
            font-weight: 700;
            color: var(--primary);
            text-transform: uppercase;
            border-top: 1px solid var(--border);
            padding-top: 1rem;
        }

        /* --- THE MASTER BOOKING SCHEDULER BOARD --- */
        .booking {
            background: var(--dark-gradient);
            padding: 8rem 5% 5rem;
            position: relative;
        }

        .booking .section-title h2 { color: var(--white); }
        .booking .section-title h2::after { content: '✨'; }
        .booking .section-title p { color: #a0a0b0; }

        .booking-container {
            max-width: 900px;
            margin: 0 auto;
            background: var(--white);
            border-radius: var(--radius-lg);
            overflow: hidden;
            color: var(--text);
            box-shadow: var(--shadow-lg);
        }

        .booking-header {
            background: var(--primary);
            color: var(--white);
            padding: 2rem;
            text-align: center;
            border-bottom: 3px solid var(--accent);
        }

        .booking-header h3 {
            font-size: 1.8rem;
            letter-spacing: 2px;
            text-transform: uppercase;
        }

        .booking-header p {
            color: #a0a0b0;
            font-family: 'Segoe UI', sans-serif;
            font-size: 0.95rem;
            margin-top: 0.3rem;
        }

        /* Pipeline Horizontal Steps Navigation */
        .booking-steps {
            display: flex;
            border-bottom: 1px solid var(--border);
            background: var(--bg-light);
        }

        .step {
            flex: 1;
            padding: 1.2rem 0.5rem;
            text-align: center;
            font-weight: 700;
            font-size: 0.85rem;
            color: var(--text-muted);
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s ease;
            position: relative;
        }

        .step.active {
            background: var(--white);
            color: var(--primary);
        }

        .step.active::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 3px;
            background: var(--gold-gradient);
        }

        .step.completed {
            color: var(--success);
        }

        .step-number {
            display: inline-block;
            width: 26px;
            height: 26px;
            background: var(--border);
            border-radius: 50%;
            line-height: 26px;
            font-size: 0.8------rem;
            margin-right: 0.5rem;
            color: var(--text);
            transition: all 0.3s ease;
        }

        .step.active .step-number {
            background: var(--primary);
            color: var(--accent);
        }

        .step.completed .step-number {
            background: var(--success);
            color: var(--white);
        }

        .booking-content {
            padding: 3rem;
            min-height: 420px;
        }

        .step-content {
            display: none;
        }

        .step-content.active {
            display: block;
            animation: slideInUp 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) forwards;
        }

        /* --- CALENDAR ENGINE CUSTOM INTERFACE --- */
        .date-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 2rem;
        }

        .month-year {
            font-size: 1.5rem;
            font-weight: 800;
            color: var(--primary);
            text-transform: uppercase;
        }

        .date-nav button {
            background: var(--white);
            border: 1px solid var(--border);
            width: 44px;
            height: 44px;
            border-radius: 50%;
            cursor: pointer;
            font-weight: bold;
            box-shadow: var(--shadow-sm);
            transition: all 0.2s ease;
        }

        .date-nav button:hover {
            background: var(--primary);
            color: var(--accent);
            border-color: var(--primary);
        }

        .calendar-grid {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            gap: 0.6rem;
            text-align: center;
        }

        .weekday {
            font-weight: 800;
            font-size: 0.85rem;
            color: var(--text-muted);
            text-transform: uppercase;
            padding-bottom: 0.8rem;
        }

        .day {
            padding: 1.1rem 0;
            font-weight: 600;
            border-radius: 12px;
            cursor: pointer;
            background: var(--bg-light);
            transition: all 0.2s ease;
            font-family: 'Segoe UI', sans-serif;
        }

        .day:hover:not(.disabled) {
            background: rgba(229, 193, 88, 0.25);
            transform: scale(1.05);
        }

        .day.selected {
            background: var(--gold-gradient) !important;
            color: var(--primary) !important;
            font-weight: 800;
            box-shadow: var(--shadow-md);
        }

        .day.disabled {
            opacity: 0.2;
            cursor: not-allowed;
            background: transparent;
        }

        /* Hourly System Slots Components */
        .time-selection {
            margin-top: 2.5rem;
            border-top: 1px dashed var(--border);
            padding-top: 2rem;
        }

        .time-selection h4 {
            text-transform: uppercase;
            font-size: 1.1rem;
            margin-bottom: 1.2rem;
            letter-spacing: 1px;
        }

        .time-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(115px, 1fr));
            gap: 0.8rem;
        }

        .time-slot {
            padding: 0.9rem;
            text-align: center;
            border: 2px solid var(--border);
            border-radius: var(--radius-sm);
            cursor: pointer;
            font-weight: 700;
            font-size: 0.85rem;
            background: var(--white);
            font-family: 'Segoe UI', sans-serif;
            transition: all 0.2s ease;
        }

        .time-slot:hover:not(.booked) {
            border-color: var(--accent);
            background: #fffdf5;
        }

        .time-slot.selected {
            background: var(--primary);
            color: var(--accent);
            border-color: var(--primary);
            box-shadow: var(--shadow-md);
        }

        .time-slot.booked {
            background: #f1f1f5;
            color: #cbd5e1;
            cursor: not-allowed;
            text-decoration: line-through;
            border-color: #f1f1f5;
        }

        /* --- FORM CONTROL SCHEMAS --- */
        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 700;
            font-size: 0.85rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .form-group input, .form-group textarea {
            width: 100%;
            padding: 1rem;
            border: 2px solid var(--border);
            border-radius: var(--radius-sm);
            font-size: 1rem;
            font-family: 'Segoe UI', sans-serif;
            transition: all 0.3s ease;
        }

        .form-group input:focus, .form-group textarea:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 4px rgba(15, 15, 26, 0.05);
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.5rem;
        }

        /* --- PAYMENT CHANNEL GRAPHICS --- */
        .payment-methods {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.5rem;
            margin: 1.2rem 0 2rem;
        }

        .payment-method {
            padding: 1.5rem;
            border: 2px solid var(--border);
            border-radius: var(--radius-md);
            text-align: center;
            cursor: pointer;
            transition: all 0.3s ease;
            background: var(--white);
        }

        .payment-method:hover {
            border-color: var(--accent);
            transform: translateY(-2px);
        }

        .payment-method.selected {
            border-color: var(--primary);
            background: rgba(15, 15, 26, 0.02);
            box-shadow: var(--shadow-md);
        }

        .payment-method-icon {
            font-size: 2.2rem;
            margin-bottom: 0.5rem;
        }

        .payment-method-name {
            font-weight: 800;
            text-transform: uppercase;
            font-size: 0.95rem;
        }

        .payment-details-box {
            background: #f8fafc;
            padding: 1.5rem;
            border-radius: var(--radius-sm);
            border-left: 4px solid var(--primary);
            margin-bottom: 2rem;
            display: none;
            animation: fadeIn 0.3s ease;
        }

        .crypto-address-container {
            display: flex;
            margin-top: 0.8rem;
            gap: 0.6rem;
        }

        .crypto-address-container input {
            flex: 1;
            padding: 0.75rem;
            border: 1px solid var(--border);
            border-radius: var(--radius-sm);
            font-size: 0.85rem;
            background: #edf2f7;
            font-family: monospace;
        }

        .copy-btn {
            background: var(--primary);
            color: var(--accent);
            border: none;
            padding: 0 1.5rem;
            border-radius: var(--radius-sm);
            cursor: pointer;
            font-size: 0.85rem;
            font-weight: 700;
            text-transform: uppercase;
            transition: all 0.2s;
        }

        .copy-btn:hover {
            background: var(--accent);
            color: var(--primary);
        }

        /* --- CONTROL FOOTER INTERFACE --- */
        .booking-footer {
            padding: 1.5rem 3rem;
            background: var(--bg-light);
            border-top: 1px solid var(--border);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .btn-control {
            padding: 1rem 2.5rem;
            border-radius: 30px;
            font-weight: 800;
            cursor: pointer;
            border: none;
            font-size: 0.85rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s ease;
        }

        .btn-back {
            background: #e2e8f0;
            color: var(--text);
        }

        .btn-back:hover { background: #cbd5e1; }

        .btn-next {
            background: var(--primary);
            color: var(--accent);
        }

        .btn-next:hover {
            background: var(--primary-light);
            transform: scale(1.02);
        }

        /* --- DYNAMIC RECEIPTS & PRINT VOUCHERS --- */
        .receipt-summary {
            background: #fafafa;
            border: 1px dashed var(--accent);
            padding: 2rem;
            border-radius: var(--radius-md);
            margin-bottom: 2rem;
        }

        .receipt-line {
            display: flex;
            justify-content: space-between;
            margin-bottom: 0.8rem;
            font-size: 1rem;
            font-family: 'Segoe UI', sans-serif;
        }

        .receipt-line.total {
            border-top: 2px solid var(--border);
            padding-top: 1rem;
            font-weight: 900;
            font-size: 1.3rem;
            color: var(--primary);
        }

        .success-screen {
            text-align: center;
            padding: 3rem 0;
        }

        .success-icon {
            font-size: 5rem;
            color: var(--success);
            margin-bottom: 1.5rem;
            animation: popScale 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        /* --- FOOTER FRAMEWORK --- */
        footer {
            background: var(--primary);
            color: var(--white);
            padding: 4rem 8% 2rem;
            text-align: center;
            border-top: 4px solid var(--accent);
        }

        /* --- ANIMATIONS TIMELINES --- */
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(40px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes slideInUp {
            from { opacity: 0; transform: translateY(15px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes pulseGlow {
            0%, 100% { transform: scale(1); filter: drop-shadow(0 10px 15px rgba(229,193,88,0.2)); }
            50% { transform: scale(1.03); filter: drop-shadow(0 15px 25px rgba(229,193,88,0.5)); }
        }
        @keyframes popScale {
            from { transform: scale(0.5); opacity: 0; }
            to { transform: scale(1); opacity: 1; }
        }

        /* --- ADAPTIVE RESPONSIVENESS CAPABILITIES --- */
        @media (max-width: 992px) {
            .about-grid { grid-template-columns: 1fr; gap: 4rem; }
            .about-img-frame { max-width: 500px; margin: 0 auto; }
            .hero-content h1 { font-size: 3.2rem; }
        }

        @media (max-width: 768px) {
            nav { padding: 1rem 5%; }
            .nav-links { display: none; }
            .form-row { grid-template-columns: 1fr; gap: 0; }
            .booking-content { padding: 1.5rem; }
            .booking-footer { padding: 1.5rem; }
            .time-grid { grid-template-columns: repeat(3, 1fr); }
        }
    </style>
    <!-- Google Fonts Resource Assets For Typography Elegance -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&display=swap" rel="stylesheet">
</head>
<body>

    <!-- STICKY HEADER GLASS NAVIGATION -->
    <nav>
        <a href="#" class="logo">👑 Queen <span>Liz</span></a>
        <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#booking">Book Now</a></li>
        </ul>
        <a href="#booking" class="book-btn">Schedule Session</a>
    </nav>

    <!-- INTRODUCTORY HERO SCENE DISPLAY -->
    <section class="hero">
        <div class="hero-content">
            <h1>HAIR BY QUEEN LIZ</h1>
            <div class="hero-tagline">Where Royalty Meets Style</div>
            <p>Experience protective luxury treatments, effortless trends, and precision hair braiding designs curated by Atlanta's premier styling technician.</p>
            <a href="#booking" class="btn-primary">View Available Slots</a>
        </div>
    </section>

    <!-- CORE BUSINESS FEATURES SEGMENT -->
    <div class="features">
        <div class="feature">
            <div class="feature-icon">✨</div>
            <div class="feature-title">Flawless Executions</div>
            <p>Premium lightweight partitions and crisp hairlines.</p>
        </div>
        <div class="feature">
            <div class="feature-icon">🔒</div>
            <div class="feature-title">Secure Deposits</div>
            <p>Direct verification protection system routing.</p>
        </div>
        <div class="feature">
            <div class="feature-icon">⚡</div>
            <div class="feature-title">Zero Wait Matrix</div>
            <p>Your scheduled deployment time is strictly maintained.</p>
        </div>
    </div>

    <!-- EDITORIAL BRAND STORY INTERFACE -->
    <section id="about" class="about">
        <div class="about-grid">
            <div class="about-img-frame">
                <div class="about-img">
                    <span class="crown">👑</span>
                    <p style="color: var(--accent); font-weight: 700; letter-spacing: 3px; margin-top:15px; font-size:1.1rem;">THE CROWN ARCHITECT</p>
                </div>
            </div>
            <div class="about-content">
                <h3>Meet Your Stylist</h3>
                <p>Welcome to the ultimate transformation salon station. I specialize in bringing out your natural inner majesty through masterfully mapped protective options, luxury flawless extensions, and intricate artistic crown braiding lines.</p>
                <p>By implementing targeted root health formulas combined with industry-leading integration techniques, your style is engineered to protect and catch glances simultaneously.</p>
                
                <div class="policy-alert-box">
                    <p style="font-weight:700; color: var(--primary); margin-bottom:0.4rem;">✨ Appointment Guidelines:</p>
                    <p style="font-size:0.9rem; color: var(--text-muted); margin:0;">• A flat-rate $25 security deposit is processed immediately to authorize your placement index slot.</p>
                    <p style="font-size:0.9rem; color: var(--text-muted); margin:0;">• Base natural hair matrix arrays must arrive completely washed and blown completely straight straight raw.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SERVICES COMPONENT INTEGRATION TARGET GRID -->
    <section id="services" class="services">
        <div class="section-title">
            <h2>Luxury USA Style Catalog</h2>
            <p>Select your signature style option below to unlock the booking pipeline scheduler</p>
        </div>
        <div class="services-grid" id="servicesGrid">
            <!-- Dynamic Injection Point for 15 Hairstyles -->
        </div>
    </section>

    <!-- INTERACTIVE CENTRAL BOOKING STEP MODULE WRAPPER -->
    <section id="booking" class="booking">
        <div class="booking-container">
            <div class="booking-header">
                <h3>HAIR BY QUEEN LIZ</h3>
                <p>Complete execution steps to receive verified confirmation voucher</p>
            </div>

            <!-- Steps Progress Node Tracks Header Bar -->
            <div class="booking-steps">
                <div class="step active" id="stepNode1"><span class="step-number">1</span>Service</div>
                <div class="step" id="stepNode2"><span class="step-number">2</span>DateTime</div>
                <div class="step" id="stepNode3"><span class="step-number">3</span>Details & Pay</div>
                <div class="step" id="stepNode4"><span class="step-number">4</span>Confirm</div>
            </div>

            <div class="booking-content">
                <!-- STEP CONTENT 1: SERVICE CONFIRM MATRIX VIEW -->
                <div class="step-content active" id="stepContent1">
                    <h3 style="margin-bottom: 1rem; font-size:1.6rem;">Confirm Selection Package</h3>
                    <p id="servicePromptText" style="color: var(--text-muted); margin-bottom: 1.5rem; font-family:'Segoe UI';">Please navigate into our Luxury Catalog above and select any hair styling card profile to mount execution attributes here.</p>
                    <div id="activeSelectionReceipt" style="display:none;" class="receipt-summary"></div>
                </div>

                <!-- STEP CONTENT 2: LIVE CALENDAR & HOURLY SLOTS MATRIX DISPLAY -->
                <div class="step-content" id="stepContent2">
                    <div class="date-header">
                        <div class="month-year" id="calendarMonthYearDisplay">June 2026</div>
                        <div class="date-nav">
                            <button type="button" onclick="adjustMonthPointer(-1)">◀️</button>
                            <button type="button" onclick="adjustMonthPointer(1)">▶️</button>
                        </div>
                    </div>
                    <div class="calendar-grid" id="calendarTargetGrid">
                        <!-- Internal Render Day Loops -->
                    </div>

                    <div class="time-selection" id="timeSelectionWrapper" style="display:none;">
                        <h4>Available Appointment Slots</h4>
                        <div class="time-grid" id="timeSlotsTargetGrid"></div>
                    </div>
                </div>

                <!-- STEP CONTENT 3: CLIENT DISPATCH FORM & DYNAMIC WALLET ROUTER -->
                <div class="step-content" id="stepContent3">
                    <form id="appointmentForm" onsubmit="event.preventDefault();">
                        <div class="form-row">
                            <div class="form-group">
                                <label for="clientFirstName">First Name *</label>
                                <input type="text" id="clientFirstName" required>
                            </div>
                            <div class="form-group">
                                <label for="clientLastName">Last Name *</label>
                                <input type="text" id="clientLastName" required>
                            </div>
                        </div>
                        <div class="form-row">
                            <div class="form-group">
                                <label for="clientEmail">Email Address *</label>
                                <input type="email" id="clientEmail" required>
                            </div>
                            <div class="form-group">
                                <label for="clientPhone">Mobile Phone Number *</label>
                                <input type="tel" id="clientPhone" placeholder="(404) 555-0199" required>
                            </div>
                        </div>
                        <div class="form-group">
                            <label for="clientNotes">Structural Notes / Custom Volume Extension Requests</label>
                            <textarea id="clientNotes" rows="3" placeholder="Describe current raw hair length characteristics, texture specifics, or lace brand preferences..."></textarea>
                        </div>

                        <!-- Payment Route Interface Elements Wrapper -->
                        <div style="margin-top:2.5rem;">
                            <h4 style="font-size:1.1rem; text-transform:uppercase;">Secure Booking Deposit Gateway</h4>
                            <p style="font-size:0.85rem; color: var(--text-muted); font-family:'Segoe UI';">A verified $25 security deposit must travel across checking routes below to authorize system ledger updates.</p>
                            
                            <div class="payment-methods">
                                <div class="payment-method" id="payMethodCashapp" onclick="setPaymentMethod('CashApp')">
                                    <div class="payment-method-icon">🟩</div>
                                    <div class="payment-method-name">CashApp</div>
                                </div>
                                <div class="payment-method" id="payMethodBitcoin" onclick="setPaymentMethod('Bitcoin')">
                                    <div class="payment-method-icon">₿</div>
                                    <div class="payment-method-name">Bitcoin Crypto</div>
                                </div>
                            </div>

                            <!-- Contextual Element Boxes Displays -->
                            <div class="payment-details-box" id="cashappDetailsBox">
                                <p style="font-weight:700; color:var(--primary);">CashApp Mobile Payment Dispatch Routing Target:</p>
                                <p style="font-size:1.05rem; margin-top:0.3rem; font-family:'Segoe UI';">Send manual funds allocation to tag link: <strong style="color:var(--success); font-size:1.15rem;">$HairByQueenLiz</strong></p>
                                <p style="font-size:0.75rem; color:var(--text-muted); margin-top:0.6rem;">⚠️ Include your name metrics string inside notes payload fields.</p>
                            </div>

                            <div class="payment-details-box" id="bitcoinDetailsBox">
                                <p style="font-weight:700; color:var(--primary);">Direct Network Bitcoin Ledger Wallet Node Target Index:</p>
                                <div class="crypto-address-container">
                                    <input type="text" id="btcAddressValue" value="bc1qxy2kgdygjrsqtzq2n0yrf2493p83kkfjhx0wlh" readonly>
                                    <button type="button" class="copy-btn" onclick="copyCryptoAddressText()">Copy Address</button>
                                </div>
                            </div>
                        </div>
                    </form>
                </div>

                <!-- STEP CONTENT 4: AUTO RENDER PRINT VOUCHER SHEET SYSTEM -->
                <div class="step-content" id="stepContent4">
                    <div class="success-screen">
                        <div class="success-icon">✓</div>
                        <h3 style="font-size:1.8rem; color: var(--primary); margin-bottom:0.5rem;">Voucher Allocation Cached</h3>
                        <p style="color:var(--text-muted); margin-bottom:2rem; max-width:550px; margin-left:auto; margin-right:auto; font-family:'Segoe UI';">
                            Your reservation has structural status clearance. Secure tracking parameters details are appended to printable transaction sheet manifest below.
                        </p>
                        <div id="finalConfirmationVoucherCard" class="receipt-summary" style="text-align: left;"></div>
                    </div>
                </div>
            </div>

            <!-- Global Pipeline Execution Controller Platform Footer -->
            <div class="booking-footer" id="bookingControlsFooter">
                <button type="button" class="btn-control btn-back" id="globalBackButton" onclick="navigatePipelineSteps(-1)" style="visibility: hidden;">Back</button>
                <button type="button" class="btn-control btn-next" id="globalNextButton" onclick="navigatePipelineSteps(1)">Continue Navigation</button>
            </div>
        </div>
    </section>

    <!-- MAIN BRAND FOOTER FRAME -->
    <footer>
        <p style="font-weight:900; color: var(--accent); margin-bottom: 0.5rem; letter-spacing:2px; font-size:1.2rem;">👑 HAIR BY QUEEN LIZ</p>
        <p style="font-size:0.85rem; opacity:0.6; font-family:'Segoe UI';">©️ 2026 Hair By Queen Liz Elite Salon Groups Inc. All Rights Reserved.</p>
        <p style="font-size:0.75rem; opacity:0.3; margin-top:1.5rem; font-family:'Segoe UI';">Atlanta Premium Hair Matrix Architecture & Network Deployment Solutions</p>
    </footer>

    <!-- LOGICAL DATA ENGINE PROCESSING SCRIPTS APPLICATION -->
    <script>
        // System Comprehensive USA Women Hairstyles Database
        const SERVICES_DATABASE = [
            { id: "srv_knotless", name: "Knotless Braids", price: 220, duration: "4.5 hrs", icon: "💇‍♀️", desc: "Premium lightweight feed-in variations. Flat, natural root profile causing near-zero tension on protective scalps." },
            { id: "srv_box", name: "Classic Box Braids", price: 195, duration: "4.0 hrs", icon: "✨", desc: "Timeless hair culture staple. Sectioned into ultra-clean geometric grids with synthetic extensions added for volume." },
            { id: "srv_cornrows", name: "Flat Cornrows Matrix", price: 120, duration: "2.0 hrs", icon: "👑", desc: "Narrow rows braided flat against the scalp. Perfect as a sleek standalone look or as a flat base under weaves and units." },
            { id: "srv_goddess", name: "Goddess Braids", price: 240, duration: "5.0 hrs", icon: "🦋", desc: "Intricate protective styles featuring cascading curly boho tendrils left loose throughout lengths and ends." },
            { id: "srv_fulani", name: "Fulani Braids Array", price: 180, duration: "3.5 hrs", icon: "🐚", desc: "Artistic traditional layout with a center cornrow, reversed side panels, and loose elements in the back." },
            { id: "srv_feedin", name: "Feed-In Cornrows", price: 140, duration: "2.5 hrs", icon: "⚡", desc: "Braids start ultra-thin along your hairline profile and widen naturally by gradually feeding extensions in." },
            { id: "srv_french", name: "Double French Braids", price: 75, duration: "1.0 hr", icon: "👱‍♀️", desc: "Classic overhand three-strand gathering layout. Great for active weeks, gym routines, and effortless styles." },
            { id: "srv_dutch", name: "Double Dutch Braids", price: 80, duration: "1.0 hr", icon: "🔥", desc: "Inverted 'inside-out' technique where braids sit dynamically raised above the crown layer lines." },
            { id: "srv_fishtail", name: "Bohemian Fishtail", price: 90, duration: "1.5 hrs", icon: "🌾", desc: "Two-strand intricate weaving pattern. Intentionally pancaked out for high-fashion, soft, messy wedding/prom aesthetics." },
            { id: "srv_lemonade", name: "Lemonade Side Cornrows", price: 160, duration: "3.0 hrs", icon: "🍋", desc: "Sleek, side-swept geometric cornrows flowing completely over one shoulder. High-impact structural statement look." },
            { id: "srv_crown", name: "Halo / Crown Braid", price: 110, duration: "1.5 hrs", icon: "😇", desc: "Elegant continuous weave pinned cleanly around the entire skull circumference to construct an regal halo frame." },
            { id: "srv_jumbo", name: "Jumbo Statement Braids", price: 130, duration: "1.5 hrs", icon: "💥", desc: "Oversized chunky box or cornrow paths. Fast installation profile for bold protection in minimal time frames." },
            { id: "srv_micro", name: "Ultra Fine Micro Braids", price: 350, duration: "7.0 hrs", icon: "🧵", desc: "Tiny thread-fine braids yielding free-flowing motion characteristics. Ultimate high-versatility luxury application." },
            { id: "srv_waterfall", name: "Waterfall Cascade Braid", price: 85, duration: "1.0 hr", icon: "💧", desc: "Modified half-up horizontal braid track that repeatedly drops loose hair strands through to form a cascade." },
            { id: "srv_bubble", name: "TikTok Trend Bubble Braids", price: 65, duration: "0.5 hrs", icon: "🫧", desc: "Segmented ponytail links wrapped at meticulous intervals to isolate puffy bubbles. Rapid Gen-Z styling option." }
        ];

        const CORE_HOURLY_SLOTS = ["09:00 AM", "11:30 AM", "02:00 PM", "04:30 PM", "07:00 PM"];

        // Master Architecture Application State Object
        let appState = {
            currentPipelineStep: 1,
            chosenService: null,
            chosenDate: null,
            chosenTimeSlot: null,
            chosenPaymentMethod: null,
            calendarYearPointer: 2026,
            calendarMonthPointer: 5 // Default tracking initial launch state focus onto June 2026
        };

        // DOM Document Attachment Inbound Engine Initialization Tasks
        window.addEventListener('DOMContentLoaded', () => {
            renderCatalogCards();
            initializeCalendarEngine();
        });

        // Loop arrays drawing interactive card structures inside target node layouts
        function renderCatalogCards() {
            const gridContainer = document.getElementById('servicesGrid');
            gridContainer.innerHTML = SERVICES_DATABASE.map(srv => `
                <div class="service-card" id="card_${srv.id}" onclick="selectServicePackage('${srv.id}')">
                    <div class="service-img">${srv.icon}</div>
                    <div class="service-content">
                        <div class="service-header">
                            <h4>${srv.name}</h4>
                            <div class="service-price">$${srv.price}</div>
                        </div>
                        <p>${srv.desc}</p>
                        <div class="service-meta">
                            <span>Duration Index</span>
                            <span>⏱ ${srv.duration}</span>
                        </div>
                    </div>
                </div>
            `).join('');
        }

        // Logic tracking internal configurations updates based on product selected
        function selectServicePackage(serviceId) {
            SERVICES_DATABASE.forEach(s => {
                const cardNode = document.getElementById(`card_${s.id}`);
                if(cardNode) cardNode.classList.remove('selected');
            });

            const currentActiveCard = document.getElementById(`card_${serviceId}`);
            if(currentActiveCard) currentActiveCard.classList.add('selected');

            appState.chosenService = SERVICES_DATABASE.find(x => x.id === serviceId);

            // Re-render internal receipt confirmation displays step 1 text zones
            document.getElementById('servicePromptText').style.display = 'none';
            const receiptDivBox = document.getElementById('activeSelectionReceipt');
            receiptDivBox.style.display = 'block';
            receiptDivBox.innerHTML = `
                <div class="receipt-line"><strong>Selected Profile:</strong> <span>${appState.chosenService.name}</span></div>
                <div class="receipt-line"><strong>Execution Run Window:</strong> <span>${appState.chosenService.duration}</span></div>
                <div class="receipt-line total"><strong>Price Evaluation:</strong> <span>$${appState.chosenService.price}</span></div>
            `;

            // Auto advance pipeline pointer tracking frame logic sequences
            setTimeout(() => { navigatePipelineSteps(1); }, 400);
        }

        // Calendar Algorithm Matrix Render Engine Tasks
        function initializeCalendarEngine() {
            const monthLabelsArray = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];
            document.getElementById('calendarMonthYearDisplay').innerText = `${monthLabelsArray[appState.calendarMonthPointer]} ${appState.calendarYearPointer}`;

            const gridContainerTarget = document.getElementById('calendarTargetGrid');
            gridContainerTarget.innerHTML = '';

            const dayPrefixLabels = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"];
            dayPrefixLabels.forEach(dStr => {
                const headDiv = document.createElement('div');
                headDiv.className = 'weekday';
                headDiv.innerText = dStr;
                gridContainerTarget.appendChild(headDiv);
            });

            let trackingIndexStartOffset = new Date(appState.calendarYearPointer, appState.calendarMonthPointer, 1).getDay();
            let calculationsMonthDaysCount = new Date(appState.calendarYearPointer, appState.calendarMonthPointer + 1, 0).getDate();

            for (let padIdx = 0; padIdx < trackingIndexStartOffset; padIdx++) {
                const dummyBlankNode = document.createElement('div');
                dummyBlankNode.className = 'day disabled';
                gridContainerTarget.appendChild(dummyBlankNode);
            }

            for (let computedDayNum = 1; computedDayNum <= calculationsMonthDaysCount; computedDayNum++) {
                const liveDayNode = document.createElement('div');
                liveDayNode.className = 'day';
                liveDayNode.innerText = computedDayNum;

                // Lock out past/unrealistic slots
                if(computedDayNum < 10 && appState.calendarMonthPointer === 5) {
                    liveDayNode.classList.add('disabled');
                } else {
                    liveDayNode.onclick = () => { registerDateStringTrackingCoordinate(liveDayNode, computedDayNum); };
                }

                if(appState.chosenDate && appState.chosenDate.day === computedDayNum && appState.chosenDate.month === appState.calendarMonthPointer) {
                    liveDayNode.classList.add('selected');
                }

                gridContainerTarget.appendChild(liveDayNode);
            }
        }

        function adjustMonthPointer(shiftMagnitudeValue) {
            appState.calendarMonthPointer += shiftMagnitudeValue;
            if(appState.calendarMonthPointer > 11) {
                appState.calendarMonthPointer = 0;
                appState.calendarYearPointer++;
            } else if (appState.calendarMonthPointer < 0) {
                appState.calendarMonthPointer = 11;
                appState.calendarYearPointer--;
            }
            initializeCalendarEngine();
        }

        function registerDateStringTrackingCoordinate(domReference, targetDayRawValue) {
            const checkAllDaysNodes = document.querySelectorAll('.calendar-grid .day');
            checkAllDaysNodes.forEach(d => d.classList.remove('selected'));

            domReference.classList.add('selected');
            appState.chosenDate = {
                day: targetDayRawValue,
                month: appState.calendarMonthPointer,
                year: appState.calendarYearPointer,
                stringRepresentation: `${appState.calendarMonthPointer + 1}/${targetDayRawValue}/${appState.calendarYearPointer}`
            };

            document.getElementById('timeSelectionWrapper').style.display = 'block';
            renderTimeGridSlots();
        }

        function renderTimeGridSlots() {
            const targetingContainer = document.getElementById('timeSlotsTargetGrid');
            targetingContainer.innerHTML = '';

            CORE_HOURLY_SLOTS.forEach((timeDisplayStr, internalIdx) => {
                const slotNodeElement = document.createElement('div');
                slotNodeElement.className = 'time-slot';
                slotNodeElement.innerText = timeDisplayStr;

                // Simulate historical collisions on random dates
                if(internalIdx === 1 && appState.chosenDate?.day % 3 === 0) {
                    slotNodeElement.classList.add('booked');
                } else {
                    slotNodeElement.onclick = () => {
                        const targetSiblingSlots = document.querySelectorAll('.time-grid .time-slot');
                        targetSiblingSlots.forEach(s => s.classList.remove('selected'));
                        slotNodeElement.classList.add('selected');
                        appState.chosenTimeSlot = timeDisplayStr;
                    };
                }

                if(appState.chosenTimeSlot === timeDisplayStr) {
                    slotNodeElement.classList.add('selected');
                }

                targetingContainer.appendChild(slotNodeElement);
            });
        }

        function setPaymentMethod(methodIdentifierStr) {
            document.getElementById('payMethodCashapp').classList.remove('selected');
            document.getElementById('payMethodBitcoin').classList.remove('selected');
            document.getElementById('cashappDetailsBox').style.display = 'none';
            document.getElementById('bitcoinDetailsBox').style.display = 'none';

            appState.chosenPaymentMethod = methodIdentifierStr;

            if(methodIdentifierStr === 'CashApp') {
                document.getElementById('payMethodCashapp').classList.add('selected');
                document.getElementById('cashappDetailsBox').style.display = 'block';
            } else if (methodIdentifierStr === 'Bitcoin') {
                document.getElementById('payMethodBitcoin').classList.add('selected');
                document.getElementById('bitcoinDetailsBox').style.display = 'block';
            }
        }

        function copyCryptoAddressText() {
            const targetInputElement = document.getElementById('btcAddressValue');
            targetInputElement.select();
            targetInputElement.setSelectionRange(0, 99999);
            navigator.clipboard.writeText(targetInputElement.value);
            alert("System Message: Bitcoin Address copied to local clipboard buffer memory!");
        }

        // Central Processing Unit Engine Navigation Matrix Route Switches
        function navigatePipelineSteps(navigationOffsetValue) {
            if(navigationOffsetValue === 1) {
                if(appState.currentPipelineStep === 1 && !appState.chosenService) {
                    alert("System Notice: Select a service catalog node styling design to engage validation parameters.");
                    return;
                }
                if(appState.currentPipelineStep === 2 && (!appState.chosenDate || !appState.chosenTimeSlot)) {
                    alert("System Notice: Core Calendar coordinates unfilled. Choose target appointment slot parameters layout.");
                    return;
                }
                if(appState.currentPipelineStep === 3) {
                    if(!document.getElementById('clientFirstName').value || 
                       !document.getElementById('clientLastName').value || 
                       !document.getElementById('clientEmail').value || 
                       !document.getElementById('clientPhone').value) {
                        alert("System Notice: Required input matrix attributes empty. Supply identity field attributes.");
                        return;
                    }
                    if(!appState.chosenPaymentMethod) {
                        alert("System Notice: Select deposit asset clearance line (CashApp or Bitcoin Wallet route nodes).");
                        return;
                    }
                    generateFinalVoucherSheetOutput();
                }
            }

            appState.currentPipelineStep += navigationOffsetValue;

            for (let currentLoopIdx = 1; currentLoopIdx <= 4; currentLoopIdx++) {
                const headerNodeRef = document.getElementById(`stepNode${currentLoopIdx}`);
                const pageContentRef = document.getElementById(`stepContent${currentLoopIdx}`);

                if(headerNodeRef) headerNodeRef.classList.remove('active', 'completed');
                if(pageContentRef) pageContentRef.classList.remove('active');

                if(currentLoopIdx < appState.currentPipelineStep) {
                    if(headerNodeRef) headerNodeRef.classList.add('completed');
                } else if(currentLoopIdx === appState.currentPipelineStep) {
                    if(headerNodeRef) headerNodeRef.classList.add('active');
                    if(pageContentRef) pageContentRef.classList.add('active');
                }
            }

            const backButtonRef = document.getElementById('globalBackButton');
            const nextButtonRef = document.getElementById('globalNextButton');

            backButtonRef.style.visibility = (appState.currentPipelineStep === 1 || appState.currentPipelineStep === 4) ? 'hidden' : 'visible';
            
            if(appState.currentPipelineStep === 3) {
                nextButtonRef.innerText = "Authorize & Finalize Booking";
            } else if (appState.currentPipelineStep === 4) {
                document.getElementById('bookingControlsFooter').style.display = 'none';
            } else {
                nextButtonRef.innerText = "Continue Navigation";
            }

            document.getElementById('booking').scrollIntoView();
        }

        // Compiles structural state cache logs translating into formal user receipts print cards HTML
        function generateFinalVoucherSheetOutput() {
            const fName = document.getElementById('clientFirstName').value;
            const lName = document.getElementById('clientLastName').value;
            const phone = document.getElementById('clientPhone').value;
            const noteText = document.getElementById('clientNotes').value || "No specialized texture instructions provided.";

            const outputContainerTarget = document.getElementById('finalConfirmationVoucherCard');
            outputContainerTarget.innerHTML = `
                <h4 style="text-align:center; color: var(--primary); border-bottom:2px dashed var(--accent); padding-bottom:0.8rem; margin-bottom:1.2rem; letter-spacing:1px; text-transform:uppercase;">OFFICIAL RESERVATION VOUCHER MANIFEST</h4>
                <div class="receipt-line"><strong>Client Name Target:</strong> <span>${fName} ${lName}</span></div>
                <div class="receipt-line"><strong>Secure Phone Interface:</strong> <span>${phone}</span></div>
                <div class="receipt-line"><strong>Selected Style Model:</strong> <span>${appState.chosenService.name}</span></div>
                <div class="receipt-line"><strong>Timeline Vectors Assignment:</strong> <span>${appState.chosenDate.stringRepresentation} @ ${appState.chosenTimeSlot}</span></div>
                <div class="receipt-line"><strong>Processing Deposit Route:</strong> <span>${appState.chosenPaymentMethod} Node Pipeline</span></div>
                <div class="receipt-line" style="flex-direction:column; margin-top:0.8rem; font-family:'Segoe UI';">
                    <strong>Patron Texture / Mapping Memos:</strong>
                    <span style="font-size:0.85rem; color:var(--text-muted); background:#fff; padding:0.8rem; border-radius:6px; margin-top:0.3rem; border:1px solid var(--border); line-height:1.5;">${noteText}</span>
                </div>
                <div class="receipt-line total" style="margin-top:1.5rem;"><strong>Outstanding Balance Due at Salon Chair:</strong> <span>$${appState.chosenService.price - 25}</span></div>
                <p style="font-size:0.75rem; color:var(--text-muted); text-align:center; margin-top:1.5rem; font-style:italic; border-top:1px solid var(--border); padding-top:0.8rem; font-family:'Segoe UI';">
                    Tracking Verification Hash Signature Code: QL-SYSTEM-RESERVE-${Math.floor(Math.random() * 900000 + 100000)}
                </p>
            `;
        }
    </script>
</body>
</html>
