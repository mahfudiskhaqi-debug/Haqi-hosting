<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>haqi Hosting — Cepat, Stabil, Terpercaya</title>
  <meta name="description" content="haqi Hosting — solusi hosting cepat dan aman: Shared Hosting, VPS, Dedicated, Domain, dan layanan tambahan." />
  <meta name="author" content="Haqi Hosting" />
  <meta name="color-scheme" content="light dark">

  <!-- =========================
       Root variables & Styles
       ========================= -->
  <style>
    :root{
      /* warna utama dan token */
      --bg: linear-gradient(135deg, #ff6b6b 0%, #ffffff 45%, #d1d5db 100%); /* merah -> putih -> abu */
      --card: rgba(255,255,255,0.06);
      --muted: #6b7280;
      --accent-start: #ef4444;
      --accent-end: #fb7185;
      --glass: rgba(255,255,255,0.06);
      --glass-2: rgba(255,255,255,0.03);
      --radius: 12px;
      --success: #10b981;
      --danger: #ef4444;
      --shadow: 0 10px 30px rgba(2,6,23,0.08);
      --max-width: 1200px;
      --ui-sans: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
      --mono: ui-monospace, SFMono-Regular, Menlo, Monaco, 'Roboto Mono', monospace;
      --glass-border: rgba(255,255,255,0.06);
      --text: #0f1724;
      --white: #ffffff;
    }

    /* Basic reset */
    *, *::before, *::after { box-sizing: border-box; }
    html,body{height:100%}
    body{
      margin:0;
      font-family:var(--ui-sans);
      background: var(--bg);
      color:var(--text);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
      padding-bottom:120px; /* space for footer */
    }

    a{color:inherit;text-decoration:none}
    img{max-width:100%;display:block}
    button{font:inherit}

    /* Layout container */
    .container{
      width:100%;
      max-width:var(--max-width);
      margin:0 auto;
      padding:0 20px;
    }

    /* ===== Header & Navbar ===== */
    header.site-header{
      position:sticky;
      top:0;
      z-index:1000;
      backdrop-filter: blur(6px);
      background: linear-gradient(180deg, rgba(255,255,255,0.55), rgba(255,255,255,0.45));
      box-shadow: 0 2px 10px rgba(2,6,23,0.05);
    }

    .nav-row{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
      padding:16px 0;
    }

    /* Logo as typed text */
    .logo{
      display:flex;
      align-items:center;
      gap:12px;
    }
    .logo .mark{
      width:48px;height:48px;border-radius:10px;display:grid;place-items:center;
      background:linear-gradient(135deg,var(--accent-start),var(--accent-end));
      color:var(--white);font-weight:800;font-family:var(--mono);
      box-shadow: 0 6px 18px rgba(239,68,68,0.12);
    }
    .logo .title{
      line-height:1;
    }
    .logo .title .brand{font-weight:800;font-size:18px}
    .logo .title .tag{font-size:12px;color:var(--muted)}

    /* Nav links */
    nav.primary{
      display:flex;
      align-items:center;
      gap:16px;
    }
    nav.primary a{
      padding:8px 12px;border-radius:8px;color:var(--text);
      transition:all .18s ease;
      font-weight:600;
      font-size:14px;
    }
    nav.primary a:hover{ transform:translateY(-3px); box-shadow:var(--shadow) }

    /* Search */
    .search-wrap{
      display:flex;
      align-items:center;
      gap:8px;
      background:rgba(255,255,255,0.9);
      border-radius:999px;
      padding:6px;
      border:1px solid var(--glass-border);
      min-width:240px;
      max-width:460px;
    }
    .search-wrap input{
      border:0;outline:none;background:transparent;padding:8px;font-size:14px;width:100%;
    }
    .icon-btn{
      background:transparent;border:0;padding:8px;border-radius:8px;cursor:pointer;font-weight:700;
    }

    /* CTA */
    .cta{
      padding:8px 14px;border-radius:10px;background:linear-gradient(90deg,var(--accent-start),var(--accent-end));color:white;font-weight:700;border:0;cursor:pointer
    }

    /* ===== HERO ===== */
    .hero{
      display:grid;grid-template-columns:1fr 420px;gap:28px;align-items:center;padding:56px 0;
      min-height:520px;
    }
    @media (max-width:980px){ .hero{grid-template-columns:1fr; padding:32px 0} .nav-row{flex-wrap:wrap} .search-wrap{width:100%} }

    .hero-left{
      padding:24px;border-radius:16px;
      background:linear-gradient(180deg, rgba(255,255,255,0.6), rgba(255,255,255,0.5));
      box-shadow:var(--shadow);
    }
    .kicker{
      display:inline-block;padding:6px 12px;border-radius:999px;background:rgba(255,255,255,0.1);font-weight:700;color:var(--accent-start);margin-bottom:12px;font-size:13px
    }
    .hero-left h1{font-size:36px;margin:0 0 12px;line-height:1.05}
    .hero-left p.lead{color:var(--muted);margin:0 0 18px}

    .hero-actions{display:flex;gap:12px;flex-wrap:wrap}

    /* small card on right */
    .hero-card{
      padding:18px;border-radius:14px;background:rgba(255,255,255,0.95);box-shadow:var(--shadow);
    }
    .hero-card h4{margin:0 0 8px}
    .hero-card p{margin:0;color:var(--muted);font-size:14px}

    /* ===== Sections ===== */
    section.block{
      padding:56px 0;
    }
    section.block h2{font-size:28px;margin:0 0 12px;color:var(--text)}
    section.block p.lead{color:var(--muted);margin:0 0 20px}

    /* Explanation cards */
    .explain-grid{
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:18px;
      margin-top:18px;
    }
    @media (max-width:980px){ .explain-grid{grid-template-columns:repeat(2,1fr)} }
    @media (max-width:560px){ .explain-grid{grid-template-columns:1fr} }

    .explain{
      background:linear-gradient(180deg, rgba(255,255,255,0.85), rgba(255,255,255,0.82));
      border-radius:12px;padding:18px;box-shadow:var(--shadow);min-height:160px;display:flex;flex-direction:column;gap:8px;
      transition:transform .25s ease, box-shadow .25s ease;
    }
    .explain:hover{transform:translateY(-8px);box-shadow:0 20px 40px rgba(2,6,23,0.12)}
    .explain h3{margin:0;font-size:18px}
    .explain p{margin:0;color:var(--muted);font-size:14px}

    /* long text area for detailed article */
    .long-article{
      margin-top:18px;background:rgba(255,255,255,0.9);padding:20px;border-radius:12px;box-shadow:var(--shadow);line-height:1.8;color:var(--text)
    }
    .long-article h3{margin-top:18px}

    /* Feature list */
    .features-list{display:grid;grid-template-columns:repeat(2,1fr);gap:12px;margin-top:18px}
    @media (max-width:760px){ .features-list{grid-template-columns:1fr} }

    .f-item{background:rgba(255,255,255,0.95);padding:12px;border-radius:10px;border-left:4px solid rgba(239,68,68,0.9);}

    /* Pricing cards */
    .pricing-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:20px}
    @media (max-width:980px){ .pricing-grid{grid-template-columns:repeat(2,1fr)} }
    @media (max-width:760px){ .pricing-grid{grid-template-columns:1fr} }

    .price-card{background:linear-gradient(180deg, #fff, #fbfbfb);padding:18px;border-radius:12px;box-shadow:var(--shadow);display:flex;flex-direction:column;gap:12px}
    .price-card .price{font-size:28px;font-weight:800;color:var(--accent-start)}

    /* Gallery images (landscape) */
    .gallery-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:18px}
    @media (max-width:980px){ .gallery-grid{grid-template-columns:repeat(2,1fr)} }
    @media (max-width:560px){ .gallery-grid{grid-template-columns:1fr} }
    .photo-card{border-radius:12px;overflow:hidden;box-shadow:var(--shadow);position:relative}
    .photo-card .caption{position:absolute;left:12px;bottom:12px;background:rgba(0,0,0,0.45);color:white;padding:6px 10px;border-radius:8px;font-size:13px}

    /* FAQ accordion */
    .accordion{margin-top:18px}
    .acc-item{background:rgba(255,255,255,0.95);border-radius:10px;margin-bottom:8px;overflow:hidden;box-shadow:var(--shadow)}
    .acc-item button{display:flex;align-items:center;justify-content:space-between;padding:12px;border:0;width:100%;background:transparent;font-weight:700;font-size:15px}
    .acc-item .panel{padding:12px;border-top:1px solid rgba(0,0,0,0.05);color:var(--muted)}

    /* Contact / CTA */
    .contact-card{background:linear-gradient(180deg, rgba(255,255,255,0.95), rgba(255,255,255,0.9));padding:20px;border-radius:12px;box-shadow:var(--shadow)}
    .form-row{display:flex;gap:12px}
    @media (max-width:760px){ .form-row{flex-direction:column} }
    .form-row input, .form-row textarea{padding:10px;border-radius:10px;border:1px solid rgba(0,0,0,0.06);width:100%}

    /* Footer */
    footer.site-footer{
      position:fixed;left:0;right:0;bottom:0;background:linear-gradient(180deg, rgba(255,255,255,0.95), rgba(255,255,255,0.95));padding:14px 0;border-top:1px solid rgba(0,0,0,0.04);
      box-shadow:0 -6px 24px rgba(2,6,23,0.04);
    }
    footer .inner{max-width:var(--max-width);margin:0 auto;padding:0 20px;display:flex;align-items:center;justify-content:space-between;gap:12px}
    footer .small{font-size:13px;color:var(--muted)}

    /* Utility: back to top */
    .to-top{position:fixed;right:18px;bottom:84px;background:linear-gradient(90deg,var(--accent-start),var(--accent-end));color:white;padding:10px;border-radius:999px;box-shadow:var(--shadow);border:0;cursor:pointer}

    /* Animations */
    .fade-in-up{opacity:0;transform:translateY(10px);transition:opacity .6s ease, transform .6s ease}
    .in-view{opacity:1;transform:none}

    /* small screens adjustments */
    @media (max-width:560px){
      .logo .title .brand{font-size:16px}
      .hero{grid-template-columns:1fr}
    }

    /* Accessibility focus */
    a:focus, button:focus, input:focus { outline:3px solid rgba(239,68,68,0.12); outline-offset:3px; border-radius:8px }
  </style>

</head>
<body>
  <!-- Header -->
  <header class="site-header" role="banner">
    <div class="container nav-row" role="navigation" aria-label="Main navigation">
      <div class="logo" aria-hidden="false">
        <div class="mark" aria-hidden="true">HQ</div>
        <div class="title">
          <div class="brand">Haqi Hosting</div>
          <div class="tag">Cepat • Stabil • Aman</div>
        </div>
      </div>

      <nav class="primary" role="menubar" aria-label="Primary">
        <a href="#home" role="menuitem">Home</a>
        <a href="#services" role="menuitem">Layanan</a>
        <a href="#pricing" role="menuitem">Harga</a>
        <a href="#about" role="menuitem">Tentang</a>
        <a href="#contact" role="menuitem">Kontak</a>
      </nav>

      <div style="display:flex;align-items:center;gap:12px">
        <div class="search-wrap" role="search" aria-label="Cari di situs">
          <input type="search" id="globalSearch" placeholder="Cari: hosting, VPS, domain..." aria-label="Pencarian situs" />
          <button class="icon-btn" id="searchBtn" title="Search" aria-label="Search">🔎</button>
        </div>
        <button class="cta" id="signupBtn">Daftar</button>
      </div>
    </div>
  </header>

  <!-- MAIN CONTENT -->
  <main id="main" class="container" role="main">
    <!-- HERO -->
    <section id="home" class="hero" aria-labelledby="heroTitle">
      <div class="hero-left fade-in-up">
        <span class="kicker">Solusi Hosting Indonesia</span>
        <h1 id="heroTitle">haqi Hosting — Infrastruktur yang andal untuk website & aplikasi Anda</h1>
        <p class="lead">haqi Hosting menyediakan shared hosting, VPS, cloud, dan layanan domain dengan jaminan uptime tinggi, performa cepat, dan dukungan 24/7. Cocok untuk blog, toko online, aplikasi, dan perusahaan.</p>

        <div class="hero-actions">
          <button class="cta" onclick="document.getElementById('pricing').scrollIntoView({behavior:'smooth'})">Lihat Harga</button>
          <button class="icon-btn" onclick="document.getElementById('services').scrollIntoView({behavior:'smooth'})">Layanan Kami ▸</button>
          <button class="icon-btn" id="learnMoreBtn">Pelajari Lebih</button>
        </div>

        <div style="margin-top:18px;display:grid;grid-template-columns:repeat(2,1fr);gap:12px">
          <div style="padding:12px;border-radius:10px;background:rgba(255,255,255,0.9);display:flex;flex-direction:column">
            <strong>99.99% Uptime</strong>
            <span class="muted">Infrastruktur redundant & monitoring 24/7</span>
          </div>
          <div style="padding:12px;border-radius:10px;background:rgba(255,255,255,0.9);display:flex;flex-direction:column">
            <strong>Support 24/7</strong>
            <span class="muted">Bantuan cepat via chat & tiket</span>
          </div>
        </div>
      </div>

      <aside class="hero-card fade-in-up" aria-hidden="false">
        <h4>Promo Bulan Ini</h4>
        <p>Dapatkan diskon 25% untuk paket VPS pertama Anda. Gunakan kode <strong>haqi25</strong> saat checkout.</p>
        <div style="margin-top:12px;display:flex;gap:8px;align-items:center">
          <button class="cta" onclick="document.getElementById('pricing').scrollIntoView({behavior:'smooth'})">Ambil Promo</button>
          <button class="icon-btn" onclick="window.open('#contact','_self')">Hubungi Sales</button>
        </div>
      </aside>
    </section>

    <!-- Services / Explanation - long content (many paragraphs) -->
    <section id="services" class="block" aria-labelledby="servicesTitle">
      <h2 id="servicesTitle">Apa itu Hosting? & Jenis Layanan haqi Hosting</h2>
      <p class="lead">Di bagian ini kami jelaskan secara mendetail apa itu web hosting, perbedaan shared hosting, VPS, dedicated server, dan layanan tambahan seperti backup, SSL, dan managed services. Bacanya sampai habis supaya Anda paham layanan mana yang tepat untuk kebutuhan Anda.</p>

      <div class="explain-grid">
        <article class="explain fade-in-up">
          <h3>Apa itu Web Hosting?</h3>
          <p>Web hosting adalah layanan penyimpanan file website pada server agar bisa diakses melalui internet. Ketika Anda membeli hosting, Anda mendapat ruang di server, bandwidth, serta tools untuk mengelola file, database, dan email.</p>
        </article>

        <article class="explain fade-in-up">
          <h3>Shared Hosting</h3>
          <p>Paket paling ekonomis, beberapa website berbagi sumber daya server. Cocok untuk blog, situs profil, dan toko kecil. Manajemen mudah via control panel.</p>
        </article>

        <article class="explain fade-in-up">
          <h3>VPS (Virtual Private Server)</h3>
          <p>Server virtual dengan alokasi CPU, RAM, dan disk khusus. Lebih stabil dan memberi kontrol lebih dari shared hosting. Cocok buat aplikasi menengah dan toko online.</p>
        </article>

        <article class="explain fade-in-up">
          <h3>Dedicated Server</h3>
          <p>Server fisik penuh untuk kebutuhan performa dan keamanan tinggi. Dipakai perusahaan besar, aplikasi berat, atau layanan yang memerlukan kontrol penuh.</p>
        </article>

        <article class="explain fade-in-up">
          <h3>Cloud Hosting</h3>
          <p>Hosting dengan skala otomatis (auto-scaling) dan infrastruktur terdistribusi untuk ketersediaan tinggi. Cocok untuk aplikasi dengan traffic fluktuatif.</p>
        </article>

        <article class="explain fade-in-up">
          <h3>Domain & SSL</h3>
          <p>Kami juga sediakan pendaftaran domain, transfer domain, serta sertifikat SSL untuk keamanan data dan SEO.</p>
        </article>
      </div>

      <div class="long-article fade-in-up" id="longInfo">
        <h3>Panduan Lengkap: Bagaimana Memilih Hosting</h3>
        <p>Memilih hosting yang tepat bergantung pada beberapa faktor: traffic yang diharapkan, jenis aplikasi (CMS seperti WordPress, marketplace, web app), kebutuhan skalabilitas, tingkat keahlian teknis, dan budget. Berikut adalah penjelasan komprehensif untuk membantu Anda memilih:</p>

        <h4>A. Menilai kebutuhan traffic dan resource</h4>
        <p>Estimasi jumlah pengunjung per bulan, rata-rata kunjungan per hari, serta jenis konten (statis vs dinamis) menentukan kebutuhan CPU dan RAM. Toko online dan aplikasi interaktif memerlukan resource lebih besar.</p>

        <h4>B. Keamanan dan backup</h4>
        <p>Pastikan penyedia hosting menawarkan backup harian/mingguan, proteksi DDoS, dan pembaruan keamanan. haqi Hosting menawarkan backup terautomasi dan snapshot VPS berdasarkan paket.</p>

        <h4>C. Support & manajemen</h4>
        <p>Support 24/7 penting ketika terjadi gangguan. Bagi yang tidak mau pusing mengelola server, fitur managed hosting termasuk patching, monitoring, dan optimasi performa sangat berguna.</p>

        <h4>D. Skalabilitas</h4>
        <p>Pilih layanan yang memungkinkan upgrade sumber daya tanpa downtime signifikan. Cloud hosting kami mendukung auto-scaling untuk beban puncak.</p>

        <h3>Contoh kasus pemilihan</h3>
        <ol>
          <li>Blog pribadi & portofolio — Shared hosting paket BASIC cukup.</li>
          <li>Toko online kecil (20-200 produk) — Shared+ atau VPS kecil dengan caching dan CDN.</li>
          <li>Aplikasi web & startup — VPS/Cloud dengan auto-scaling.</li>
          <li>Platform enterprise — Dedicated atau private cloud.</li>
        </ol>

        <h3>Performa teknis</h3>
        <p>Kami menggunakan SSD NVMe pada semua server, HTTP/2 & HTTP/3 bila memungkinkan, serta cache tingkat server untuk meningkatkan kecepatan. Selain itu, jaringan fiber & peering regional menjamin latensi rendah untuk pengguna di Indonesia.</p>

        <h3>Keamanan</h3>
        <p>Segala layanan kami dilengkapi dengan firewall, WAF (opsional), SSL gratis, dan proteksi bot. Kami juga memberikan rekomendasi konfigurasi keamanan untuk CMS populer.</p>

        <h3>Penutup</h3>
        <p>Semoga penjelasan ini membantu Anda menentukan pilihan. Jika ragu, tim sales kami siap memberi rekomendasi gratis berdasarkan pola traffic dan kebutuhan teknis Anda.</p>
      </div>

      <!-- features list -->
      <div class="features-list" aria-hidden="false">
        <div class="f-item fade-in-up">
          <strong>Monitoring 24/7</strong>
          <div class="muted">Kami memantau server setiap saat untuk mendeteksi dan memperbaiki gangguan lebih cepat.</div>
        </div>
        <div class="f-item fade-in-up">
          <strong>Jaringan Peering</strong>
          <div class="muted">Koneksi cepat ke ISP lokal dan internasional dengan peering berkualitas.</div>
        </div>
        <div class="f-item fade-in-up">
          <strong>Backup Otomatis</strong>
          <div class="muted">Backup harian & snapshot tersedia sesuai paket.</div>
        </div>
        <div class="f-item fade-in-up">
          <strong>Garansi Refund</strong>
          <div class="muted">30 hari garansi uang kembali tanpa alasan untuk paket shared hosting.</div>
        </div>
      </div>

    </section>

    <!-- Pricing -->
    <section id="pricing" class="block" aria-labelledby="pricingTitle">
      <h2 id="pricingTitle">Harga dan Paket</h2>
      <p class="lead">Pilih paket yang paling sesuai. Semua paket bisa di-upgrade kapan saja.</p>

      <div class="pricing-grid">
        <div class="price-card fade-in-up">
          <div style="display:flex;justify-content:space-between;align-items:center">
            <div><strong>Shared BASIC</strong><div class="muted">Untuk pemula</div></div>
            <div class="badge" style="background:linear-gradient(90deg,#ffd1d1,#ffbaba);padding:6px 10px;border-radius:8px;font-weight:700">Popular</div>
          </div>
          <div class="price">Rp 19.000<span style="font-size:12px;font-weight:600;color:var(--muted)">/bln</span></div>
          <div>Disk 5GB NVMe • Bandwidth 100GB • 10 database</div>
          <div style="margin-top:auto"><button class="cta">Pilih Paket</button></div>
        </div>

        <div class="price-card fade-in-up">
          <div style="display:flex;justify-content:space-between;align-items:center">
            <div><strong>Shared PRO</strong><div class="muted">Toko online kecil</div></div>
          </div>
          <div class="price">Rp 49.000<span style="font-size:12px;font-weight:600;color:var(--muted)">/bln</span></div>
          <div>Disk 20GB NVMe • Bandwidth 500GB • 50 database</div>
          <div style="margin-top:auto"><button class="cta">Pilih Paket</button></div>
        </div>

        <div class="price-card fade-in-up">
          <div style="display:flex;justify-content:space-between;align-items:center">
            <div><strong>VPS START</strong><div class="muted">Lebih kontrol & performa</div></div>
          </div>
          <div class="price">Rp 149.000<span style="font-size:12px;font-weight:600;color:var(--muted)">/bln</span></div>
          <div>2 vCPU • 4GB RAM • 80GB NVMe</div>
          <div style="margin-top:auto"><button class="cta">Pilih Paket</button></div>
        </div>
      </div>

      <p style="margin-top:12px;color:var(--muted)">Catatan: Harga bisa berubah sesuai promosi. Harga di atas hanya contoh demo.</p>
    </section>

    <!-- Gallery of landscapes -->
    <section id="gallery" class="block" aria-labelledby="galleryTitle">
      <h2 id="galleryTitle">Galeri Pemandangan (Contoh Foto untuk Website)</h2>
      <p class="lead">Foto-foto pemandangan ini hanya ilustrasi untuk menunjukkan bagaimana website Anda akan tampil dengan gambar berkualitas tinggi.</p>

      <div class="gallery-grid">
        <figure class="photo-card fade-in-up">
          <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?w=1200&q=80&auto=format&fit=crop" alt="Sunset mountain" />
          <figcaption class="caption">Pegunungan senja</figcaption>
        </figure>

        <figure class="photo-card fade-in-up">
          <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?w=1200&q=80&auto=format&fit=crop" alt="Ocean waves" />
          <figcaption class="caption">Ombak biru</figcaption>
        </figure>

        <figure class="photo-card fade-in-up">
          <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?w=1200&q=80&auto=format&fit=crop" alt="Forest path" />
          <figcaption class="caption">Jalan hutan</figcaption>
        </figure>

        <figure class="photo-card fade-in-up">
          <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?w=1200&q=80&auto=format&fit=crop&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8bW91bnRhaW58ZW58MHx8MHx8" alt="Valley" />
          <figcaption class="caption">Lembah hijau</figcaption>
        </figure>

        <figure class="photo-card fade-in-up">
          <img src="https://images.unsplash.com/photo-1499346030926-9a72daac6c63?w=1200&q=80&auto=format&fit=crop" alt="Lake" />
          <figcaption class="caption">Danau tenang</figcaption>
        </figure>

        <figure class="photo-card fade-in-up">
          <img src="https://images.unsplash.com/photo-1470770903676-69b98201ea1c?w=1200&q=80&auto=format&fit=crop" alt="Desert dunes" />
          <figcaption class="caption">Gurun bertekstur</figcaption>
        </figure>
      </div>
    </section>

    <!-- FAQ / Accordion (long) -->
    <section id="faq" class="block" aria-labelledby="faqTitle">
      <h2 id="faqTitle">Pertanyaan Umum (FAQ)</h2>
      <p class="lead">Pertanyaan yang sering ditanyakan calon pelanggan kami.</p>

      <div class="accordion">
        <div class="acc-item fade-in-up">
          <button aria-expanded="false">Apa perbedaan Shared Hosting dan VPS? <span class="muted">▸</span></button>
          <div class="panel" hidden>
            <p>Shared hosting artinya beberapa pengguna berbagi sumber daya server. VPS memberikan sumber daya virtual khusus sehingga stabilitas dan performa lebih terjaga.</p>
          </div>
        </div>

        <div class="acc-item fade-in-up">
          <button aria-expanded="false">Apakah kalian menyediakan layanan migrasi website? <span class="muted">▸</span></button>
          <div class="panel" hidden>
            <p>Kami menyediakan migrasi gratis untuk paket tertentu. Tim teknis akan bantu memindahkan file dan database tanpa downtime signifikan.</p>
          </div>
        </div>

        <div class="acc-item fade-in-up">
          <button aria-expanded="false">Bagaimana proses klaim refund? <span class="muted">▸</span></button>
          <div class="panel" hidden>
            <p>Ajukan tiket pada dashboard dalam waktu 30 hari, tim billing akan memproses sesuai syarat dan ketentuan.</p>
          </div>
        </div>

        <div class="acc-item fade-in-up">
          <button aria-expanded="false">Apakah ada garansi uptime? <span class="muted">▸</span></button>
          <div class="panel" hidden>
            <p>Kami menjamin SLA 99.9% untuk paket VPS dan dedicated. Detail SLA ada di halaman Terms of Service.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact / CTA with form -->
    <section id="contact" class="block" aria-labelledby="contactTitle">
      <h2 id="contactTitle">Hubungi Kami</h2>
      <p class="lead">Tim sales & support siap membantu. Isi formulir di bawah atau gunakan chat di pojok kanan bawah.</p>

      <div class="contact-card fade-in-up">
        <form id="contactForm" onsubmit="return handleContactSubmit(event)">
          <div class="form-row">
            <input type="text" id="cname" placeholder="Nama lengkap" required />
            <input type="email" id="cemail" placeholder="Email" required />
          </div>
          <div style="margin-top:12px">
            <input type="text" id="csubject" placeholder="Subjek" required />
          </div>
          <div style="margin-top:12px">
            <textarea id="cmessage" rows="5" placeholder="Tulis pesan Anda..." required></textarea>
          </div>
          <div style="margin-top:12px;display:flex;gap:8px;align-items:center">
            <button class="cta" type="submit">Kirim Pesan</button>
            <button type="button" class="icon-btn" onclick="document.getElementById('contactForm').reset()">Reset</button>
            <div class="muted" id="contactNote" style="font-size:13px">Kami akan merespon dalam 24 jam kerja.</div>
          </div>
        </form>
      </div>

    </section>

    <!-- Extra long content: in-depth technical articles (to lengthen) -->
    <section id="deepdive" class="block" aria-labelledby="deepTitle">
      <h2 id="deepTitle">Deep Dive: Infrastruktur Teknis haqi Hosting</h2>
      <p class="lead">Untuk Anda yang ingin tahu lebih teknis — arsitektur, jaringan, backup, dan best practices.</p>

      <div class="long-article fade-in-up">
        <h3>1. Arsitektur Server</h3>
        <p>Kami menggunakan arsitektur multi-availability zone dengan load balancer front-end, layer cache (Redis / Varnish), dan backend server yang terukur. Database dipisahkan pada node dedicated untuk keandalan.</p>

        <h3>2. Jaringan & Peering</h3>
        <p>Peering lokal dan internasional memberikan rute terpendek ke ISP. Monitoring BGP & route analytics memastikan rute terbaik untuk paket data Anda.</p>

        <h3>3. Backup & Disaster Recovery</h3>
        <p>Snapshot harian dan retention policy configurable. Untuk VPS dan dedicated, kami sediakan opsi off-site backup untuk DR (Disaster Recovery).</p>

        <h3>4. Security & Compliance</h3>
        <p>Firewall, WAF, otentikasi dua faktor (2FA), enkripsi at-rest (disk), dan enkripsi in transit (TLS) adalah standar. Kami juga membantu audit security untuk client enterprise.</p>

        <h3>5. Monitoring & Alerting</h3>
        <p>Service monitoring menggunakan tools industry-standard. Event alert dikirim via SMS, email, dan dashboard realtime.</p>

        <h3>6. DevOps & Automation</h3>
        <p>CI/CD pipelines, automated provisioning, dan Infrastructure as Code (IaC) untuk deployment reproducible dan cepat.</p>

        <h3>7. Skenario skala</h3>
        <p>Kami mendukung vertical scaling dan horizontal scaling lengkap dengan session management dan sticky sessions bila diperlukan.</p>

        <h3>8. Contoh Implementasi</h3>
        <p>Contoh: migrasi aplikasi monolit menjadi microservices, memecah database menjadi primary-read replicas, dan memanfaatkan CDN untuk konten statis.</p>

        <p style="margin-top:18px">Jika Anda ingin diskusi teknis lebih mendalam, tim kami siap mengadakan sesi konsultasi terstruktur (berbayar/komersial) atau sesi discovery gratis untuk proposal.</p>
      </div>

    </section>

  </main>

  <!-- Back to top & Floating chat placeholder -->
  <button class="to-top" id="toTop" title="Kembali ke atas" aria-label="Kembali ke atas">↑</button>

  <!-- Footer -->
  <footer class="site-footer" role="contentinfo">
    <div class="inner">
      <div>
        <strong>HAQI Hosting</strong>
        <div class="small">Jalan Dermawan Gresik no 1 jl supratman• support@haqihosting.example</div>
      </div>
      <div style="text-align:right">
        <div class="small">© <span id="year"></span> haqi Hosting. All rights reserved.</div>
        <div class="small muted">Syarat & Ketentuan • Kebijakan Privasi</div>
      </div>
    </div>
  </footer>

  <!-- ======================
       JavaScript (interactions)
       ====================== -->
  <script>
    // Helpers
    const inViewObserver = new IntersectionObserver((entries)=>{
      entries.forEach(e=>{
        if(e.isIntersecting){
          e.target.classList.add('in-view');
        }
      });
    }, {threshold:0.12});

    // Attach observer to fade-in elements
    document.querySelectorAll('.fade-in-up').forEach(el=> inViewObserver.observe(el));

    // Accordion behaviour
    document.querySelectorAll('.acc-item button').forEach(btn=>{
      btn.addEventListener('click', ()=> {
        const expanded = btn.getAttribute('aria-expanded') === 'true';
        btn.setAttribute('aria-expanded', (!expanded).toString());
        const panel = btn.nextElementSibling;
        if(!panel) return;
        if(expanded){
          panel.hidden = true;
        } else {
          panel.hidden = false;
        }
      });
    });

    // Back to top
    document.getElementById('toTop').addEventListener('click', ()=> window.scrollTo({top:0,behavior:'smooth'}));

    // Contact form submit (demo)
    function handleContactSubmit(e){
      e.preventDefault();
      const name = document.getElementById('cname').value.trim();
      const email = document.getElementById('cemail').value.trim();
      const subj = document.getElementById('csubject').value.trim();
      const msg = document.getElementById('cmessage').value.trim();
      if(!name || !email || !subj || !msg){ alert('Lengkapi semua field.'); return false; }
      // For demo: just show a message and reset
      document.getElementById('contactNote').textContent = 'Terima kasih, pesan terkirim. Kami akan menghubungi ' + name + ' melalui ' + email + '.';
      document.getElementById('contactForm').reset();
      // In production: send to API endpoint
      return false;
    }

    // Global search (simple filter: scroll to first matching section or highlight)
    document.getElementById('searchBtn').addEventListener('click', runSearch);
    document.getElementById('globalSearch').addEventListener('keydown', (e)=>{ if(e.key === 'Enter') runSearch(); });

    function runSearch(){
      const q = document.getElementById('globalSearch').value.trim().toLowerCase();
      if(!q){ alert('Masukkan kata kunci pencarian.'); return; }
      // Search in headings & paragraphs
      const selectors = 'main h2, main h3, main p, main li';
      const nodes = Array.from(document.querySelectorAll(selectors));
      const found = nodes.find(n => (n.textContent || '').toLowerCase().includes(q));
      if(found){
        found.scrollIntoView({behavior:'smooth', block:'center'});
        // briefly flash
        const orig = found.style.transition;
        found.style.transition = 'background .4s ease';
        found.style.background = 'rgba(255,230,230,0.6)';
        setTimeout(()=>{ found.style.background = ''; found.style.transition = orig; }, 1200);
      } else {
        alert('Tidak ditemukan: ' + q + '. Coba kata kunci lain.');
      }
    }

    // Year in footer
    document.getElementById('year').textContent = new Date().getFullYear();

    // Smooth internal anchor: enhance all nav links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', (e)=>{
        const href = a.getAttribute('href');
        if(href === '#') return;
        const el = document.querySelector(href);
        if(el){
          e.preventDefault();
          el.scrollIntoView({behavior:'smooth', block:'start'});
        }
      });
    });

    // Simple scrollspy highlight nav (optional)
    const sections = Array.from(document.querySelectorAll('main > section.block, main > section'));
    const navLinks = Array.from(document.querySelectorAll('nav.primary a'));
    const spyObs = new IntersectionObserver((entries)=>{
      entries.forEach(ent=>{
        if(ent.isIntersecting){
          const id = ent.target.id;
          navLinks.forEach(link=>{
            link.style.opacity = link.getAttribute('href') === '#' + id ? '1' : '0.6';
          });
        }
      });
    }, {threshold:0.3});
    sections.forEach(s => spyObs.observe(s));

    // Small UX: smooth reveal of hero when clicking learnMore
    document.getElementById('learnMoreBtn').addEventListener('click', ()=>{
      document.getElementById('services').scrollIntoView({behavior:'smooth'});
    });

    // Ensure images lazy-load progressively for performance
    document.addEventListener('DOMContentLoaded', ()=>{
      const imgs = Array.from(document.querySelectorAll('img'));
      imgs.forEach((img, i)=>{
        // small stagger
        setTimeout(()=>{ img.loading = 'lazy'; }, i*80);
      });
    });

    // Optional: keyboard shortcut "/" focuses search
    window.addEventListener('keydown', (e)=>{
      if(e.key === '/' && document.activeElement.tagName.toLowerCase() !== 'input' && document.activeElement.tagName.toLowerCase() !== 'textarea'){
        e.preventDefault();
        document.getElementById('globalSearch').focus();
      }
    });

    // small accessibility improvement: ensure all buttons have accessible names (already labeled)
    // End of interactive scripts
  </script>

  <!-- End of file -->
</body>
</html>
