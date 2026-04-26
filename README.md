[index.html](https://github.com/user-attachments/files/27094358/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Karan | Finance & Accounting Professional</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --navy: #0a1628;
    --dark: #111827;
    --gold: #c9a84c;
    --gold-light: #e8c96d;
    --cream: #f5f0e8;
    --white: #ffffff;
    --gray: #6b7280;
    --light-gray: #f3f4f6;
    --border: rgba(201,168,76,0.2);
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  html { scroll-behavior: smooth; }

  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--navy);
    color: var(--cream);
    overflow-x: hidden;
  }

  /* NAV */
  nav {
    position: fixed; top: 0; width: 100%; z-index: 100;
    padding: 1.2rem 4rem;
    display: flex; justify-content: space-between; align-items: center;
    background: rgba(10,22,40,0.9);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid var(--border);
  }
  .nav-logo {
    font-family: 'Playfair Display', serif;
    font-size: 1.4rem; color: var(--gold); font-weight: 700; letter-spacing: 1px;
  }
  .nav-links { display: flex; gap: 2.5rem; list-style: none; }
  .nav-links a {
    color: var(--cream); text-decoration: none; font-size: 0.85rem;
    letter-spacing: 1.5px; text-transform: uppercase; font-weight: 500;
    opacity: 0.8; transition: all 0.3s;
  }
  .nav-links a:hover { color: var(--gold); opacity: 1; }

  /* HERO */
  #home {
    min-height: 100vh;
    display: flex; align-items: center;
    padding: 8rem 4rem 4rem;
    position: relative;
    overflow: hidden;
  }
  .hero-bg {
    position: absolute; inset: 0;
    background: radial-gradient(ellipse at 70% 50%, rgba(201,168,76,0.08) 0%, transparent 60%),
                radial-gradient(ellipse at 10% 80%, rgba(201,168,76,0.05) 0%, transparent 50%);
  }
  .hero-grid {
    position: absolute; inset: 0; opacity: 0.03;
    background-image: linear-gradient(var(--gold) 1px, transparent 1px),
                      linear-gradient(90deg, var(--gold) 1px, transparent 1px);
    background-size: 60px 60px;
  }
  .hero-content { position: relative; max-width: 700px; }
  .hero-tag {
    display: inline-block;
    border: 1px solid var(--gold);
    color: var(--gold); font-size: 0.75rem; letter-spacing: 3px;
    text-transform: uppercase; padding: 0.4rem 1rem;
    margin-bottom: 1.5rem;
    animation: fadeUp 0.8s ease both;
  }
  .hero-name {
    font-family: 'Playfair Display', serif;
    font-size: clamp(3rem, 7vw, 5.5rem);
    font-weight: 900; line-height: 1.05;
    color: var(--white);
    animation: fadeUp 0.8s 0.1s ease both;
  }
  .hero-name span { color: var(--gold); }
  .hero-title {
    font-size: 1.1rem; font-weight: 300; color: var(--cream);
    opacity: 0.75; margin: 1.2rem 0 2rem;
    line-height: 1.7; max-width: 520px;
    animation: fadeUp 0.8s 0.2s ease both;
  }
  .hero-stats {
    display: flex; gap: 3rem; margin-bottom: 2.5rem;
    animation: fadeUp 0.8s 0.3s ease both;
  }
  .stat { }
  .stat-num {
    font-family: 'Playfair Display', serif;
    font-size: 2rem; font-weight: 700; color: var(--gold);
  }
  .stat-label { font-size: 0.78rem; color: var(--cream); opacity: 0.6; letter-spacing: 1px; text-transform: uppercase; }
  .hero-btns {
    display: flex; gap: 1rem; flex-wrap: wrap;
    animation: fadeUp 0.8s 0.4s ease both;
  }
  .btn-gold {
    background: var(--gold); color: var(--navy);
    padding: 0.85rem 2rem; font-weight: 600; font-size: 0.9rem;
    border: none; cursor: pointer; letter-spacing: 0.5px;
    text-decoration: none; display: inline-block;
    transition: all 0.3s;
  }
  .btn-gold:hover { background: var(--gold-light); transform: translateY(-2px); }
  .btn-outline {
    background: transparent; color: var(--cream);
    padding: 0.85rem 2rem; font-weight: 500; font-size: 0.9rem;
    border: 1px solid rgba(245,240,232,0.3); cursor: pointer;
    text-decoration: none; display: inline-block;
    transition: all 0.3s;
  }
  .btn-outline:hover { border-color: var(--gold); color: var(--gold); transform: translateY(-2px); }
  .hero-side {
    position: absolute; right: 4rem; top: 50%; transform: translateY(-50%);
    display: flex; flex-direction: column; gap: 1.5rem;
    animation: fadeLeft 1s 0.5s ease both;
  }
  .hero-card {
    background: rgba(255,255,255,0.04);
    border: 1px solid var(--border);
    padding: 1.2rem 1.5rem; min-width: 220px;
    backdrop-filter: blur(8px);
  }
  .hero-card-icon { font-size: 1.4rem; margin-bottom: 0.4rem; }
  .hero-card-val { font-family: 'Playfair Display', serif; font-size: 1.3rem; color: var(--gold); }
  .hero-card-desc { font-size: 0.78rem; color: var(--cream); opacity: 0.6; margin-top: 0.2rem; }

  /* SECTIONS COMMON */
  section { padding: 6rem 4rem; }
  .section-label {
    font-size: 0.75rem; letter-spacing: 4px; text-transform: uppercase;
    color: var(--gold); margin-bottom: 0.6rem;
  }
  .section-title {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2rem, 4vw, 3rem); font-weight: 700;
    color: var(--white); line-height: 1.2; margin-bottom: 1rem;
  }
  .section-line {
    width: 60px; height: 2px; background: var(--gold); margin-bottom: 3rem;
  }

  /* ABOUT */
  #about { background: var(--dark); }
  .about-grid {
    display: grid; grid-template-columns: 1fr 1fr; gap: 5rem; align-items: start;
  }
  .about-text p {
    color: var(--cream); opacity: 0.8; line-height: 1.9; font-size: 0.95rem;
    margin-bottom: 1.2rem;
  }
  .about-highlights {
    display: flex; flex-direction: column; gap: 1rem; margin-top: 2rem;
  }
  .highlight-item {
    display: flex; align-items: flex-start; gap: 1rem;
    padding: 1rem; border-left: 2px solid var(--gold);
    background: rgba(201,168,76,0.05);
  }
  .highlight-icon { font-size: 1.2rem; flex-shrink: 0; }
  .highlight-text { font-size: 0.88rem; opacity: 0.85; line-height: 1.6; }
  .about-right { }
  .contact-block {
    background: rgba(201,168,76,0.08);
    border: 1px solid var(--border);
    padding: 2rem; margin-bottom: 2rem;
  }
  .contact-block h3 {
    font-family: 'Playfair Display', serif; font-size: 1.2rem;
    color: var(--gold); margin-bottom: 1.2rem;
  }
  .contact-item {
    display: flex; align-items: center; gap: 0.8rem;
    margin-bottom: 0.9rem; font-size: 0.88rem; opacity: 0.85;
  }
  .contact-item a { color: var(--cream); text-decoration: none; }
  .contact-item a:hover { color: var(--gold); }

  /* EXPERIENCE */
  #experience { background: var(--navy); }
  .exp-timeline { position: relative; }
  .exp-timeline::before {
    content: ''; position: absolute; left: 0; top: 0; bottom: 0;
    width: 1px; background: var(--border);
  }
  .exp-item {
    padding-left: 2.5rem; margin-bottom: 3.5rem; position: relative;
  }
  .exp-item::before {
    content: ''; position: absolute; left: -5px; top: 6px;
    width: 11px; height: 11px;
    background: var(--gold); border-radius: 50%;
  }
  .exp-period {
    font-size: 0.75rem; letter-spacing: 2px; text-transform: uppercase;
    color: var(--gold); margin-bottom: 0.4rem;
  }
  .exp-role {
    font-family: 'Playfair Display', serif; font-size: 1.3rem;
    color: var(--white); margin-bottom: 0.2rem;
  }
  .exp-company { font-size: 0.88rem; color: var(--cream); opacity: 0.6; margin-bottom: 1rem; }
  .exp-points { list-style: none; }
  .exp-points li {
    font-size: 0.88rem; color: var(--cream); opacity: 0.8;
    line-height: 1.7; padding-left: 1.2rem; position: relative; margin-bottom: 0.5rem;
  }
  .exp-points li::before { content: '→'; position: absolute; left: 0; color: var(--gold); font-size: 0.8rem; }
  .exp-badge {
    display: inline-block; background: rgba(201,168,76,0.15);
    border: 1px solid var(--border);
    color: var(--gold); font-size: 0.72rem; padding: 0.25rem 0.7rem;
    margin-top: 0.8rem; letter-spacing: 1px;
  }

  /* SKILLS */
  #skills { background: var(--dark); }
  .skills-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 2rem; }
  .skill-category {
    background: rgba(255,255,255,0.03);
    border: 1px solid var(--border);
    padding: 1.8rem;
    transition: all 0.3s;
  }
  .skill-category:hover { border-color: var(--gold); background: rgba(201,168,76,0.05); }
  .skill-cat-title {
    font-family: 'Playfair Display', serif; font-size: 1rem;
    color: var(--gold); margin-bottom: 1rem; padding-bottom: 0.8rem;
    border-bottom: 1px solid var(--border);
  }
  .skill-tags { display: flex; flex-wrap: wrap; gap: 0.5rem; }
  .skill-tag {
    font-size: 0.76rem; padding: 0.3rem 0.7rem;
    background: rgba(245,240,232,0.06);
    border: 1px solid rgba(245,240,232,0.12);
    color: var(--cream); opacity: 0.85;
    letter-spacing: 0.3px;
  }

  /* SERVICES */
  #services { background: var(--navy); }
  .services-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 2rem; }
  .services-grid .service-card:last-child { grid-column: 2 / 3; }
  .service-card {
    background: rgba(255,255,255,0.03);
    border: 1px solid var(--border);
    padding: 2.2rem; position: relative;
    transition: all 0.4s; overflow: hidden;
  }
  .service-card::before {
    content: ''; position: absolute; top: 0; left: 0; right: 0;
    height: 2px; background: var(--gold);
    transform: scaleX(0); transition: transform 0.4s;
  }
  .service-card:hover { transform: translateY(-4px); border-color: rgba(201,168,76,0.4); }
  .service-card:hover::before { transform: scaleX(1); }
  .service-num {
    font-family: 'Playfair Display', serif; font-size: 2.5rem;
    color: rgba(201,168,76,0.15); font-weight: 900;
    position: absolute; top: 1rem; right: 1.5rem;
  }
  .service-icon { font-size: 1.8rem; margin-bottom: 1rem; }
  .service-title {
    font-family: 'Playfair Display', serif; font-size: 1.15rem;
    color: var(--white); margin-bottom: 0.8rem;
  }
  .service-desc { font-size: 0.85rem; color: var(--cream); opacity: 0.7; line-height: 1.8; }
  .service-tags { display: flex; flex-wrap: wrap; gap: 0.4rem; margin-top: 1rem; }
  .service-tag {
    font-size: 0.7rem; padding: 0.2rem 0.6rem;
    border: 1px solid var(--border); color: var(--gold); letter-spacing: 0.5px;
  }

  /* PROJECTS */
  #projects { background: var(--dark); }
  .projects-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 2rem; }
  .project-card {
    background: rgba(255,255,255,0.03);
    border: 1px solid var(--border);
    padding: 2rem; transition: all 0.3s;
  }
  .project-card:hover { border-color: var(--gold); }
  .project-impact {
    font-family: 'Playfair Display', serif; font-size: 1.8rem;
    color: var(--gold); margin-bottom: 0.5rem;
  }
  .project-title { font-size: 1rem; color: var(--white); font-weight: 500; margin-bottom: 0.8rem; }
  .project-desc { font-size: 0.85rem; color: var(--cream); opacity: 0.75; line-height: 1.8; }

  /* CONTACT */
  #contact { background: var(--navy); }
  .contact-wrapper {
    display: grid; grid-template-columns: 1fr 1fr; gap: 5rem; align-items: start;
  }
  .contact-info h3 {
    font-family: 'Playfair Display', serif; font-size: 1.8rem;
    color: var(--white); margin-bottom: 1rem;
  }
  .contact-info p { font-size: 0.9rem; color: var(--cream); opacity: 0.75; line-height: 1.8; margin-bottom: 2rem; }
  .contact-links { display: flex; flex-direction: column; gap: 1rem; }
  .clink {
    display: flex; align-items: center; gap: 1rem;
    padding: 1rem 1.2rem;
    border: 1px solid var(--border);
    text-decoration: none; color: var(--cream);
    transition: all 0.3s; font-size: 0.88rem;
  }
  .clink:hover { border-color: var(--gold); color: var(--gold); }
  .clink-icon { font-size: 1.2rem; width: 1.5rem; text-align: center; }
  .contact-form { display: flex; flex-direction: column; gap: 1.2rem; }
  .contact-form input, .contact-form textarea {
    background: rgba(255,255,255,0.04);
    border: 1px solid var(--border);
    color: var(--cream); padding: 0.9rem 1rem;
    font-family: 'DM Sans', sans-serif; font-size: 0.88rem;
    outline: none; transition: border 0.3s; resize: vertical;
  }
  .contact-form input::placeholder, .contact-form textarea::placeholder { opacity: 0.4; }
  .contact-form input:focus, .contact-form textarea:focus { border-color: var(--gold); }
  .contact-form textarea { min-height: 120px; }

  /* FOOTER */
  footer {
    background: rgba(0,0,0,0.5);
    border-top: 1px solid var(--border);
    padding: 2rem 4rem;
    display: flex; justify-content: space-between; align-items: center;
    font-size: 0.8rem; color: var(--cream); opacity: 0.5;
  }

  /* ANIMATIONS */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(24px); }
    to { opacity: 1; transform: translateY(0); }
  }
  @keyframes fadeLeft {
    from { opacity: 0; transform: translate(24px, -50%); }
    to { opacity: 1; transform: translate(0, -50%); }
  }

  /* RESPONSIVE */
  @media (max-width: 900px) {
    nav { padding: 1rem 1.5rem; }
    .nav-links { gap: 1.2rem; }
    section { padding: 4rem 1.5rem; }
    #home { padding: 7rem 1.5rem 4rem; flex-direction: column; }
    .hero-side { position: static; transform: none; flex-direction: row; flex-wrap: wrap; margin-top: 2rem; animation: fadeUp 1s 0.5s ease both; }
    .about-grid, .contact-wrapper { grid-template-columns: 1fr; gap: 2.5rem; }
    .skills-grid, .services-grid { grid-template-columns: 1fr; }
    .projects-grid { grid-template-columns: 1fr; }
    footer { flex-direction: column; gap: 0.5rem; text-align: center; }
    .hero-stats { gap: 1.5rem; }
  }
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="nav-logo">Karan</div>
  <ul class="nav-links">
    <li><a href="#about">About</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#services">Services</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<!-- HERO -->
