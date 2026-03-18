<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kalpvriksha Legal & Environmental Solutions — Prayagraj</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --forest: #1a3a2a;
    --moss: #2d5a3d;
    --leaf: #4a8c5c;
    --sage: #8ab89a;
    --mist: #c8ddd0;
    --cream: #f5f0e8;
    --gold: #c9a84c;
    --gold-light: #e8c97a;
    --text-dark: #0f1f17;
    --text-mid: #2d4a38;
    --text-light: #6b8c78;
  }
  * { margin: 0; padding: 0; box-sizing: border-box; }
  html { scroll-behavior: smooth; }
  body { font-family: 'DM Sans', sans-serif; background: var(--cream); color: var(--text-dark); overflow-x: hidden; }

  /* NAV */
  nav {
    position: fixed; top: 0; width: 100%; z-index: 100;
    padding: 16px 60px;
    display: flex; justify-content: space-between; align-items: center;
    background: rgba(245,240,232,0.96); backdrop-filter: blur(12px);
    border-bottom: 1px solid rgba(74,140,92,0.15);
  }
  .nav-logo { font-family: 'Cormorant Garamond', serif; font-size: 20px; font-weight: 600; color: var(--forest); }
  .nav-logo span { color: var(--gold); }
  .nav-sub { font-size: 10px; letter-spacing: 1.5px; text-transform: uppercase; color: var(--text-light); display: block; margin-top: 2px; }
  .nav-links { display: flex; gap: 28px; list-style: none; align-items: center; }
  .nav-links a { font-size: 11px; font-weight: 500; letter-spacing: 1.5px; text-transform: uppercase; color: var(--text-mid); text-decoration: none; transition: color 0.3s; }
  .nav-links a:hover { color: var(--leaf); }
  .nav-cta { background: var(--forest) !important; color: var(--cream) !important; padding: 9px 22px; border-radius: 2px; }

  /* HERO */
  .hero { min-height: 100vh; display: grid; grid-template-columns: 1.1fr 0.9fr; }
  .hero-left { background: var(--forest); padding: 140px 60px 80px; display: flex; flex-direction: column; justify-content: center; position: relative; }
  .hero-left::after { content: ''; position: absolute; right: -40px; top: 0; bottom: 0; width: 80px; background: var(--forest); clip-path: polygon(0 0, 0 100%, 100% 100%); z-index: 2; }
  .hero-eyebrow { font-size: 11px; letter-spacing: 3px; text-transform: uppercase; color: var(--gold); margin-bottom: 20px; display: flex; align-items: center; gap: 12px; }
  .hero-eyebrow::before { content: ''; width: 40px; height: 1px; background: var(--gold); }
  .hero-title { font-family: 'Cormorant Garamond', serif; font-size: 60px; line-height: 1.05; color: var(--cream); font-weight: 300; margin-bottom: 10px; }
  .hero-title em { font-style: italic; color: var(--gold-light); display: block; }
  .hero-subtitle { font-size: 11px; letter-spacing: 2px; text-transform: uppercase; color: var(--sage); margin-bottom: 24px; margin-top: 6px; }
  .hero-desc { font-size: 14px; line-height: 1.9; color: var(--mist); max-width: 430px; margin-bottom: 32px; font-weight: 300; }
  .hero-badges { display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 36px; }
  .hero-badge { font-size: 10px; letter-spacing: 1px; border: 1px solid rgba(201,168,76,0.4); color: var(--gold-light); padding: 5px 13px; border-radius: 20px; }
  .hero-location { display: flex; align-items: center; gap: 8px; font-size: 12px; color: var(--sage); margin-bottom: 32px; }
  .hero-location::before { content: '📍'; font-size: 14px; }
  .hero-btn { display: inline-flex; align-items: center; gap: 10px; background: var(--gold); color: var(--forest); padding: 15px 32px; font-size: 11px; letter-spacing: 2px; text-transform: uppercase; font-weight: 500; text-decoration: none; border-radius: 2px; transition: all 0.3s; width: fit-content; }
  .hero-btn:hover { background: var(--gold-light); transform: translateX(4px); }

  .hero-right { background: var(--cream); display: flex; align-items: center; justify-content: center; padding: 80px 50px 80px 90px; }
  .hero-right-inner { width: 100%; }
  .tree-svg { width: 200px; height: 220px; display: block; margin: 0 auto 32px; }
  .hero-stats { display: grid; grid-template-columns: 1fr 1fr; gap: 18px; }
  .stat-box { border-left: 3px solid var(--gold); padding-left: 14px; }
  .stat-num { font-family: 'Cormorant Garamond', serif; font-size: 34px; font-weight: 600; color: var(--forest); line-height: 1; }
  .stat-label { font-size: 10px; letter-spacing: 1.5px; text-transform: uppercase; color: var(--text-light); margin-top: 3px; }

  /* IMPORTANT NOTICE BAR */
  .notice-bar {
    background: var(--gold); padding: 14px 60px;
    display: flex; align-items: center; justify-content: center; gap: 16px;
    flex-wrap: wrap;
  }
  .notice-bar-icon { font-size: 18px; }
  .notice-bar-text { font-size: 12px; font-weight: 500; letter-spacing: 0.5px; color: var(--forest); text-align: center; }
  .notice-bar-text strong { font-weight: 700; }

  /* TICKER */
  .ticker { background: var(--forest); padding: 11px 0; overflow: hidden; white-space: nowrap; }
  .ticker-inner { display: inline-block; animation: ticker 30s linear infinite; }
  .ticker-inner span { font-size: 10px; letter-spacing: 2px; text-transform: uppercase; font-weight: 500; color: var(--sage); padding: 0 36px; }
  .ticker-inner span::after { content: '◆'; margin-left: 36px; color: var(--gold); }
  @keyframes ticker { from { transform: translateX(0); } to { transform: translateX(-50%); } }

  /* SECTIONS */
  section { padding: 90px 60px; }
  .section-label { font-size: 11px; letter-spacing: 3px; text-transform: uppercase; color: var(--gold); margin-bottom: 14px; display: flex; align-items: center; gap: 12px; }
  .section-label::before { content: ''; width: 30px; height: 1px; background: var(--gold); }
  .section-title { font-family: 'Cormorant Garamond', serif; font-size: 46px; font-weight: 300; line-height: 1.1; color: var(--forest); margin-bottom: 20px; }
  .section-title em { font-style: italic; color: var(--leaf); }

  /* HOW WE WORK — MODEL */
  .model { background: var(--forest); }
  .model .section-title { color: var(--cream); }
  .model .section-label { color: var(--gold); }
  .model-desc { font-size: 14px; color: var(--mist); line-height: 1.8; max-width: 600px; margin-bottom: 50px; }
  .model-flow { display: grid; grid-template-columns: repeat(4, 1fr); gap: 2px; background: rgba(255,255,255,0.05); margin-bottom: 50px; }
  .flow-step { background: rgba(255,255,255,0.03); padding: 32px 24px; text-align: center; position: relative; }
  .flow-step::after { content: '→'; position: absolute; right: -14px; top: 50%; transform: translateY(-50%); color: var(--gold); font-size: 20px; z-index: 1; }
  .flow-step:last-child::after { display: none; }
  .flow-num { font-family: 'Cormorant Garamond', serif; font-size: 48px; font-weight: 300; color: rgba(201,168,76,0.2); line-height: 1; margin-bottom: 12px; }
  .flow-icon { font-size: 28px; margin-bottom: 12px; display: block; }
  .flow-title { font-size: 13px; font-weight: 500; letter-spacing: 1px; text-transform: uppercase; color: var(--gold); margin-bottom: 8px; }
  .flow-text { font-size: 12px; color: var(--mist); line-height: 1.6; }

  .model-boxes { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; }
  .model-box { border-radius: 3px; padding: 28px 28px; }
  .model-box.firm { background: rgba(201,168,76,0.12); border: 1px solid rgba(201,168,76,0.3); }
  .model-box.advocate { background: rgba(255,255,255,0.04); border: 1px solid rgba(255,255,255,0.1); }
  .model-box-title { font-size: 12px; letter-spacing: 2px; text-transform: uppercase; margin-bottom: 16px; font-weight: 500; }
  .model-box.firm .model-box-title { color: var(--gold); }
  .model-box.advocate .model-box-title { color: var(--sage); }
  .model-box-item { font-size: 13px; color: var(--mist); padding: 6px 0; border-bottom: 1px solid rgba(255,255,255,0.06); display: flex; align-items: center; gap: 8px; }
  .model-box-item::before { content: '✓'; flex-shrink: 0; }
  .model-box.firm .model-box-item::before { color: var(--gold); }
  .model-box.advocate .model-box-item::before { color: var(--sage); }
  .model-box-note { font-size: 11px; color: var(--text-light); margin-top: 14px; font-style: italic; }

  /* SERVICES */
  .services { background: var(--cream); }
  .services-intro { max-width: 600px; margin-bottom: 56px; }
  .services-intro p { font-size: 14px; color: var(--text-light); line-height: 1.8; }

  .service-category { margin-bottom: 56px; }
  .cat-header { display: flex; align-items: center; gap: 14px; margin-bottom: 20px; padding-bottom: 14px; border-bottom: 2px solid var(--mist); }
  .cat-icon { font-size: 26px; }
  .cat-title { font-family: 'Cormorant Garamond', serif; font-size: 26px; font-weight: 600; color: var(--forest); }
  .cat-count { font-size: 10px; letter-spacing: 2px; text-transform: uppercase; color: var(--text-light); margin-left: auto; }
  .cat-note { font-size: 11px; color: var(--leaf); margin-left: 8px; }

  .svc-row { display: grid; gap: 2px; background: var(--mist); }
  .svc-row.col4 { grid-template-columns: repeat(4,1fr); }
  .svc-row.col3 { grid-template-columns: repeat(3,1fr); }
  .svc-row.col2 { grid-template-columns: repeat(2,1fr); }

  .svc-card { background: var(--cream); padding: 26px 22px; position: relative; overflow: hidden; transition: all 0.35s; }
  .svc-card:hover { background: var(--forest); }
  .svc-card:hover .svc-title { color: var(--cream); }
  .svc-card:hover .svc-text { color: var(--mist); }
  .svc-card:hover .tag { border-color: rgba(138,184,154,0.4); color: var(--sage); }
  .svc-card::after { content: ''; position: absolute; bottom: 0; left: 0; right: 0; height: 2px; background: var(--gold); transform: scaleX(0); transform-origin: left; transition: transform 0.35s; }
  .svc-card:hover::after { transform: scaleX(1); }
  .svc-icon { font-size: 24px; margin-bottom: 12px; display: block; }
  .svc-title { font-family: 'Cormorant Garamond', serif; font-size: 19px; font-weight: 600; color: var(--forest); margin-bottom: 8px; line-height: 1.3; transition: color 0.35s; }
  .svc-text { font-size: 12px; line-height: 1.75; color: var(--text-light); transition: color 0.35s; }
  .svc-tags { margin-top: 12px; display: flex; flex-wrap: wrap; gap: 5px; }
  .tag { font-size: 9px; letter-spacing: 1px; text-transform: uppercase; padding: 3px 8px; border: 1px solid var(--sage); color: var(--text-light); border-radius: 20px; transition: all 0.35s; }

  /* REFER BOX */
  .refer-box {
    background: var(--forest); border-radius: 3px;
    padding: 28px 32px; margin-top: 14px;
    display: flex; align-items: center; gap: 20px;
    border-left: 4px solid var(--gold);
  }
  .refer-icon { font-size: 32px; flex-shrink: 0; }
  .refer-title { font-size: 12px; letter-spacing: 2px; text-transform: uppercase; color: var(--gold); margin-bottom: 6px; }
  .refer-text { font-size: 13px; color: var(--mist); line-height: 1.6; }

  /* ABOUT */
  .about { background: #f0ede4; display: grid; grid-template-columns: 1fr 1fr; gap: 70px; align-items: start; }
  .about-text { font-size: 14px; line-height: 1.9; color: var(--text-mid); margin-bottom: 16px; }
  .about-quote { background: var(--forest); border-left: 3px solid var(--gold); padding: 18px 22px; font-family: 'Cormorant Garamond', serif; font-size: 20px; font-style: italic; color: var(--gold-light); line-height: 1.6; margin: 28px 0; }
  .about-badges { display: flex; flex-direction: column; gap: 14px; }
  .about-badge { background: white; border: 1px solid var(--mist); border-radius: 3px; padding: 18px 20px; display: flex; align-items: flex-start; gap: 14px; transition: border-color 0.3s; }
  .about-badge:hover { border-color: var(--leaf); }
  .badge-icon { font-size: 22px; flex-shrink: 0; }
  .badge-title { font-size: 11px; font-weight: 500; letter-spacing: 1px; text-transform: uppercase; color: var(--forest); margin-bottom: 4px; }
  .badge-text { font-size: 12px; color: var(--text-light); line-height: 1.6; }

  /* PRICING */
  .pricing { background: var(--cream); }
  .pricing-intro { max-width: 560px; margin-bottom: 48px; }
  .pricing-intro p { font-size: 14px; color: var(--text-light); line-height: 1.8; }
  .pricing-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 18px; }
  .price-card { background: white; border: 1px solid var(--mist); border-radius: 3px; padding: 34px 28px; position: relative; transition: all 0.3s; }
  .price-card:hover { border-color: var(--leaf); transform: translateY(-4px); box-shadow: 0 16px 48px rgba(26,58,42,0.1); }
  .price-card.featured { background: var(--forest); border-color: var(--forest); }
  .price-card.featured .price-name, .price-card.featured .price-amount, .price-card.featured .price-per, .price-card.featured .price-desc { color: var(--cream); }
  .price-card.featured .price-feature { color: var(--mist); border-color: rgba(255,255,255,0.1); }
  .price-card.featured .price-feature::before { color: var(--gold); }
  .featured-badge { position: absolute; top: -11px; left: 50%; transform: translateX(-50%); background: var(--gold); color: var(--forest); font-size: 9px; letter-spacing: 2px; text-transform: uppercase; padding: 4px 16px; font-weight: 600; white-space: nowrap; }
  .price-name { font-size: 10px; letter-spacing: 2px; text-transform: uppercase; color: var(--text-light); margin-bottom: 18px; }
  .price-amount { font-family: 'Cormorant Garamond', serif; font-size: 46px; font-weight: 300; color: var(--forest); line-height: 1; }
  .price-per { font-size: 12px; color: var(--text-light); margin-bottom: 6px; }
  .price-desc { font-size: 12px; color: var(--text-light); margin-bottom: 22px; line-height: 1.6; }
  .price-divider { height: 1px; background: var(--mist); margin-bottom: 18px; }
  .price-feature { font-size: 12px; color: var(--text-mid); padding: 6px 0; border-bottom: 1px solid var(--mist); display: flex; align-items: center; gap: 8px; }
  .price-feature::before { content: '✓'; color: var(--leaf); font-weight: 700; flex-shrink: 0; }
  .price-btn { display: block; text-align: center; margin-top: 22px; padding: 12px; font-size: 11px; letter-spacing: 1.5px; text-transform: uppercase; font-weight: 500; text-decoration: none; border-radius: 2px; border: 1px solid var(--forest); color: var(--forest); transition: all 0.3s; }
  .price-btn:hover { background: var(--forest); color: var(--cream); }
  .price-card.featured .price-btn { background: var(--gold); border-color: var(--gold); color: var(--forest); }
  .price-note { font-size: 12px; color: var(--text-light); text-align: center; margin-top: 14px; }

  /* CONTACT */
  .contact { background: var(--forest); display: grid; grid-template-columns: 1fr 1fr; gap: 70px; align-items: start; }
  .contact .section-title { color: var(--cream); }
  .contact .section-label { color: var(--gold); }
  .contact-text { font-size: 14px; color: var(--mist); line-height: 1.9; font-weight: 300; margin-bottom: 32px; }
  .contact-item { display: flex; align-items: flex-start; gap: 14px; margin-bottom: 18px; padding-bottom: 18px; border-bottom: 1px solid rgba(255,255,255,0.07); }
  .c-icon { font-size: 18px; margin-top: 2px; }
  .c-label { font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: var(--gold); margin-bottom: 3px; }
  .c-val { font-size: 14px; color: var(--cream); }
  .whatsapp-btn { display: inline-flex; align-items: center; gap: 10px; background: #25D366; color: white; padding: 14px 28px; border-radius: 2px; text-decoration: none; font-size: 12px; letter-spacing: 1px; text-transform: uppercase; font-weight: 500; transition: all 0.3s; margin-top: 8px; }
  .whatsapp-btn:hover { background: #1ebe5d; transform: translateY(-2px); }

  .contact-form { display: flex; flex-direction: column; gap: 13px; }
  .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 13px; }
  .form-group { display: flex; flex-direction: column; gap: 6px; }
  .form-label { font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: var(--sage); }
  .form-input, .form-select, .form-textarea { background: rgba(255,255,255,0.06); border: 1px solid rgba(255,255,255,0.12); border-radius: 2px; padding: 12px 14px; font-size: 13px; color: var(--cream); font-family: 'DM Sans', sans-serif; outline: none; transition: border-color 0.3s; }
  .form-input::placeholder { color: rgba(200,221,208,0.4); }
  .form-input:focus, .form-select:focus, .form-textarea:focus { border-color: var(--gold); }
  .form-select option { background: var(--forest); }
  .form-textarea { resize: vertical; min-height: 100px; }
  .form-submit { background: var(--gold); color: var(--forest); border: none; padding: 14px 36px; font-size: 11px; letter-spacing: 2px; text-transform: uppercase; font-weight: 500; cursor: pointer; border-radius: 2px; font-family: 'DM Sans', sans-serif; transition: all 0.3s; width: fit-content; }
  .form-submit:hover { background: var(--gold-light); transform: translateY(-2px); }

  /* FOOTER */
  footer { background: var(--text-dark); padding: 32px 60px; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 12px; }
  .footer-logo { font-family: 'Cormorant Garamond', serif; font-size: 18px; color: var(--cream); }
  .footer-logo span { color: var(--gold); }
  .footer-mid { text-align: center; }
  .footer-text { font-size: 11px; color: var(--text-light); }
  .footer-disclaimer { font-size: 10px; color: rgba(107,140,120,0.6); margin-top: 4px; }
  .footer-tag { font-size: 10px; letter-spacing: 2px; text-transform: uppercase; color: var(--text-light); }

  /* ANIMATIONS */
  @keyframes fadeUp { from { opacity: 0; transform: translateY(28px); } to { opacity: 1; transform: translateY(0); } }
  .hero-left > * { animation: fadeUp 0.8s ease forwards; opacity: 0; }
  .hero-left > *:nth-child(1) { animation-delay: 0.2s; }
  .hero-left > *:nth-child(2) { animation-delay: 0.35s; }
  .hero-left > *:nth-child(3) { animation-delay: 0.45s; }
  .hero-left > *:nth-child(4) { animation-delay: 0.55s; }
  .hero-left > *:nth-child(5) { animation-delay: 0.65s; }
  .hero-left > *:nth-child(6) { animation-delay: 0.72s; }
  .hero-left > *:nth-child(7) { animation-delay: 0.8s; }

  @media (max-width: 900px) {
    nav { padding: 14px 20px; }
    .nav-links { display: none; }
    .hero { grid-template-columns: 1fr; }
    .hero-left::after { display: none; }
    .hero-left, .hero-right { padding: 80px 20px 40px; }
    .hero-title { font-size: 40px; }
    .notice-bar { padding: 12px 20px; }
    .model-flow, .model-boxes, .about, .contact { grid-template-columns: 1fr; }
    .svc-row.col4, .svc-row.col3, .svc-row.col2 { grid-template-columns: 1fr; }
    .pricing-grid { grid-template-columns: 1fr; }
    section { padding: 60px 20px; }
    footer { flex-direction: column; text-align: center; padding: 24px 20px; }
    .flow-step::after { display: none; }
  }
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="nav-logo">
    Kalpvriksha <span>⚖</span>
    <span class="nav-sub">Legal & Environmental Solutions · Prayagraj</span>
  </div>
  <ul class="nav-links">
    <li><a href="#how-we-work">How We Work</a></li>
    <li><a href="#services">Services</a></li>
    <li><a href="#pricing">Pricing</a></li>
    <li><a href="#contact" class="nav-cta">Free Consult</a></li>
  </ul>
</nav>

<!-- HERO -->
<section class="hero" id="home">
  <div class="hero-left">
    <div class="hero-eyebrow">Consulting · Compliance · Advisory — Prayagraj</div>
    <h1 class="hero-title">Aapki Har<em>Compliance Zaroorat</em></h1>
    <div class="hero-subtitle">Kalpvriksha Legal & Environmental Solutions</div>
    <p class="hero-desc">Environment clearance se lekar GST filing tak, STP plant se company registration tak — Prayagraj ka sabse comprehensive consulting firm. Hum consulting dete hain, aur litigation ke liye aapko Allahabad ke best advocates se connect karte hain.</p>
    <div class="hero-location">Prayagraj, Uttar Pradesh — Allahabad High Court Network ke saath</div>
    <div class="hero-badges">
      <span class="hero-badge">🌿 Environment Consulting</span>
      <span class="hero-badge">💧 STP/ETP O&M</span>
      <span class="hero-badge">🏢 Company Registration</span>
      <span class="hero-badge">📋 GST & Tax</span>
      <span class="hero-badge">♻️ Waste Management</span>
      <span class="hero-badge">⚖️ Advocate Network</span>
    </div>
    <a href="#contact" class="hero-btn">Free Consultation →</a>
  </div>
  <div class="hero-right">
    <div class="hero-right-inner">
      <svg class="tree-svg" viewBox="0 0 220 240" xmlns="http://www.w3.org/2000/svg">
        <ellipse cx="110" cy="225" rx="55" ry="7" fill="#2d5a3d" opacity="0.25"/>
        <path d="M103 225 Q101 195 104 172 Q107 155 110 148" stroke="#1a3a2a" stroke-width="10" fill="none" stroke-linecap="round"/>
        <path d="M117 225 Q119 195 116 172 Q113 155 110 148" stroke="#2d5a3d" stroke-width="7" fill="none" stroke-linecap="round"/>
        <path d="M110 165 Q85 150 68 130" stroke="#1a3a2a" stroke-width="5" fill="none" stroke-linecap="round"/>
        <path d="M110 162 Q132 147 148 128" stroke="#1a3a2a" stroke-width="5" fill="none" stroke-linecap="round"/>
        <path d="M108 178 Q88 167 75 155" stroke="#2d5a3d" stroke-width="3.5" fill="none" stroke-linecap="round"/>
        <path d="M112 176 Q130 164 142 152" stroke="#2d5a3d" stroke-width="3.5" fill="none" stroke-linecap="round"/>
        <circle cx="110" cy="92" r="56" fill="#2d5a3d" opacity="0.9"/>
        <circle cx="80" cy="80" r="40" fill="#4a8c5c" opacity="0.85"/>
        <circle cx="140" cy="80" r="40" fill="#4a8c5c" opacity="0.85"/>
        <circle cx="110" cy="65" r="44" fill="#1a3a2a" opacity="0.9"/>
        <circle cx="88" cy="58" r="32" fill="#4a8c5c" opacity="0.8"/>
        <circle cx="132" cy="58" r="32" fill="#4a8c5c" opacity="0.8"/>
        <circle cx="110" cy="42" r="36" fill="#2d5a3d"/>
        <circle cx="98" cy="36" r="5" fill="#c9a84c"/>
        <circle cx="122" cy="30" r="4" fill="#c9a84c"/>
        <circle cx="110" cy="22" r="6" fill="#e8c97a"/>
        <circle cx="83" cy="72" r="4" fill="#c9a84c"/>
        <circle cx="137" cy="68" r="4" fill="#c9a84c"/>
        <circle cx="110" cy="80" r="3" fill="#e8c97a"/>
        <line x1="110" y1="18" x2="94" y2="4" stroke="#e8c97a" stroke-width="1.5" opacity="0.45"/>
        <line x1="110" y1="18" x2="110" y2="2" stroke="#e8c97a" stroke-width="1.5" opacity="0.45"/>
        <line x1="110" y1="18" x2="126" y2="4" stroke="#e8c97a" stroke-width="1.5" opacity="0.45"/>
      </svg>
      <div class="hero-stats">
        <div class="stat-box"><div class="stat-num">25+</div><div class="stat-label">Services</div></div>
        <div class="stat-box"><div class="stat-num">100%</div><div class="stat-label">Consulting Only</div></div>
        <div class="stat-box"><div class="stat-num">AHC</div><div class="stat-label">Advocate Network</div></div>
        <div class="stat-box"><div class="stat-num">FREE</div><div class="stat-label">First Consult</div></div>
      </div>
    </div>
  </div>
</section>

<!-- NOTICE BAR -->
<div class="notice-bar">
  <span class="notice-bar-icon">ℹ️</span>
  <p class="notice-bar-text">
    <strong>Hum sirf Consulting & Advisory services dete hain.</strong> Court ya tribunal mein representation ke liye hum aapko Allahabad ke trusted advocates se connect karte hain.
  </p>
</div>

<!-- TICKER -->
<div class="ticker">
  <div class="ticker-inner">
    <span>Environment Consulting</span><span>GST Filing</span><span>Company Registration</span><span>STP/ETP O&M</span><span>Waste Management</span><span>CPCB Compliance</span><span>Advocate Referral</span><span>Environmental Clearance</span><span>ITR Filing</span><span>MSME Registration</span><span>Environment Consulting</span><span>GST Filing</span><span>Company Registration</span><span>STP/ETP O&M</span><span>Waste Management</span><span>CPCB Compliance</span><span>Advocate Referral</span><span>Environmental Clearance</span><span>ITR Filing</span><span>MSME Registration</span>
  </div>
</div>

<!-- HOW WE WORK -->
<section class="model" id="how-we-work">
  <div class="section-label">Our Model</div>
  <h2 class="section-title">Hum Kaise <em>Kaam Karte Hain</em></h2>
  <p class="model-desc">Kalpvriksha ek pure consulting firm hai — hum aapke saare compliance, documentation, registration, aur advisory kaam karte hain. Agar kabhi court ya tribunal jaana pade, hum aapko Allahabad ke trusted advocates se directly connect karte hain.</p>

  <div class="model-flow">
    <div class="flow-step">
      <div class="flow-num">01</div>
      <span class="flow-icon">📞</span>
      <div class="flow-title">Aap Call Karo</div>
      <p class="flow-text">WhatsApp ya call — apni problem batao. Pehli baat bilkul free hai.</p>
    </div>
    <div class="flow-step">
      <div class="flow-num">02</div>
      <span class="flow-icon">🔍</span>
      <div class="flow-title">Hum Assess Karte Hain</div>
      <p class="flow-text">Aapki situation review — kya consulting se solve hoga, kya advocate chahiye.</p>
    </div>
    <div class="flow-step">
      <div class="flow-num">03</div>
      <span class="flow-icon">⚙️</span>
      <div class="flow-title">Hum Kaam Karte Hain</div>
      <p class="flow-text">Documents, applications, filings, compliance — sab hum handle karte hain.</p>
    </div>
    <div class="flow-step">
      <div class="flow-num">04</div>
      <span class="flow-icon">⚖️</span>
      <div class="flow-title">Agar Court Chahiye</div>
      <p class="flow-text">Allahabad High Court ya NGT ke trusted advocate se seedha connect karte hain.</p>
    </div>
  </div>

  <div class="model-boxes">
    <div class="model-box firm">
      <div class="model-box-title">✅ Kalpvriksha Karta Hai</div>
      <div class="model-box-item">Environment Consent (CTE/CTO) Application</div>
      <div class="model-box-item">CPCB / HSPCB Compliance Documents</div>
      <div class="model-box-item">Environmental Clearance (EC/EIA) Filing</div>
      <div class="model-box-item">Waste Management Authorization</div>
      <div class="model-box-item">STP/ETP Operation & Maintenance</div>
      <div class="model-box-item">Company / LLP / MSME Registration</div>
      <div class="model-box-item">GST Registration & Return Filing</div>
      <div class="model-box-item">ITR, TDS/TCS Compliance</div>
      <div class="model-box-item">Notice Reply Drafting (Non-Court)</div>
      <div class="model-box-note">* Saari services consulting & documentation basis par</div>
    </div>
    <div class="model-box advocate">
      <div class="model-box-title">🤝 Advocate Se Connect Karte Hain</div>
      <div class="model-box-item">Allahabad High Court Cases</div>
      <div class="model-box-item">NGT (National Green Tribunal) Matters</div>
      <div class="model-box-item">Civil / Criminal Litigation</div>
      <div class="model-box-item">GST Tribunal Appearances</div>
      <div class="model-box-item">Any Court Representation</div>
      <div class="model-box-item">Writ Petitions</div>
      <div class="model-box-note">* Hum trusted Allahabad advocates se aapka seedha contact karate hain — aapko dhundhna nahi padta</div>
    </div>
  </div>
</section>

<!-- SERVICES -->
<section class="services" id="services">
  <div class="services-intro">
    <div class="section-label">Our Services</div>
    <h2 class="section-title">25+ Services, <em>Ek Jagah</em></h2>
    <p>Environment consulting se lekar taxation tak — Prayagraj aur poore UP ki industries, businesses aur individuals ke liye complete consulting solutions.</p>
  </div>

  <!-- ENV CONSENT -->
  <div class="service-category">
    <div class="cat-header">
      <span class="cat-icon">🌿</span>
      <div class="cat-title">Environment Consent & Clearance</div>
      <div class="cat-count">7 Services</div>
    </div>
    <div class="svc-row col4">
      <div class="svc-card"><span class="svc-icon">📝</span><div class="svc-title">Consent to Establish (CTE)</div><p class="svc-text">Nayi factory ke liye UPPCB se CTE — application se approval tak poora kaam hum karte hain.</p><div class="svc-tags"><span class="tag">UPPCB</span><span class="tag">New Unit</span></div></div>
      <div class="svc-card"><span class="svc-icon">✅</span><div class="svc-title">Consent to Operate (CTO)</div><p class="svc-text">CTO renewal aur fresh application — timely filing taaki aapka plant kabhi band na ho.</p><div class="svc-tags"><span class="tag">CTO Renewal</span><span class="tag">UPPCB</span></div></div>
      <div class="svc-card"><span class="svc-icon">🌲</span><div class="svc-title">Environmental Clearance (EC)</div><p class="svc-text">MoEFCC se EC application, EIA report, public hearing — expansion projects ke liye complete support.</p><div class="svc-tags"><span class="tag">MoEFCC</span><span class="tag">EIA</span></div></div>
      <div class="svc-card"><span class="svc-icon">🏭</span><div class="svc-title">Air / Water / Noise NOC</div><p class="svc-text">Specific pollution NOCs — complete documentation aur UPPCB submission.</p><div class="svc-tags"><span class="tag">Air Act</span><span class="tag">Water Act</span></div></div>
    </div>
    <div class="svc-row col3" style="margin-top:2px;">
      <div class="svc-card"><span class="svc-icon">🔬</span><div class="svc-title">EIA Report Preparation</div><p class="svc-text">Environmental Impact Assessment report — baseline data, impact analysis, mitigation measures.</p><div class="svc-tags"><span class="tag">EIA</span><span class="tag">Baseline</span></div></div>
      <div class="svc-card"><span class="svc-icon">🛡️</span><div class="svc-title">Environmental Audit</div><p class="svc-text">Factory ka pre-inspection audit — compliance gaps identify karo authorities se pehle.</p><div class="svc-tags"><span class="tag">Risk Audit</span><span class="tag">Compliance</span></div></div>
      <div class="svc-card"><span class="svc-icon">📊</span><div class="svc-title">Annual Environment Statement</div><p class="svc-text">Mandatory AES filing — every year timely submission, koi penalty nahi.</p><div class="svc-tags"><span class="tag">AES</span><span class="tag">Annual</span></div></div>
    </div>
    <div class="refer-box">
      <span class="refer-icon">⚖️</span>
      <div>
        <div class="refer-title">UPPCB / NGT Notice mila? Court jaana hai?</div>
        <p class="refer-text">Notice ka reply hum draft karte hain. Agar matter court ya NGT tak jaata hai — hum aapko Allahabad ke experienced advocate se seedha connect karte hain. Aapko kuch dhundhna nahi padta.</p>
      </div>
    </div>
  </div>

  <!-- WASTE -->
  <div class="service-category">
    <div class="cat-header">
      <span class="cat-icon">♻️</span>
      <div class="cat-title">Waste Management Compliance</div>
      <div class="cat-count">5 Services</div>
    </div>
    <div class="svc-row col3">
      <div class="svc-card"><span class="svc-icon">☣️</span><div class="svc-title">Hazardous Waste Authorization</div><p class="svc-text">HWM Rules 2016 ke under authorization, manifest system, annual returns — complete HW compliance.</p><div class="svc-tags"><span class="tag">HWM Rules</span><span class="tag">Authorization</span></div></div>
      <div class="svc-card"><span class="svc-icon">🏗️</span><div class="svc-title">Solid Waste Management</div><p class="svc-text">SWM Rules compliance, waste audit documentation — industries aur commercial establishments ke liye.</p><div class="svc-tags"><span class="tag">SWM Rules</span><span class="tag">Waste Audit</span></div></div>
      <div class="svc-card"><span class="svc-icon">🧪</span><div class="svc-title">Biomedical Waste Compliance</div><p class="svc-text">BMW Rules 2016 — hospitals, clinics ke liye authorization, records, training documentation.</p><div class="svc-tags"><span class="tag">BMW Rules</span><span class="tag">Hospitals</span></div></div>
    </div>
    <div class="svc-row col2" style="margin-top:2px;">
      <div class="svc-card"><span class="svc-icon">🔋</span><div class="svc-title">E-Waste EPR Registration</div><p class="svc-text">E-Waste Rules 2022 — CPCB portal par EPR registration, authorized recycler tie-up advisory.</p><div class="svc-tags"><span class="tag">E-Waste</span><span class="tag">EPR</span></div></div>
      <div class="svc-card"><span class="svc-icon">🏭</span><div class="svc-title">Plastic Waste / EPR Portal</div><p class="svc-text">Plastic packaging producers, importers — CPCB EPR portal registration aur annual compliance.</p><div class="svc-tags"><span class="tag">Plastic Rules</span><span class="tag">EPR Portal</span></div></div>
    </div>
  </div>

  <!-- STP/ETP -->
  <div class="service-category">
    <div class="cat-header">
      <span class="cat-icon">💧</span>
      <div class="cat-title">STP / ETP Operation & Maintenance</div>
      <div class="cat-count">4 Services</div>
    </div>
    <div class="svc-row col4">
      <div class="svc-card"><span class="svc-icon">⚙️</span><div class="svc-title">STP/ETP O&M Contract</div><p class="svc-text">Monthly Operation & Maintenance — actual Chemical Engineer dwara. Plant performance guarantee.</p><div class="svc-tags"><span class="tag">O&M</span><span class="tag">Monthly</span></div></div>
      <div class="svc-card"><span class="svc-icon">🔍</span><div class="svc-title">Technical Audit</div><p class="svc-text">Plant efficiency check, issue identification, CPCB discharge standards ke liye upgrade recommendations.</p><div class="svc-tags"><span class="tag">Tech Audit</span><span class="tag">Performance</span></div></div>
      <div class="svc-card"><span class="svc-icon">📈</span><div class="svc-title">ZLD Compliance Advisory</div><p class="svc-text">Zero Liquid Discharge planning — CPCB mandated ZLD achieve karne ke liye step-by-step guidance.</p><div class="svc-tags"><span class="tag">ZLD</span><span class="tag">CPCB</span></div></div>
      <div class="svc-card"><span class="svc-icon">📋</span><div class="svc-title">Effluent Testing & Reporting</div><p class="svc-text">NABL lab coordination, results interpretation, compliance report preparation aur submission.</p><div class="svc-tags"><span class="tag">NABL</span><span class="tag">Testing</span></div></div>
    </div>
  </div>

  <!-- COMPANY REG -->
  <div class="service-category">
    <div class="cat-header">
      <span class="cat-icon">🏢</span>
      <div class="cat-title">Business & Company Registration</div>
      <div class="cat-count">5 Services</div>
    </div>
    <div class="svc-row col3">
      <div class="svc-card"><span class="svc-icon">🏢</span><div class="svc-title">Private Limited Company</div><p class="svc-text">MCA portal par Pvt Ltd registration — DIN, DSC, MOA, AOA, Certificate of Incorporation.</p><div class="svc-tags"><span class="tag">MCA</span><span class="tag">Pvt Ltd</span></div></div>
      <div class="svc-card"><span class="svc-icon">🤝</span><div class="svc-title">LLP Registration</div><p class="svc-text">Limited Liability Partnership — professionals aur small businesses ke liye, low compliance structure.</p><div class="svc-tags"><span class="tag">LLP</span><span class="tag">MCA</span></div></div>
      <div class="svc-card"><span class="svc-icon">👤</span><div class="svc-title">Proprietorship / Partnership</div><p class="svc-text">Shop Act, trade licence, partnership deed drafting — small business complete setup.</p><div class="svc-tags"><span class="tag">Shop Act</span><span class="tag">Trade Licence</span></div></div>
    </div>
    <div class="svc-row col2" style="margin-top:2px;">
      <div class="svc-card"><span class="svc-icon">🌱</span><div class="svc-title">MSME / Startup India Registration</div><p class="svc-text">Udyam MSME, DPIIT Startup recognition — government schemes, subsidies, tax benefits unlock karo.</p><div class="svc-tags"><span class="tag">Udyam</span><span class="tag">DPIIT</span><span class="tag">MSME</span></div></div>
      <div class="svc-card"><span class="svc-icon">📑</span><div class="svc-title">IEC / FSSAI / Trade Licence</div><p class="svc-text">Import Export Code, FSSAI food licence, municipal trade licence — sab ek jagah.</p><div class="svc-tags"><span class="tag">IEC</span><span class="tag">FSSAI</span></div></div>
    </div>
  </div>

  <!-- GST -->
  <div class="service-category">
    <div class="cat-header">
      <span class="cat-icon">📋</span>
      <div class="cat-title">GST & Taxation Services</div>
      <div class="cat-count">5 Services</div>
    </div>
    <div class="svc-row col3">
      <div class="svc-card"><span class="svc-icon">📝</span><div class="svc-title">GST Registration</div><p class="svc-text">New GST registration, amendments, additional place of business — quick processing.</p><div class="svc-tags"><span class="tag">GSTN</span><span class="tag">New Reg</span></div></div>
      <div class="svc-card"><span class="svc-icon">🗓️</span><div class="svc-title">GST Return Filing</div><p class="svc-text">Monthly/quarterly GSTR-1, GSTR-3B, GSTR-9 annual return — timely, zero penalty.</p><div class="svc-tags"><span class="tag">GSTR-1</span><span class="tag">GSTR-3B</span></div></div>
      <div class="svc-card"><span class="svc-icon">🔎</span><div class="svc-title">GST Notice Reply</div><p class="svc-text">GST department notice aaya? Hum legally sound reply draft karte hain — tribunal ke liye advocate se connect.</p><div class="svc-tags"><span class="tag">Notice Reply</span><span class="tag">Draft</span></div></div>
    </div>
    <div class="svc-row col2" style="margin-top:2px;">
      <div class="svc-card"><span class="svc-icon">💰</span><div class="svc-title">Income Tax Return (ITR)</div><p class="svc-text">Individuals, firms, companies — ITR filing with proper tax planning.</p><div class="svc-tags"><span class="tag">ITR</span><span class="tag">Tax Planning</span></div></div>
      <div class="svc-card"><span class="svc-icon">📊</span><div class="svc-title">TDS / TCS Compliance</div><p class="svc-text">TDS deduction, challan payment, 24Q/26Q quarterly returns — complete TDS management.</p><div class="svc-tags"><span class="tag">TDS</span><span class="tag">26Q/24Q</span></div></div>
    </div>
  </div>

</section>

<!-- ABOUT -->
<section class="about" id="about">
  <div>
    <div class="section-label">About Us</div>
    <h2 class="section-title">Prayagraj Ka <em>Unique</em> Consulting Firm</h2>
    <p class="about-text">Kalpvriksha Legal & Environmental Solutions Prayagraj mein based ek pure consulting firm hai. Hamare paas Chemical Engineering background hai — matlab hum sirf documents nahi banate, hum aapki factory ki actual problems bhi samajhte hain.</p>
    <p class="about-text">Hum court nahi jaate — lekin agar aapko litigation ki zaroorat hai, toh hum Allahabad High Court ke trusted advocates se aapka seedha connection karate hain. Aapko kuch dhundhna nahi padta.</p>
    <div class="about-quote">"Consulting mein hum hain, court mein hamare network hain — aap sirf apna kaam karo."</div>
    <p class="about-text">Prayagraj — Allahabad High Court ki city — India ka ek important legal hub. Yahan industries, businesses, aur hospitals sabko compliance ki zaroorat hai. Hum unka bharosemand partner hain.</p>
  </div>
  <div class="about-badges">
    <div class="about-badge"><span class="badge-icon">⚗️</span><div><div class="badge-title">Chemical Engineering Background</div><div class="badge-text">STP plant ka real experience — documents ke saath technical reality bhi samajhte hain.</div></div></div>
    <div class="about-badge"><span class="badge-icon">📍</span><div><div class="badge-title">Prayagraj Based</div><div class="badge-text">UP ki industries ko locally serve karte hain — UPPCB, MoEFCC UP office ka poora knowledge.</div></div></div>
    <div class="about-badge"><span class="badge-icon">⚖️</span><div><div class="badge-title">Allahabad Advocate Network</div><div class="badge-text">High Court aur NGT ke liye trusted advocates ready — aapko sirf ek call karna hai humein.</div></div></div>
    <div class="about-badge"><span class="badge-icon">💼</span><div><div class="badge-title">Ek Jagah, Sab Kuch</div><div class="badge-text">Environment, GST, company registration, waste management — sab ek hi firm se.</div></div></div>
    <div class="about-badge"><span class="badge-icon">🌿</span><div><div class="badge-title">Kalpvriksha Ka Vaada</div><div class="badge-text">Kalpvriksha — jo har wish poori kare. Aapki har compliance zaroorat yahan poori hogi.</div></div></div>
  </div>
</section>

<!-- PRICING -->
<section class="pricing" id="pricing">
  <div class="pricing-intro">
    <div class="section-label">Pricing</div>
    <h2 class="section-title">Simple, <em>Transparent</em> Fees</h2>
    <p>Koi hidden charges nahi. Retainer lo ya individual service lo — dono options available hain.</p>
  </div>
  <div class="pricing-grid">
    <div class="price-card">
      <div class="price-name">Basic — Small Business</div>
      <div class="price-amount">₹5,000</div>
      <div class="price-per">/month retainer</div>
      <div class="price-desc">Proprietorship, small shop, clinic, startup ke liye.</div>
      <div class="price-divider"></div>
      <div class="price-feature">GST Return Filing</div>
      <div class="price-feature">1 Compliance Service/Month</div>
      <div class="price-feature">Business Registration Help</div>
      <div class="price-feature">WhatsApp Support</div>
      <a href="#contact" class="price-btn">Get Started</a>
    </div>
    <div class="price-card featured">
      <div class="featured-badge">Most Popular</div>
      <div class="price-name">Standard — Medium Industry</div>
      <div class="price-amount">₹20,000</div>
      <div class="price-per">/month retainer</div>
      <div class="price-desc">Mid-size factory — full environment + GST + registration cover.</div>
      <div class="price-divider"></div>
      <div class="price-feature">Everything in Basic</div>
      <div class="price-feature">UPPCB Consent Management</div>
      <div class="price-feature">Quarterly Env. Audit</div>
      <div class="price-feature">GST + ITR Filing</div>
      <div class="price-feature">Advocate Referral (Free)</div>
      <div class="price-feature">Priority 24hr Response</div>
      <a href="#contact" class="price-btn">Get Started</a>
    </div>
    <div class="price-card">
      <div class="price-name">Premium — Large Industry</div>
      <div class="price-amount">₹50,000</div>
      <div class="price-per">/month retainer</div>
      <div class="price-desc">Large manufacturers — complete compliance outsourcing.</div>
      <div class="price-divider"></div>
      <div class="price-feature">Everything in Standard</div>
      <div class="price-feature">EC / EIA Applications</div>
      <div class="price-feature">STP/ETP O&M</div>
      <div class="price-feature">Hazardous Waste Auth.</div>
      <div class="price-feature">All Waste Compliances</div>
      <div class="price-feature">Dedicated Site Visits</div>
      <a href="#contact" class="price-btn">Get Started</a>
    </div>
  </div>
  <p class="price-note">* EC applications, company registrations, one-time services alag charge hote hain. Pehli consultation hamesha free.</p>
</section>

<!-- CONTACT -->
<section class="contact" id="contact">
  <div>
    <div class="section-label">Contact Us</div>
    <h2 class="section-title">Aaj Hi <em>Baat Karein</em></h2>
    <p class="contact-text">Koi bhi problem ho — environment notice, GST issue, company banana ho, plant compliance — pehli baat hamesha free. WhatsApp karein abhi.</p>
    <div class="contact-item"><span class="c-icon">📍</span><div><div class="c-label">Location</div><div class="c-val">Prayagraj, Uttar Pradesh</div></div></div>
    <div class="contact-item"><span class="c-icon">🏛️</span><div><div class="c-label">Advocate Network</div><div class="c-val">Allahabad High Court · NGT · UP Courts</div></div></div>
    <div class="contact-item"><span class="c-icon">🌿</span><div><div class="c-label">Consulting Services</div><div class="c-val">Environment · GST · Company Reg · Waste · STP/ETP</div></div></div>
    <div class="contact-item"><span class="c-icon">🏭</span><div><div class="c-label">Industries We Serve</div><div class="c-val">Chemical · Textile · Paper · Food · Pharma · Manufacturing</div></div></div>
    <a href="https://wa.me/91XXXXXXXXXX" class="whatsapp-btn">💬 WhatsApp Par Message Karein</a>
  </div>
  <div class="contact-form">
    <div class="form-row">
      <div class="form-group"><label class="form-label">Aapka Naam</label><input type="text" class="form-input" placeholder="Full name"></div>
      <div class="form-group"><label class="form-label">Business / Factory</label><input type="text" class="form-input" placeholder="Business name"></div>
    </div>
    <div class="form-row">
      <div class="form-group"><label class="form-label">Phone / WhatsApp</label><input type="tel" class="form-input" placeholder="+91 XXXXX XXXXX"></div>
      <div class="form-group"><label class="form-label">City / District</label><input type="text" class="form-input" placeholder="Prayagraj, Lucknow..."></div>
    </div>
    <div class="form-group">
      <label class="form-label">Service Chahiye</label>
      <select class="form-select">
        <option>Service chunein...</option>
        <option>Environment Consent (CTE/CTO) — UPPCB</option>
        <option>Environmental Clearance (EC/EIA)</option>
        <option>UPPCB / CPCB Notice Reply</option>
        <option>Waste Management (HW/BMW/E-Waste)</option>
        <option>STP/ETP O&M Contract</option>
        <option>Company / LLP Registration</option>
        <option>GST Registration / Return Filing</option>
        <option>ITR / Tax Filing</option>
        <option>MSME / Startup Registration</option>
        <option>Advocate Referral Chahiye</option>
        <option>Monthly Retainer Package</option>
        <option>Other</option>
      </select>
    </div>
    <div class="form-group"><label class="form-label">Apni Problem Batayein</label><textarea class="form-textarea" placeholder="Koi notice mila? Compliance deadline? Company banana? Court jaana hai? Sab yahan likhein — pehli baat free hai..."></textarea></div>
    <button class="form-submit">Free Consultation Request Karein →</button>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-logo">Kalpvriksha <span>Legal & Environmental Solutions</span></div>
  <div class="footer-mid">
    <div class="footer-text">© 2025 Kalpvriksha Legal & Environmental Solutions · Prayagraj, UP</div>
    <div class="footer-disclaimer">Hum sirf consulting & advisory services provide karte hain. Court representation ke liye registered advocates se connect karate hain.</div>
  </div>
  <div class="footer-tag">Prayagraj · Uttar Pradesh · India</div>
</footer>

</body>
</html>
