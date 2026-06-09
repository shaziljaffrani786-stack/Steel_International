<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Steel International - Leading Steel Supplier in Karachi</title>
  <meta name="description" content="Steel International supplies CRC, HRC coils, GI sheets, pipes & structural steel. Old Steel Market, Karachi. Call 03317128737">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #0A2647;     /* Dark blue like Bisteel */
      --accent: #FF6B35;      /* Orange accent */
      --dark: #1C1C1C;
      --light: #F8F9FA;
      --gray: #6C757D;
    }
    * { margin: 0; padding: 0; box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body { font-family: 'Inter', sans-serif; color: var(--dark); line-height: 1.7; }
    .container { max-width: 1200px; margin: 0 auto; padding: 0 20px; }
    
    /* Header */
    header { background: #fff; box-shadow: 0 2px 10px rgba(0,0,0,0.05); position: sticky; top: 0; z-index: 1000; }
    .nav { display: flex; justify-content: space-between; align-items: center; height: 80px; }
    .logo { display: flex; align-items: center; gap: 12px; text-decoration: none; }
    .logo-text { font-size: 1.4rem; font-weight: 800; color: var(--primary); }
    .logo-text span { color: var(--accent); }
    .nav-links { display: flex; gap: 30px; }
    .nav-links a { text-decoration: none; color: var(--dark); font-weight: 500; transition: 0.3s; }
    .nav-links a:hover { color: var(--accent); }
    .cta-btn { background: var(--accent); color: #fff; padding: 10px 22px; border-radius: 6px; text-decoration: none; font-weight: 600; transition: 0.3s; }
    .cta-btn:hover { background: #e55a2b; transform: translateY(-2px); }
    
    /* Hero */
    .hero { background: linear-gradient(135deg, var(--primary) 0%, #144272 100%); color: #fff; padding: 120px 0 100px; }
    .hero-grid { display: grid; grid-template-columns: 1.2fr 1fr; gap: 60px; align-items: center; }
    .hero h1 { font-size: 3.2rem; font-weight: 800; line-height: 1.2; margin-bottom: 20px; }
    .hero h1 span { color: var(--accent); }
    .hero p { font-size: 1.1rem; opacity: 0.9; margin-bottom: 30px; max-width: 500px; }
    .hero-img { background: url('https://images.unsplash.com/photo-1587293852726-70cdb56c2866?q=80&w=2072') center/cover; height: 400px; border-radius: 12px; box-shadow: 0 20px 40px rgba(0,0,0,0.2); }
    
    /* Stats Bar */
    .stats { background: var(--light); padding: 40px 0; margin-top: -40px; position: relative; z-index: 10; }
    .stats-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 30px; background: #fff; padding: 30px; border-radius: 12px; box-shadow: 0 10px 30px rgba(0,0,0,0.08); }
    .stat { text-align: center; }
    .stat h3 { font-size: 2rem; color: var(--primary); font-weight: 800; }
    .stat p { color: var(--gray); font-weight: 500; }
    
    /* Section */
    section { padding: 80px 0; }
    .section-title { text-align: center; margin-bottom: 60px; }
    .section-title h2 { font-size: 2.5rem; font-weight: 800; color: var(--primary); margin-bottom: 10px; }
    .section-title p { color: var(--gray); max-width: 600px; margin: 0 auto; }
    
    /* Products */
    .product-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 30px; }
    .product-card { background: #fff; border: 1px solid #eee; border-radius: 12px; overflow: hidden; transition: 0.3s; }
    .product-card:hover { transform: translateY(-8px); box-shadow: 0 15px 35px rgba(0,0,0,0.1); }
    .product-img { height: 200px; background: var(--light); background-size: cover; background-position: center; }
    .product-content { padding: 25px; }
    .product-content h3 { font-size: 1.3rem; margin-bottom: 10px; color: var(--primary); }
    .product-content p { color: var(--gray); font-size: 0.95rem; margin-bottom: 15px; }
    .tag { display: inline-block; background: rgba(255,107,53,0.1); color: var(--accent); padding: 4px 12px; border-radius: 20px; font-size: 0.8rem; font-weight: 600; }
    
    /* About */
    .about { background: var(--light); }
    .about-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 60px; align-items: center; }
    .about-img { height: 450px; background: url('https://images.unsplash.com/photo-1565043666747-69f6646db940?q=80&w=1974') center/cover; border-radius: 12px; }
    .feature { display: flex; gap: 15px; margin-bottom: 25px; }
    .feature-icon { width: 50px; height: 50px; background: rgba(10,38,71,0.1); border-radius: 10px; display: flex; align-items: center; justify-content: center; flex-shrink: 0; }
    .feature-icon svg { width: 24px; height: 24px; color: var(--primary); }
    
    /* Contact */
    .contact-box { background: var(--primary); color: #fff; padding: 60px; border-radius: 16px; text-align: center; }
    .contact-box h2 { font-size: 2.2rem; margin-bottom: 15px; }
    .contact-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 30px; margin: 40px 0; }
    .contact-item h4 { color: var(--accent); margin-bottom: 8px; }
    .contact-item a { color: #fff; text-decoration: none; }
    .whatsapp-btn { background: #25D366; color: #fff; padding: 14px 35px; border-radius: 8px; text-decoration: none; font-weight: 700; display: inline-block; margin-top: 10px; }
    
    /* Footer */
    footer { background: var(--dark); color: #aaa; padding: 30px 0; text-align: center; font-size: 0.9rem; }
    
    /* Mobile */
    @media(max-width: 992px) {
      .hero-grid, .about-grid { grid-template-columns: 1fr; }
      .hero-img, .about-img { height: 300px; }
      .stats-grid { grid-template-columns: repeat(2, 1fr); }
      .contact-grid { grid-template-columns: 1fr; }
      .nav-links { display: none; }
      .hero h1 { font-size: 2.4rem; }
    }
    @media(max-width: 576px) {
      .stats-grid { grid-template-columns: 1fr; }
      .hero { padding: 80px 0; }
      section { padding: 60px 0; }
    }
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <a href="#" class="logo">
        <!-- Custom SVG Logo -->
        <svg width="40" height="40" viewBox="0 0 40 40" fill="none">
          <rect width="40" height="40" rx="8" fill="#0A2647"/>
          <path d="M10 28L20 12L30 28H25L20 19L15 28H10Z" fill="#FF6B35"/>
          <path d="M15 28H25V31H15V28Z" fill="white"/>
        </svg>
        <div class="logo-text">STEEL<span>INTERNATIONAL</span></div>
      </a>
      <nav class="nav-links">
        <a href="#products">Products</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </nav>
      <a href="tel:03317128737" class="cta-btn">Call Now</a>
    </div>
  </header>

  <section class="hero">
    <div class="container hero-grid">
      <div>
        <h1>Pakistan's Trusted <span>Steel Supplier</span></h1>
        <p>Premium quality CRC, HRC coils, GI sheets, and structural steel products. Serving Karachi's Old Steel Market with integrity and competitive rates.</p>
        <a href="#products" class="cta-btn">Explore Products</a>
      </div>
      <div class="hero-img"></div>
    </div>
  </section>

  <section class="stats">
    <div class="container">
      <div class="stats-grid">
        <div class="stat"><h3>15+</h3><p>Years Experience</p></div>
        <div class="stat"><h3>500+</h3><p>Happy Clients</p></div>
        <div class="stat"><h3>50+</h3><p>Steel Variants</p></div>
        <div class="stat"><h3>24/7</h3><p>Support</p></div>
      </div>
    </div>
  </section>

  <section id="products">
    <div class="container">
      <div class="section-title">
        <h2>Our Steel Products</h2>
        <p>We stock a complete range of steel products for construction, fabrication, and industrial applications</p>
      </div>
      <div class="product-grid">
        <div class="product-card">
          <div class="product-img" style="background-image: url('https://images.unsplash.com/photo-1613665813446-82a78c468a1d?q=80&w=2058')"></div>
          <div class="product-content">
            <span class="tag">Best Seller</span>
            <h3>CRC Coil Sheets</h3>
            <p>Cold Rolled Coils with smooth finish. Available in 0.3mm to 3.0mm. Used in appliances, automobiles, furniture.</p>
          </div>
        <div class="product-card">
          <div class="product-img" style="background-image: url('https://images.unsplash.com/photo-1621905252507-b35492cc74b4?q=80&w=2069')"></div>
          <div class="product-content">
            <span class="tag">Industrial Grade</span>
            <h3>HRC Coil Sheets</h3>
            <p>Hot Rolled Coils for heavy-duty use. High tensile strength for construction, pipes, and shipbuilding.</p>
          </div>
        </div>
        <div class="product-card">
          <div class="product-img" style="background-image: url('https://images.unsplash.com/photo-1541888946425-d81bb19240f5?q=80&w=2070')"></div>
          <div class="product-content">
            <span class="tag">Corrosion Free</span>
            <h3>GI Sheets & Coils</h3>
            <p>Galvanized Iron sheets for roofing, ducting, and outdoor use. Zinc coated for maximum rust protection.</p>
          </div>
        <div class="product-card">
          <div class="product-img" style="background-image: url('https://images.unsplash.com/photo-1504307651254-35680f356dfd?q=80&w=2076')"></div>
          <div class="product-content">
            <h3>MS Pipes & Tubes</h3>
            <p>Mild Steel round, square & rectangular pipes. All sizes available for scaffolding, gates, and structures.</p>
          </div>
        </div>
        <div class="product-card">
          <div class="product-img" style="background-image: url('https://images.unsplash.com/photo-1599707367072-cd6ada2bc375?q=80&w=2033')"></div>
          <div class="product-content">
            <h3>Steel Plates</h3>
            <p>MS Plates and Chequered plates for flooring, bridges, and heavy machinery base. Cut-to-size available.</p>
          </div>
        </div>
        <div class="product-card">
          <div class="product-img" style="background-image: url('https://images.unsplash.com/photo-1581092918056-0c4c3acd3789?q=80&w=2070')"></div>
          <div class="product-content">
            <h3>Angle, Channel, T-Iron</h3>
            <p>Complete structural steel range for building frames, trusses, industrial sheds, and fabrication work.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="about" class="about">
    <div class="container about-grid">
      <div class="about-img"></div>
      <div>
        <div class="section-title" style="text-align:left; margin-bottom: 30px;">
          <h2>Why Steel International?</h2>
          <p>Located in Karachi's Old Steel Market, we combine quality material with honest business practices.</p>
        </div>
        <div class="feature">
          <div class="feature-icon">
            <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>
          </div>
          <div><h4>Quality Guaranteed</h4><p>We source directly from top mills. Every sheet and coil meets industry standards.</p></div>
        </div>
        <div class="feature">
          <div class="feature-icon">
            <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1"></path></svg>
          </div>
          <div><h4>Competitive Pricing</h4><p>Wholesale rates for bulk buyers. Regular stock updates to give you the best market price.</p></div>
        </div>
        <div class="feature">
          <div class="feature-icon">
            <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
          </div>
          <div><h4>Fast Delivery</h4><p>Ready stock for immediate pickup. Karachi-wide delivery available for bulk orders.</p></div>
        </div>
      </div>
    </div>
  </section>

  <section id="contact">
    <div class="container">
      <div class="contact-box">
        <h2>Get Steel Rates Today</h2>
        <p>Call us for live rates, stock availability, and expert advice</p>
        <div class="contact-grid">
          <div class="contact-item">
            <h4>Address</h4>
            <p>Old Steel Market<br>Karachi, Pakistan</p>
          </div>
          <div class="contact-item">
            <h4>Phone</h4>
            <p><a href="tel:03317128737">0331-7128737</a></p>
          </div>
          <div class="contact-item">
            <h4>Business Hours</h4>
            <p>Mon - Sat<br>10:00 AM - 7:00 PM</p>
          </div>
        <a href="https://wa.me/923317128737" class="whatsapp-btn">Chat on WhatsApp</a>
      </div>
    </div>
  </section>

  <footer>
    <div class="container">
      <p>&copy; 2026 Steel International. Old Steel Market, Karachi. All Rights Reserved.</p>
    </div>
  </footer>
</body>
</html>