<section id="home">
  <div class="hero-bg"></div>
  <div class="hero-grid"></div>
  <div class="hero-content">
    <div class="hero-tag">Finance & Accounting Professional</div>
    <h1 class="hero-name">Karan<br><span>Finance</span></h1>
    <p class="hero-title">GST Compliance · Financial Reconciliation · Tax Advisory<br>5+ years driving accuracy across ₹200 Cr–₹5,000 Cr businesses</p>
    <div class="hero-stats">
      <div class="stat">
        <div class="stat-num">5+</div>
        <div class="stat-label">Years Experience</div>
      </div>
      <div class="stat">
        <div class="stat-num">₹1 Cr</div>
        <div class="stat-label">Revenue Recovered</div>
      </div>
      <div class="stat">
        <div class="stat-num">100%</div>
        <div class="stat-label">On-Time Compliance</div>
      </div>
    </div>
    <div class="hero-btns">
      <a href="#services" class="btn-gold">View Services</a>
      <a href="#contact" class="btn-outline">Get in Touch</a>
    </div>
  </div>
  <div class="hero-side">
    <div class="hero-card">
      <div class="hero-card-icon">🏦</div>
      <div class="hero-card-val">₹5,000 Cr</div>
      <div class="hero-card-desc">MNC Reconciliation Exposure</div>
    </div>
    <div class="hero-card">
      <div class="hero-card-icon">📋</div>
      <div class="hero-card-val">15+ Clients</div>
      <div class="hero-card-desc">Diverse Industry Portfolio</div>
    </div>
    <div class="hero-card">
      <div class="hero-card-icon">⚡</div>
      <div class="hero-card-val">Multi-Bank</div>
      <div class="hero-card-desc">HDFC, SCB, Deutsche & more</div>
    </div>
  </div>
