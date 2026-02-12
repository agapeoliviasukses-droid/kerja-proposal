<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>PT. AGAPE OLIVIA SUKSES - Spesialis Heater Industri</title>
  <meta name="description" content="Spesialis Heater Element & Sistem Pemanas Industri terbaik dan terpercaya.">
  
  <!-- Font Google 'Inter' -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
  
  <style>
    /* --- CSS VARIABLES & RESET --- */
    :root {
      /* Palette Warna Brand */
      --primary-color: #2563eb;     /* Biru Utama */
      --primary-dark: #1e40af;      /* Biru Gelap */
      --secondary-color: #1f2937;   /* Abu-abu Gelap */
      --accent-color: #f59e0b;      /* Oranye Safety */
      --red-logo: #dc2626;          /* Merah Brand */
      --black-logo: #180082;        /* Hitam Kebiruan (Sesuai aslinya) */
      
      /* Netral & Background */
      --bg-light: #f9fafb;
      --bg-white: #ffffff;
      --text-dark: #111827;
      --text-gray: #4b5563;
      --border-color: #e5e7eb;
      
      /* Efek */
      --shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
      --shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
      --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
      --radius: 8px;
      --transition: all 0.3s ease;
    }

    *, *::before, *::after {
      box-sizing: border-box;
    }
    
    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Inter', sans-serif;
      margin: 0;
      padding: 0;
      line-height: 1.6;
      color: var(--text-dark);
      background-color: var(--bg-light);
      overflow-x: hidden; /* Mencegah scroll horizontal */
    }

    a { text-decoration: none; color: inherit; transition: var(--transition); }
    ul { list-style: none; padding: 0; margin: 0; }
    img { max-width: 100%; display: block; }
    h1, h2, h3, p { margin-top: 0; }

    /* --- HEADER & NAVIGATION --- */
    header {
      background-color: var(--bg-white);
      box-shadow: var(--shadow-sm);
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    .header-top {
      max-width: 1200px;
      margin: auto;
      padding: 15px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    /* Styling Logo yang Lebih Rapi */
    .brand {
      display: flex;
      flex-direction: column;
    }

    .brand-logo-text {
      font-size: 1.8rem; /* Ukuran font disesuaikan agar tidak terlalu besar */
      font-weight: 800;
      text-transform: uppercase;
      line-height: 1.1;
      letter-spacing: -0.5px;
    }

    .brand-tagline {
      font-size: 0.9rem;
      color: var(--primary-color);
      font-weight: 600;
      margin-top: 4px;
    }

    /* Warna Logo */
    .txt-black { color: var(--black-logo); }
    .txt-blue { color: var(--primary-color); }
    .txt-red { color: var(--red-logo); }

    /* Navigasi */
    nav {
      background-color: var(--secondary-color);
      width: 100%;
    }

    .nav-container {
      max-width: 1200px;
      margin: auto;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .nav-list {
      display: flex;
      gap: 40px;
      padding: 12px 0;
    }

    .nav-link {
      color: var(--bg-white);
      font-weight: 500;
      font-size: 0.95rem;
      position: relative;
    }

    .nav-link:hover {
      color: var(--accent-color);
    }

    .nav-link::after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      bottom: -4px;
      left: 0;
      background-color: var(--accent-color);
      transition: width 0.3s;
    }

    .nav-link:hover::after {
      width: 100%;
    }

    /* Tombol Hamburger (Mobile) */
    .menu-toggle {
      display: none;
      flex-direction: column;
      cursor: pointer;
      gap: 5px;
    }

    .bar {
      width: 25px;
      height: 3px;
      background-color: var(--text-dark);
      transition: 0.3s;
    }

    /* --- HERO SECTION --- */
    .hero {
      position: relative;
      background: linear-gradient(rgba(31, 41, 55, 0.8), rgba(31, 41, 55, 0.85)), 
                  url('https://files.catbox.moe/6agle1.png') no-repeat center center/cover;
      color: var(--bg-white);
      text-align: center;
      padding: 120px 20px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      min-height: 80vh; /* Tinggi minimum layar */
    }

    .hero h2 {
      font-size: 3rem;
      margin-bottom: 20px;
      font-weight: 700;
      line-height: 1.2;
    }

    .hero p {
      font-size: 1.2rem;
      max-width: 700px;
      margin: 0 auto 40px;
      opacity: 0.9;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      padding: 14px 36px;
      background-color: var(--primary-color);
      color: var(--bg-white);
      border-radius: 50px; /* Rounded pill shape lebih modern */
      font-weight: 600;
      border: none;
      cursor: pointer;
      box-shadow: 0 4px 14px rgba(37, 99, 235, 0.4);
      transition: var(--transition);
    }

    .btn:hover { 
      background-color: var(--primary-dark); 
      transform: translateY(-3px);
      box-shadow: 0 6px 20px rgba(37, 99, 235, 0.6);
    }

    .btn-secondary {
      background-color: var(--secondary-color);
      box-shadow: var(--shadow-md);
    }

    .btn-secondary:hover {
      background-color: #000;
      box-shadow: var(--shadow-lg);
    }

    /* --- SECTIONS LAYOUT --- */
    main {
      overflow: hidden;
    }

    section {
      padding: 80px 20px;
      max-width: 1200px;
      margin: auto;
    }

    .section-header {
      text-align: center;
      margin-bottom: 60px;
    }

    .section-header h2 {
      font-size: 2.25rem;
      color: var(--secondary-color);
      margin-bottom: 15px;
      position: relative;
      display: inline-block;
    }
    
    .section-header p {
      color: var(--text-gray);
      max-width: 600px;
      margin: 0 auto;
    }

    .separator-line {
      width: 60px;
      height: 4px;
      background-color: var(--accent-color);
      margin: 10px auto 0;
      border-radius: 2px;
    }

    /* --- ABOUT SECTION (List Produk) --- */
    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 40px;
      align-items: start;
    }

    .catalog-card {
      background: var(--bg-white);
      padding: 40px;
      border-radius: var(--radius);
      box-shadow: var(--shadow-md);
      border: 1px solid var(--border-color);
      border-top: 5px solid var(--primary-color);
      height: 100%;
    }

    .catalog-card h3 {
      color: var(--primary-color);
      font-size: 1.3rem;
      margin-bottom: 25px;
      display: flex;
      align-items: center;
      gap: 12px;
      border-bottom: 1px solid var(--bg-light);
      padding-bottom: 15px;
    }

    .catalog-list li {
      padding: 12px 0;
      border-bottom: 1px dashed var(--border-color);
      color: var(--text-gray);
      display: flex;
      align-items: center;
      transition: 0.2s;
    }

    .catalog-list li:last-child {
      border-bottom: none;
    }

    .catalog-list li:hover {
      color: var(--primary-color);
      padding-left: 5px;
    }

    .catalog-list li::before {
      content: "•";
      color: var(--accent-color);
      font-weight: bold;
      display: inline-block;
      width: 20px;
      font-size: 1.2em;
    }

    /* --- SERVICES / CARDS --- */
    .bg-gray {
      background-color: var(--bg-light);
      width: 100%;
      max-width: 100%; /* Full width background */
    }
    
    .bg-gray section {
        /* Padding tetap */
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 30px;
    }

    .product-card {
      background: var(--bg-white);
      border-radius: var(--radius);
      overflow: hidden;
      box-shadow: var(--shadow-sm);
      transition: var(--transition);
      border: 1px solid var(--border-color);
      display: flex;
      flex-direction: column;
    }

    .product-card:hover {
      transform: translateY(-8px);
      box-shadow: var(--shadow-lg);
    }

    .card-img-wrapper {
      height: 200px;
      overflow: hidden;
      position: relative;
      background-color: #eee;
    }

    .card-img-wrapper img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.5s ease;
    }

    .product-card:hover img {
      transform: scale(1.1);
    }

    .card-content {
      padding: 25px;
      flex-grow: 1;
      display: flex;
      flex-direction: column;
    }

    .card-content h3 {
      font-size: 1.25rem;
      color: var(--secondary-color);
      margin-bottom: 10px;
    }

    .card-content p {
      color: var(--text-gray);
      font-size: 0.95rem;
      line-height: 1.6;
    }

    /* --- CONTACT SECTION --- */
    .contact-wrapper {
      background: var(--bg-white);
      border-radius: var(--radius);
      box-shadow: var(--shadow-md);
      display: flex;
      flex-wrap: wrap;
      overflow: hidden;
      border: 1px solid var(--border-color);
    }

    .contact-info-col {
      flex: 1;
      min-width: 320px;
      padding: 50px;
    }

    .contact-map-col {
      flex: 1;
      min-width: 300px;
      background: #eee;
      min-height: 400px;
      position: relative;
    }
    
    .map-container {
      width: 100%;
      height: 100%;
      position: absolute;
      top: 0;
      left: 0;
    }

    .map-container iframe {
      width: 100%;
      height: 100%;
      border: 0;
    }

    .contact-item {
      display: flex;
      align-items: flex-start;
      margin-bottom: 30px;
    }

    .icon-box {
      background: #eff6ff;
      color: var(--primary-color);
      width: 50px;
      height: 50px;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 12px;
      margin-right: 20px;
      flex-shrink: 0;
      transition: var(--transition);
    }
    
    .contact-item:hover .icon-box {
      background-color: var(--primary-color);
      color: var(--bg-white);
    }

    .contact-details h4 {
      color: var(--secondary-color);
      font-size: 1.1rem;
      margin-bottom: 5px;
    }

    .contact-details p {
      color: var(--text-gray);
      margin: 0;
    }
    
    .contact-details a {
      color: var(--text-gray);
    }
    
    .contact-details a:hover {
      color: var(--primary-color);
      text-decoration: underline;
    }

    /* --- FOOTER --- */
    footer {
      background-color: var(--secondary-color);
      color: #d1d5db;
      text-align: center;
      padding: 40px 20px;
      margin-top: 80px;
      border-top: 5px solid var(--accent-color);
    }
    
    footer p { margin: 5px 0; font-size: 0.95rem; }
    footer strong { color: var(--bg-white); }

    /* --- MEDIA QUERIES --- */
    @media (max-width: 992px) {
      .about-grid { grid-template-columns: 1fr; }
    }

    @media (max-width: 768px) {
      /* Header Mobile */
      .header-top { padding: 10px 20px; }
      .brand-logo-text { font-size: 1.4rem; }
      .brand-tagline { font-size: 0.8rem; }
      
      /* Nav Mobile */
      .menu-toggle { display: flex; }
      
      .nav-container { flex-direction: column; align-items: flex-start; }
      
      .nav-list {
        display: none; /* Hide default */
        flex-direction: column;
        width: 100%;
        gap: 0;
        padding: 0;
        background-color: var(--secondary-color);
      }
      
      .nav-list.active {
        display: flex; /* Show when active */
      }
      
      .nav-list li {
        width: 100%;
        border-bottom: 1px solid rgba(255,255,255,0.1);
      }
      
      .nav-link {
        display: block;
        padding: 15px 20px;
      }
      
      .nav-link::after { display: none; }
      
      /* Hero Mobile */
      .hero { padding: 80px 20px; min-height: 60vh; }
      .hero h2 { font-size: 2.2rem; }
      .hero p { font-size: 1rem; }
      
      /* Layout Mobile */
      .catalog-card { padding: 25px; }
      section { padding: 50px 20px; }
      
      .contact-info-col { padding: 30px; order: 2; }
      .contact-map-col { min-height: 300px; order: 1; }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="header-top">
      <div class="brand">
        <div class="brand-logo-text">
          <span class="txt-black">PT. AGAPE OLIVIA</span> <span class="txt-red">SUKSES</span>
        </div>
        <div class="brand-tagline">Spesialis Heater Element & Sistem Pemanas Industri</div>
      </div>
      
      <!-- Tombol Hamburger untuk Mobile -->
      <div class="menu-toggle" id="mobile-menu">
        <span class="bar"></span>
        <span class="bar"></span>
        <span class="bar"></span>
      </div>
    </div>

    <nav>
      <div class="nav-container">
        <ul class="nav-list" id="nav-list">
          <li><a href="#about" class="nav-link">Tentang Kami</a></li>
          <li><a href="#services" class="nav-link">Produk Unggulan</a></li>
          <li><a href="#contact" class="nav-link">Kontak</a></li>
        </ul>
      </div>
    </nav>
  </header>

  <main>
    <!-- Hero Section -->
    <section class="hero">
      <h2>Solusi Pemanas Industri Terpercaya</h2>
      <p>Kami menyediakan kualitas heater element terbaik untuk mendukung efisiensi dan kehandalan produksi manufaktur Anda.</p>
      <a href="#contact" class="btn">Hubungi Kami Sekarang</a>
    </section>

    <!-- About Section -->
    <section id="about">
      <div class="section-header">
        <h2>Tentang Kami</h2>
        <div class="separator-line"></div>
        <p style="margin-top: 15px;">
          <strong>PT. Agape Olivia Sukses</strong> adalah perusahaan yang bergerak di bidang penyediaan
          heater element (alat pemanas industri) untuk berbagai kebutuhan manufaktur.
        </p>
      </div>
      
      <div class="about-grid">
        <!-- Kolom Spare Part -->
        <div class="catalog-card">
          <h3>
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3L6.91 6.91a6 6 0 0 1 7.94-7.94l-3.76 3.76z"></path></svg>
            Katalog Spare Part
          </h3>
          <ul class="catalog-list">
            <li>Immersion Heater</li>
            <li>Silicon Nitride</li>
            <li>Infrared Black Body</li>
            <li>Bobin Heater</li>
            <li>Cartridge Heater</li>
            <li>Tubular Heater</li>
            <li>Silica Quartz Heater</li>
            <li>Thermocouple Control</li>
            <li>Band Heater</li>
            <li>Cooling Heatsink</li>
            <li>Heatsink Heater</li>
            <li>Ceramic Heater</li>
            <li>Cast In Heater</li>
            <li>Coil Heater</li>
            <li>Flat/Strip Heater</li>
          </ul>
        </div>

        <!-- Kolom Mesin -->
        <div class="catalog-card">
          <h3>
             <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="3" width="20" height="14" rx="2" ry="2"></rect><line x1="8" y1="21" x2="16" y2="21"></line><line x1="12" y1="17" x2="12" y2="21"></line></svg>
            Katalog Mesin Industri
          </h3>
          <ul class="catalog-list">
            <li>Oven Circulation</li>
            <li>Oven Furnace</li>
            <li>Electric Duct Heater</li>
            <li>Load Bank</li>
            <li>Incinerator</li>
            <li>Hot Room Installation</li>
            <li>Oven Conveyor</li>
            <li>Hot Tank</li>
            <li>Heat Exchangers</li>
            <li>Heat Boiler</li>
            <li>Custom Order (Spesifikasi Khusus)</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- Services / Products Showcase -->
    <div class="bg-gray">
      <section id="services">
        <div class="section-header">
          <h2>Produk Unggulan</h2>
          <div class="separator-line"></div>
        </div>

        <div class="product-grid">
          <!-- Card 1 -->
          <div class="product-card">
            <div class="card-img-wrapper">
              <img src="https://files.catbox.moe/kufa54.jpg" alt="Band Heater" loading="lazy">
            </div>
            <div class="card-content">
              <h3>Band Heater</h3>
              <p>Pemanas berbentuk cincin yang efisien digunakan pada mesin injection molding dan extruder plastik untuk memanaskan barel.</p>
            </div>
          </div>

          <!-- Card 2 -->
          <div class="product-card">
            <div class="card-img-wrapper">
              <img src="https://files.catbox.moe/8aq9a7.jpg" alt="Cartridge Heater" loading="lazy">
            </div>
            <div class="card-content">
              <h3>Cartridge Heater</h3>
              <p>Elemen pemanas silinder berkapasitas tinggi, sangat cocok untuk pemanas cetakan (mold) dan plat industri.</p>
            </div>
          </div>

          <!-- Card 3 -->
          <div class="product-card">
            <div class="card-img-wrapper">
              <img src="https://files.catbox.moe/zyla7r.jpg" alt="Tubular Heater" loading="lazy">
            </div>
            <div class="card-content">
              <h3>Tubular Heater</h3>
              <p>Heater fleksibel berbentuk tabung yang umum digunakan untuk oven industri, pemanas air, dan sistem pemanas udara.</p>
            </div>
          </div>

          <!-- Card 4 -->
          <div class="product-card">
            <div class="card-img-wrapper">
              <img src="https://files.catbox.moe/5rfcpb.png" alt="Immersion Heater" loading="lazy">
            </div>
            <div class="card-content">
              <h3>Immersion Heater</h3>
              <p>Solusi tepat untuk memanaskan cairan langsung di dalam tangki atau bak proses industri secara efisien.</p>
            </div>
          </div>
        </div>
      </section>
    </div>

    <!-- Contact Section -->
    <section id="contact">
      <div class="section-header">
        <h2>Hubungi Kami</h2>
        <div class="separator-line"></div>
      </div>

      <div class="contact-wrapper">
        <div class="contact-info-col">
          <div class="contact-item">
            <div class="icon-box">
              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
            </div>
            <div class="contact-details">
              <h4>Email</h4>
              <p><a href="mailto:agape.oliviasukses@gmail.com">agape.oliviasukses@gmail.com</a></p>
            </div>
          </div>

          <div class="contact-item">
            <div class="icon-box">
               <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path></svg>
            </div>
            <div class="contact-details">
              <h4>Telepon / WhatsApp</h4>
              <p>
                <a href="tel:+2182582836">+21 8258 2836</a><br>
                <a href="tel:+62811186676">+62 811-1866-76</a>
              </p>
            </div>
          </div>

          <div class="contact-item">
            <div class="icon-box">
               <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
            </div>
            <div class="contact-details">
              <h4>Alamat Kantor</h4>
              <p>Perum. Mayang Pratama Blok E10 No.23, Kel. Mustikasari, Kec. Mustika Jaya, Kota Bks, Jawa Barat 17157</p>
            </div>
          </div>

          <div style="margin-top: 40px;">
            <a class="btn btn-secondary" href="mailto:agape.oliviasukses@gmail.com">
              <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="margin-right:8px"><line x1="22" y1="2" x2="11" y2="13"></line><polygon points="22 2 15 22 11 13 2 9 22 2"></polygon></svg>
              Kirim Email
            </a>
          </div>
        </div>
        
        <div class="contact-map-col">
          <div class="map-container">
            <iframe 
              src="https://maps.google.com/maps?q=Perumahan%20Mayang%20Pratama%20Blok%20E10%20No.23,%20Mustikasari,%20Kec.%20Mustika%20Jaya,%20Kota%20Bekasi,%20Jawa%20Barat&t=&z=15&ie=UTF8&iwloc=&output=embed" 
              allowfullscreen="" 
              loading="lazy"
              referrerpolicy="no-referrer-when-downgrade"
              title="Lokasi PT Agape Olivia Sukses">
            </iframe>
          </div>
        </div>
      </div>
    </section>
  </main>

  <!-- Footer -->
  <footer>
    <p>&copy; 2026 <strong>PT Agape Olivia Sukses</strong>. All rights reserved.</p>
    <p>Spesialis Heater Element & Sistem Pemanas Industri</p>
  </footer>

  <!-- Script Sederhana untuk Mobile Menu -->
  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const menuToggle = document.getElementById('mobile-menu');
      const navList = document.getElementById('nav-list');
      const navLinks = document.querySelectorAll('.nav-link');

      // Toggle menu saat hamburger diklik
      menuToggle.addEventListener('click', () => {
        navList.classList.toggle('active');
      });

      // Tutup menu saat salah satu link diklik
      navLinks.forEach(link => {
        link.addEventListener('click', () => {
          navList.classList.remove('active');
        });
      });
    });
  </script>

</body>
</html># kerja-proposal
pemanas 