</section>

<!-- ABOUT -->
<section id="about">
  <div class="section-label">Who I Am</div>
  <div class="section-title">About Me</div>
  <div class="section-line"></div>
  <div class="about-grid">
    <div class="about-text">
      <p>I'm a finance and accounting professional with 5+ years of experience working at the intersection of financial compliance, reconciliation, and operational finance. My core focus is ensuring accuracy across financial systems — connecting tax data, banking transactions, and business records into a structured, reliable framework.</p>
      <p>I specialize in identifying gaps such as pending credits, unmatched deductions, and timing differences, ensuring that financial data reflects the true position of the business. Currently handling multi-bank and high-volume reconciliation processes at Aadifidelis Solutions for a ₹500 Cr business.</p>
      <p>What drives me is bringing clarity and control to financial data — and continuously improving finance processes through automation, structured reporting, and technology-enabled systems.</p>
      <div class="about-highlights">
        <div class="highlight-item">
          <div class="highlight-icon">🎓</div>
          <div class="highlight-text">B.Com (Hons) — Delhi University (2020–2024)</div>
        </div>
        <div class="highlight-item">
          <div class="highlight-icon">📍</div>
          <div class="highlight-text">Based in Patel Nagar, New Delhi — open to remote roles</div>
        </div>
        <div class="highlight-item">
          <div class="highlight-icon">💡</div>
          <div class="highlight-text">Advanced Excel (VLOOKUP, Pivot Tables, Macros, Power Query) + Tally, Busy, Finsys ERP</div>
        </div>
      </div>
    </div>
    <div class="about-right">
      <div class="contact-block">
        <h3>📬 Contact Details</h3>
        <div class="contact-item">📱 <span>+91 85889 65723</span></div>
        <div class="contact-item">✉️ <a href="mailto:karanfinance108@gmail.com">karanfinance108@gmail.com</a></div>
        <div class="contact-item">🔗 <a href="https://www.linkedin.com/in/karan-finance-" target="_blank">linkedin.com/in/karan-finance-</a></div>
      </div>
    </div>
  </div>
</section>

<!-- EXPERIENCE -->
<section id="experience">
  <div class="section-label">Work History</div>
  <div class="section-title">Experience</div>
  <div class="section-line"></div>
  <div class="exp-timeline">

    <div class="exp-item">
      <div class="exp-period">Jul 2024 – Present</div>
      <div class="exp-role">Account Manager</div>
      <div class="exp-company">Aadifidelis Solutions Pvt. Ltd. · New Delhi</div>
      <ul class="exp-points">
        <li>Spearheaded end-to-end GST & payment reconciliation for high-volume transactions across a ₹500 Cr business with 100% statutory compliance and zero mismatches</li>
        <li>Orchestrated multi-bank reconciliations across HDFC, IDFC First, Aditya Birla Finance, SCB, Deutsche Bank and others</li>
        <li>Executed 3-way reconciliation of TDS, GST & Bank Statements; identified pending input credits and unclaimed TDS</li>
        <li>Drove process improvement using Advanced Excel (Power Query, Pivot Tables) to streamline reconciliation workflows</li>
        <li>Recovered ₹1 Cr in unrecognised revenue by identifying unbilled transactions and raising missing invoices</li>
      </ul>
      <span class="exp-badge">₹500 Cr Business</span>
    </div>

    <div class="exp-item">
      <div class="exp-period">Jul 2023 – Jul 2024</div>
      <div class="exp-role">Account Associate</div>
      <div class="exp-company">H Arora & Associates · New Delhi</div>
      <ul class="exp-points">
        <li>Managed GST, TDS & Income Tax compliance for 15+ clients across diverse industries with 100% on-time compliance in FY 2023–24</li>
        <li>Filed GSTR-1, GSTR-3B & GSTR-9; maintained books of accounts including GL, AP, AR and trial balance</li>
        <li>Rebuilt 5 years of historical financial data for a ₹500 Cr company post ERP migration — within ~1 month</li>
        <li>Contributed to ₹5,000 Cr MNC reconciliation project with a 2-week turnaround</li>
      </ul>
      <span class="exp-badge">15+ Clients · ₹5,000 Cr MNC</span>
    </div>

    <div class="exp-item">
      <div class="exp-period">Dec 2020 – Jul 2023</div>
      <div class="exp-role">Assistant Accountant</div>
      <div class="exp-company">Govind Associates · New Delhi</div>
      <ul class="exp-points">
        <li>Managed end-to-end bookkeeping and GST compliance for a diverse multi-client tax consultancy</li>
        <li>Prepared weekly P&L reports for a ₹200 Cr enterprise and supported month-end financial monitoring</li>
        <li>Supported financial reporting for ₹200 Cr Asian Paints dealer — reconciled bill discounting & outstanding receivables</li>
        <li>Executed ITR filings for individuals and businesses with accuracy and timely submission</li>
      </ul>
      <span class="exp-badge">₹200 Cr Enterprise</span>
    </div>

  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="section-label">Expertise</div>
  <div class="section-title">Core Skills</div>
  <div class="section-line"></div>
  <div class="skills-grid">
    <div class="skill-category">
      <div class="skill-cat-title">🧾 Tax & Compliance</div>
      <div class="skill-tags">
        <span class="skill-tag">GST (GSTR-1, 3B, 9)</span>
        <span class="skill-tag">TDS Compliance</span>
        <span class="skill-tag">Income Tax & ITR</span>
        <span class="skill-tag">Tax Audit (TAR)</span>
        <span class="skill-tag">Notice Handling</span>
        <span class="skill-tag">Regulatory Compliance</span>
        <span class="skill-tag">Internal Audits</span>
      </div>
    </div>
    <div class="skill-category">
      <div class="skill-cat-title">🔁 Reconciliation</div>
      <div class="skill-tags">
        <span class="skill-tag">Bank Reconciliation</span>
        <span class="skill-tag">Vendor Reconciliation</span>
        <span class="skill-tag">Ledger Reconciliation</span>
        <span class="skill-tag">3-Way Reconciliation</span>
        <span class="skill-tag">Intercompany Recon</span>
        <span class="skill-tag">Month-End Closing</span>
        <span class="skill-tag">Year-End Closing</span>
      </div>
    </div>
    <div class="skill-category">
      <div class="skill-cat-title">📊 Financial Reporting</div>
      <div class="skill-tags">
        <span class="skill-tag">MIS Reporting</span>
        <span class="skill-tag">P&L Statements</span>
        <span class="skill-tag">Variance Analysis</span>
        <span class="skill-tag">GL Accounting</span>
        <span class="skill-tag">AP & AR Management</span>
        <span class="skill-tag">Journal Entries</span>
        <span class="skill-tag">Trial Balance</span>
      </div>
    </div>
    <div class="skill-category">
      <div class="skill-cat-title">🛠 Tools & ERP</div>
      <div class="skill-tags">
        <span class="skill-tag">Tally ERP</span>
        <span class="skill-tag">Busy Accounting</span>
        <span class="skill-tag">Finsys ERP</span>
        <span class="skill-tag">QuickBooks</span>
        <span class="skill-tag">Xero</span>
        <span class="skill-tag">GST Portal</span>
        <span class="skill-tag">TRACES</span>
      </div>
    </div>
    <div class="skill-category">
      <div class="skill-cat-title">💻 Excel & Automation</div>
      <div class="skill-tags">
        <span class="skill-tag">VLOOKUP / XLOOKUP</span>
        <span class="skill-tag">Pivot Tables</span>
        <span class="skill-tag">Power Query</span>
        <span class="skill-tag">Macros</span>
        <span class="skill-tag">Data Validation</span>
        <span class="skill-tag">Process Automation</span>
      </div>
    </div>
    <div class="skill-category">
      <div class="skill-cat-title">🤝 Soft Skills</div>
      <div class="skill-tags">
        <span class="skill-tag">Client Handling</span>
        <span class="skill-tag">Cross-functional Coordination</span>
        <span class="skill-tag">Remote Work</span>
        <span class="skill-tag">Compliance Advisory</span>
        <span class="skill-tag">Problem Solving</span>
      </div>
    </div>
  </div>
</section>

<!-- SERVICES -->
<section id="services">
  <div class="section-label">What I Offer</div>
  <div class="section-title">Services</div>
  <div class="section-line"></div>
  <div class="services-grid">
    <div class="service-card">
      <div class="service-num">01</div>
      <div class="service-icon">🧾</div>
      <div class="service-title">GST Compliance & Filing</div>
      <div class="service-desc">End-to-end GST management — filing GSTR-1, GSTR-3B, GSTR-9, input credit reconciliation, notice handling, and ensuring 100% statutory compliance.</div>
      <div class="service-tags">
        <span class="service-tag">GSTR-1 / 3B / 9</span>
        <span class="service-tag">Input Credit</span>
        <span class="service-tag">Notice Handling</span>
      </div>
    </div>
    <div class="service-card">
      <div class="service-num">02</div>
      <div class="service-icon">🔄</div>
      <div class="service-title">Financial Reconciliation</div>
      <div class="service-desc">Multi-bank reconciliation, 3-way TDS/GST/Bank reconciliation, ledger and vendor reconciliation for businesses of any size — from ₹1 Cr to ₹5,000 Cr.</div>
      <div class="service-tags">
        <span class="service-tag">Bank Recon</span>
        <span class="service-tag">3-Way Recon</span>
        <span class="service-tag">Ledger Recon</span>
      </div>
    </div>
    <div class="service-card">
      <div class="service-num">03</div>
      <div class="service-icon">📈</div>
      <div class="service-title">Bookkeeping & Accounting</div>
      <div class="service-desc">Complete bookkeeping — journal entries, AP/AR management, General Ledger maintenance, trial balance, and month-end/year-end financial closes.</div>
      <div class="service-tags">
        <span class="service-tag">GL Accounting</span>
        <span class="service-tag">AP / AR</span>
        <span class="service-tag">Month-End Close</span>
      </div>
    </div>
    <div class="service-card">
      <div class="service-num">04</div>
      <div class="service-icon">🏛</div>
      <div class="service-title">Income Tax & TDS</div>
      <div class="service-desc">ITR filing for individuals and businesses, TDS returns, income tax computations, notice handling, and compliance advisory for a stress-free tax season.</div>
      <div class="service-tags">
        <span class="service-tag">ITR Filing</span>
        <span class="service-tag">TDS Returns</span>
        <span class="service-tag">Notice Handling</span>
      </div>
    </div>
    <div class="service-card">
      <div class="service-num">05</div>
      <div class="service-icon">📊</div>
      <div class="service-title">MIS & Financial Reporting</div>
      <div class="service-desc">Custom MIS reports, P&L statements, variance analysis, and management dashboards — helping you make informed business decisions with clean, reliable data.</div>
      <div class="service-tags">
        <span class="service-tag">MIS Reports</span>
        <span class="service-tag">P&L Analysis</span>
        <span class="service-tag">Dashboards</span>
      </div>
    </div>
    <div class="service-card">
      <div class="service-num">06</div>
      <div class="service-icon">⚙️</div>
      <div class="service-title">Excel Automation & Process Improvement</div>
      <div class="service-desc">Automate repetitive finance workflows using Advanced Excel (VLOOKUP, Power Query, Macros) — reducing manual effort and improving turnaround time.</div>
      <div class="service-tags">
        <span class="service-tag">Power Query</span>
        <span class="service-tag">Macros</span>
        <span class="service-tag">Workflow Automation</span>
      </div>
    </div>
    <div class="service-card">
      <div class="service-num">07</div>
      <div class="service-icon">🏦</div>
      <div class="service-title">Loan & Financing Assistance</div>
      <div class="service-desc">End-to-end loan facilitation for individuals and businesses — helping you find the right financing solution, prepare documentation, and navigate the approval process with ease.</div>
      <div class="service-tags">
        <span class="service-tag">Personal Loan</span>
        <span class="service-tag">Business Loan</span>
        <span class="service-tag">Home Loan</span>
        <span class="service-tag">LAP</span>
      </div>
    </div>
  </div>
</section>

<!-- PROJECTS -->
<section id="projects">
  <div class="section-label">Key Achievements</div>
  <div class="section-title">Notable Projects</div>
  <div class="section-line"></div>
  <div class="projects-grid">
    <div class="project-card">
      <div class="project-impact">₹1 Cr</div>
      <div class="project-title">Revenue Recovery — Aadifidelis Solutions</div>
      <div class="project-desc">Identified business transactions where services had been delivered but invoices were never raised. Issued all missing invoices, tracked collections, and successfully recovered the full outstanding amount — directly strengthening AR and revenue recognition accuracy.</div>
    </div>
    <div class="project-card">
      <div class="project-impact">3 Years</div>
      <div class="project-title">Reconciliation Backlog Cleared from Scratch</div>
      <div class="project-desc">Conducted full ledger reconciliation across all disputed accounts covering a 3-year period. Resolved long-standing mismatches across bank debtors, GL, invoices, and statements — delivering clean, audit-ready reconciliation records with complete management visibility.</div>
    </div>
    <div class="project-card">
      <div class="project-impact">₹500 Cr</div>
      <div class="project-title">ERP Migration & Books Reconstruction</div>
      <div class="project-desc">Rebuilt and corrected 5 years of historical financial data for a ₹500 Cr company impacted by ERP migration — completed within approximately 1 month while simultaneously learning the new ERP system (Finsys).</div>
    </div>
    <div class="project-card">
      <div class="project-impact">₹5,000 Cr</div>
      <div class="project-title">MNC Reconciliation Project</div>
      <div class="project-desc">Contributed to large-scale data reconciliation and validation for a ₹5,000 Cr MNC — completed within a 2-week turnaround, gaining exposure to enterprise-level financial processes and high-pressure reconciliation environments.</div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="section-label">Let's Connect</div>
  <div class="section-title">Get in Touch</div>
  <div class="section-line"></div>
  <div class="contact-wrapper">
    <div class="contact-info">
      <h3>Open to Remote Finance Roles & Freelance Projects</h3>
      <p>Whether you need help with GST compliance, financial reconciliation, bookkeeping, or Excel automation — I'd love to hear from you. I work with businesses of all sizes and am comfortable handling complex, high-volume environments remotely.</p>
      <div class="contact-links">
        <a href="tel:+918588965723" class="clink">
          <span class="clink-icon">📱</span>
          <span>+91 85889 65723</span>
        </a>
        <a href="mailto:karanfinance108@gmail.com" class="clink">
          <span class="clink-icon">✉️</span>
          <span>karanfinance108@gmail.com</span>
        </a>
        <a href="https://www.linkedin.com/in/karan-finance-" target="_blank" class="clink">
          <span class="clink-icon">🔗</span>
          <span>linkedin.com/in/karan-finance-</span>
        </a>
      </div>
    </div>
    <div>
      <div class="contact-form">
        <input type="text" placeholder="Your Name">
        <input type="email" placeholder="Your Email">
        <input type="text" placeholder="Subject (e.g. GST Filing, Reconciliation)">
        <textarea placeholder="Tell me about your requirement..."></textarea>
        <a href="mailto:karanfinance108@gmail.com" class="btn-gold" style="text-align:center;">Send Message</a>
      </div>
    </div>
  </div>
</section>

<footer>
  <span>© 2025 Karan Finance. All rights reserved.</span>
  <span>Finance & Accounting Professional · New Delhi</span>
</footer>

</body>
</html>
