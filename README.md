# Website-Personal
Web
<!DOCTYPE html>
<html>

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title></title>
</head>

<body>
  
</body>

</html><!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Rehan Pernandes | Portfolio & Data Diri</title>
    <!-- Font Awesome 6 (free) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Google Fonts: Poppins & Space Grotesk untuk sentuhan modern -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&family=Space+Grotesk:wght@400;500;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(145deg, #0a0515 0%, #170b2a 100%);
            color: #f0eaff;
            line-height: 1.5;
            scroll-behavior: smooth;
        }

        /* Custom scroll */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #2a1a42;
            border-radius: 10px;
        }
        ::-webkit-scrollbar-thumb {
            background: #aa66ff;
            border-radius: 10px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #c084fc;
        }

        /* Dekorasi bintang / titik ungu */
        .bg-bling {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
            overflow: hidden;
        }
        .bg-bling span {
            position: absolute;
            background: rgba(170, 102, 255, 0.2);
            border-radius: 50%;
            animation: floatGlow 12s infinite alternate ease-in-out;
        }
        @keyframes floatGlow {
            0% { transform: translateY(0px) scale(1); opacity: 0.2; }
            100% { transform: translateY(-40px) scale(1.2); opacity: 0.6; }
        }

        .container {
            max-width: 1300px;
            margin: 0 auto;
            padding: 2rem 2rem 3rem;
            position: relative;
            z-index: 2;
        }

        /* header + navbar */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-bottom: 3rem;
            background: rgba(25, 12, 48, 0.5);
            backdrop-filter: blur(12px);
            border-radius: 70px;
            padding: 0.8rem 2rem;
            border: 1px solid rgba(160, 100, 255, 0.4);
            box-shadow: 0 10px 25px -5px rgba(0,0,0,0.3);
        }
        .logo h1 {
            font-size: 1.8rem;
            font-weight: 700;
            background: linear-gradient(135deg, #e2b0ff, #aa66ff);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            letter-spacing: -0.5px;
        }
        .logo p {
            font-size: 0.75rem;
            color: #c7b0ff;
            letter-spacing: 1px;
        }
        .nav-links a {
            color: #e2d6ff;
            margin-left: 2rem;
            text-decoration: none;
            font-weight: 500;
            transition: 0.3s;
            font-size: 1rem;
        }
        .nav-links a:hover {
            color: #d78cff;
            text-shadow: 0 0 6px #b77eff;
        }
        .btn-contact {
            background: linear-gradient(95deg, #9b4dff, #c66eff);
            padding: 0.5rem 1.4rem;
            border-radius: 40px;
            font-weight: 600;
            box-shadow: 0 4px 12px rgba(156, 78, 255, 0.4);
        }
        .btn-contact:hover {
            background: linear-gradient(95deg, #b05eff, #da8aff);
            transform: scale(1.02);
        }

        /* Hero section */
        .hero {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            gap: 3rem;
            margin: 2rem 0 4rem;
        }
        .hero-left {
            flex: 1.2;
        }
        .hero-left .badge {
            background: rgba(156, 78, 255, 0.25);
            backdrop-filter: blur(4px);
            display: inline-block;
            padding: 0.3rem 1rem;
            border-radius: 30px;
            font-size: 0.8rem;
            font-weight: 500;
            margin-bottom: 1rem;
            border-left: 3px solid #c273ff;
        }
        .hero-left h1 {
            font-size: 3.3rem;
            font-weight: 800;
            line-height: 1.2;
            margin-bottom: 1rem;
        }
        .gradient-text {
            background: linear-gradient(125deg, #f0b3ff, #bc7aff);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        .hero-left p {
            font-size: 1.1rem;
            color: #cdbef5;
            margin: 1rem 0 2rem;
            max-width: 500px;
        }
        .hero-stats {
            display: flex;
            gap: 1.5rem;
            margin-top: 1rem;
        }
        .stat {
            background: rgba(60, 30, 100, 0.5);
            backdrop-filter: blur(8px);
            padding: 0.5rem 1rem;
            border-radius: 2rem;
            font-weight: 500;
        }
        .hero-right {
            flex: 0.9;
            display: flex;
            justify-content: center;
        }
        .avatar-frame {
            background: linear-gradient(145deg, #b46eff, #642bb3);
            padding: 6px;
            border-radius: 38% 62% 70% 30% / 42% 40% 60% 58%;
            animation: morph 8s infinite alternate;
            box-shadow: 0 20px 35px -10px rgba(106, 13, 173, 0.6);
        }
        .avatar-frame img {
            width: 280px;
            height: 280px;
            object-fit: cover;
            border-radius: 38% 62% 70% 30% / 42% 40% 60% 58%;
            background: #1f0e3a;
            display: block;
        }
        @keyframes morph {
            0% { border-radius: 38% 62% 70% 30% / 42% 40% 60% 58%; }
            100% { border-radius: 55% 45% 35% 65% / 55% 55% 45% 45%; }
        }

        /* Card Section */
        .section-title {
            font-size: 2rem;
            font-weight: 700;
            margin: 3rem 0 1.5rem;
            position: relative;
            display: inline-block;
        }
        .section-title:after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 60%;
            height: 4px;
            background: linear-gradient(90deg, #b66aff, #e69eff);
            border-radius: 5px;
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }
        .card {
            background: rgba(30, 16, 56, 0.65);
            backdrop-filter: blur(12px);
            border-radius: 2rem;
            padding: 1.8rem;
            border: 1px solid rgba(160, 100, 255, 0.35);
            transition: all 0.3s ease;
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);
        }
        .card:hover {
            transform: translateY(-6px);
            border-color: #c47eff;
            background: rgba(45, 24, 82, 0.8);
            box-shadow: 0 25px 40px -12px #a05eff40;
        }
        .card-icon {
            font-size: 2.5rem;
            color: #cb91ff;
            margin-bottom: 1rem;
        }
        .card h3 {
            font-size: 1.5rem;
            margin-bottom: 0.7rem;
        }
        .detail-item {
            margin: 0.8rem 0;
            display: flex;
            align-items: center;
            gap: 0.8rem;
            flex-wrap: wrap;
            word-break: break-word;
        }
        .detail-item i {
            width: 28px;
            color: #cb91ff;
            font-size: 1.2rem;
        }

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 0.7rem;
            margin-top: 1rem;
        }
        .skill-tag {
            background: #2f1a55;
            padding: 0.4rem 1rem;
            border-radius: 40px;
            font-size: 0.8rem;
            font-weight: 500;
            color: #e6ceff;
        }

        /* Sosmed & WA */
        .social-links {
            display: flex;
            gap: 1.2rem;
            margin-top: 1.5rem;
            flex-wrap: wrap;
        }
        .social-btn {
            background: rgba(0,0,0,0.35);
            padding: 0.7rem 1.5rem;
            border-radius: 60px;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            text-decoration: none;
            color: white;
            font-weight: 500;
            transition: 0.2s;
            border: 1px solid #b675ff;
        }
        .social-btn i {
            font-size: 1.2rem;
        }
        .social-btn.wa:hover {
            background: #25D366;
            border-color: #25D366;
        }
        .social-btn.ig:hover {
            background: radial-gradient(circle at 30% 110%, #ffdb7e, #ff9b4a, #d62976);
            border-color: #ffb86b;
        }
        .social-btn.github:hover {
            background: #171515;
            border-color: #f0eaff;
        }

        /* testimoni / kutipan */
        .quote-block {
            background: linear-gradient(120deg, #311c62, #1f0e44);
            border-radius: 2rem;
            padding: 2rem;
            margin: 2rem 0;
            text-align: center;
            border-left: 6px solid #cb7eff;
        }
        .quote-block i {
            font-size: 2rem;
            color: #cb7eff;
            margin-bottom: 1rem;
        }

        footer {
            margin-top: 4rem;
            text-align: center;
            padding-top: 1.5rem;
            border-top: 1px solid #4a2b7a;
            font-size: 0.85rem;
            color: #b8a2e6;
        }

        @media (max-width: 800px) {
            .container { padding: 1.5rem; }
            .navbar { flex-direction: column; border-radius: 2rem; }
            .nav-links a { margin: 0 1rem; }
            .hero-left h1 { font-size: 2.2rem; }
            .avatar-frame img { width: 220px; height: 220px; }
            .section-title { font-size: 1.7rem; }
        }
        @media (max-width: 550px) {
            .hero-stats { flex-direction: column; gap: 0.5rem; }
        }
        .btn-hire {
            background: linear-gradient(90deg, #aa66ff, #cd8eff);
            border: none;
            padding: 0.8rem 1.8rem;
            border-radius: 40px;
            font-weight: bold;
            color: #130b21;
            cursor: pointer;
            transition: 0.2s;
            font-family: inherit;
            margin-top: 1rem;
            box-shadow: 0 6px 14px #a05eff55;
        }
        .btn-hire:hover {
            transform: scale(1.02);
            background: linear-gradient(90deg, #bc7aff, #dfa0ff);
        }
    </style>
</head>
<body>

<div class="bg-bling" id="particles-bg"></div>

<div class="container">
    <!-- Navbar -->
    <div class="navbar">
        <div class="logo">
            <h1>REHAN PERNANDES</h1>
            <p>✦ Fullstack Creator ✦</p>
        </div>
        <div class="nav-links">
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#data">Data Diri</a>
            <a href="#contact" class="btn-contact">Kontak</a>
        </div>
    </div>

    <!-- Hero Section / Home -->
    <div id="home" class="hero">
        <div class="hero-left">
            <div class="badge">
                <i class="fas fa-code"></i>  Web Expert • Freelance
            </div>
            <h1>Halo, Saya <span class="gradient-text">Rehan</span><br>Pembuat Website Kreatif</h1>
            <p>Membangun website impian untuk klien dari Indonesia hingga mancanegara. Saya hadir untuk mewujudkan ide digitalmu menjadi nyata.</p>
            <div class="hero-stats">
                <div class="stat"><i class="fas fa-globe"></i> 15+ Project</div>
                <div class="stat"><i class="fas fa-users"></i> 12+ Klien Puas</div>
                <div class="stat"><i class="fas fa-laptop-code"></i> 24/7 Support</div>
            </div>
            <button class="btn-hire" id="scrollToContact"><i class="fab fa-whatsapp"></i>  Hubungi via WA</button>
        </div>
        <div class="hero-right">
            <div class="avatar-frame">
                <!-- Avatar placeholder dengan inisial R dengan gaya modern, karena tidak ada foto asli, buat ilustrasi ungu -->
                <img src="https://ui-avatars.com/api/?background=8b5cf6&color=fff&bold=true&size=280&name=Rehan+P&length=2&fontsize=0.33&rounded=true" alt="Rehan Pernandes">
            </div>
        </div>
    </div>

    <!-- About Section -->
    <div id="about">
        <div class="section-title">Tentang Saya</div>
        <div class="info-grid">
            <div class="card">
                <div class="card-icon"><i class="fas fa-user-astronaut"></i></div>
                <h3>Who Am I?</h3>
                <p>Saya Rehan Pernandes, anak ke-2 dari keluarga di Bengkulu. Berusia 17 tahun dengan semangat muda yang membara untuk menjadi programmer sukses. Saya percaya bahwa kode bukan sekadar baris, tapi seni membangun solusi.</p>
            </div>
            <div class="card">
                <div class="card-icon"><i class="fas fa-bullseye"></i></div>
                <h3>Misi & Visi</h3>
                <p>💜 Menjadi programmer kelas dunia dari Bengkulu. 💜 Membantu orang Indonesia & luar negeri dalam membangun website modern. 💜 Sukses di bidang programming dan membanggakan keluarga.</p>
            </div>
            <div class="card">
                <div class="card-icon"><i class="fas fa-laptop"></i></div>
                <h3>Keahlian</h3>
                <div class="skills">
                    <span class="skill-tag">HTML/CSS</span>
                    <span class="skill-tag">Tailwind</span>
                    <span class="skill-tag">JavaScript</span>
                    <span class="skill-tag">React.js</span>
                    <span class="skill-tag">Node.js</span>
                    <span class="skill-tag">PHP & MySQL</span>
                    <span class="skill-tag">UI/UX Design</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Data Diri & Portofolio detail -->
    <div id="data">
        <div class="section-title">Data Diri & Informasi</div>
        <div class="info-grid">
            <div class="card">
                <div class="card-icon"><i class="fas fa-id-card"></i></div>
                <h3>Biodata</h3>
                <div class="detail-item"><i class="fas fa-user"></i> Nama: <strong>Rehan Pernandes</strong></div>
                <div class="detail-item"><i class="fas fa-calendar-alt"></i> Umur: <strong>17 Tahun</strong></div>
                <div class="detail-item"><i class="fas fa-baby-carriage"></i> Anak Ke: <strong>2 dari bersaudara</strong></div>
                <div class="detail-item"><i class="fas fa-map-marker-alt"></i> Alamat: <strong>Bengkulu, Indonesia</strong></div>
                <div class="detail-item"><i class="fas fa-briefcase"></i> Pekerjaan: <strong>Web Developer Freelance (Indonesia & International)</strong></div>
            </div>
            <div class="card">
                <div class="card-icon"><i class="fas fa-rocket"></i></div>
                <h3>Portofolio Highlights</h3>
                <div class="detail-item"><i class="fas fa-check-circle"></i> Website Company Profile - PT Maju Jaya</div>
                <div class="detail-item"><i class="fas fa-check-circle"></i> E-commerce UMKM Madu Asli</div>
                <div class="detail-item"><i class="fas fa-check-circle"></i> Landing Page Agency Luar Negeri (Australia)</div>
                <div class="detail-item"><i class="fas fa-check-circle"></i> Sistem Informasi Sekolah (Laravel)</div>
                <div class="detail-item"><i class="fas fa-check-circle"></i> Dashboard Admin + API Integration</div>
                <div class="social-links" style="margin-top: 12px;">
                    <span style="font-size: 0.8rem;"><i class="fab fa-github"></i> github/rehanpernandes (coming soon)</span>
                </div>
            </div>
            <div class="card">
                <div class="card-icon"><i class="fas fa-heart"></i></div>
                <h3>Quote & Motivasi</h3>
                <p><i class="fas fa-quote-left"></i> "Saya ingin sukses di bidang programmer, karena dari situlah saya bisa memberikan dampak besar untuk orang banyak dan keluarga. Terus belajar dan berkarya tanpa batas."</p>
                <hr style="margin: 1rem 0; border-color:#5c3c9e;">
                <div class="detail-item"><i class="fas fa-language"></i> Bahasa: Indonesia, English (Intermediate)</div>
                <div class="detail-item"><i class="fas fa-certificate"></i> Sertifikat: Web Development Bootcamp 2024</div>
            </div>
        </div>
    </div>

    <!-- Kontak + Sosmed -->
    <div id="contact">
        <div class="section-title">Hubungi Saya</div>
        <div class="card" style="background: rgba(45, 25, 85, 0.8);">
            <div class="card-icon"><i class="fas fa-address-card"></i></div>
            <h3>Mari Berkolaborasi!</h3>
            <p>Saya terbuka untuk proyek website, entah untuk keperluan pribadi, bisnis, atau start-up. Hubungi saya sekarang untuk mendapatkan website keren dan profesional.</p>
            <div class="social-links">
                <a href="https://wa.me/6285123256703?text=Halo%20Rehan,%20saya%20tertarik%20dengan%20layanan%20website%20Anda!" class="social-btn wa" target="_blank" rel="noopener noreferrer">
                    <i class="fab fa-whatsapp"></i> WhatsApp: +62851-2325-6703
                </a>
                <a href="https://www.instagram.com/_reh4npernandes?igsh=MWt2amdzMDBoMjcyeA==" class="social-btn ig" target="_blank" rel="noopener noreferrer">
                    <i class="fab fa-instagram"></i> Instagram @_reh4npernandes
                </a>
                <a href="#" class="social-btn github" onclick="copyEmailAlert()">
                    <i class="fas fa-envelope"></i> rehan@devportfolio.my.id
                </a>
            </div>
            <div class="detail-item" style="margin-top: 1rem;">
                <i class="fas fa-clock"></i> Respon cepat: <strong> biasanya < 1 jam (via WA)</strong>
            </div>
        </div>
        <div class="quote-block">
            <i class="fas fa-star-of-life"></i>
            <h3>"Bikin website untuk orang luar maupun orang Indonesia"</h3>
            <p>— Rehan Pernandes, Developer Muda dari Bengkulu —</p>
        </div>
    </div>

    <footer>
        <p>© 2025 Rehan Pernandes | Dibuat dengan <i class="fas fa-heart" style="color:#cd8eff"></i> menggunakan kode dan kreativitas | Author: Rehan Pernandes</p>
        <p style="margin-top: 0.5rem;"><i class="fas fa-code-branch"></i> Semangat programmer sukses 2025 ✨</p>
    </footer>
</div>

<script>
    // Membuat efek bintang latar belakang dengan DOM
    function createBling() {
        const container = document.getElementById('particles-bg');
        if(!container) return;
        const count = 80;
        for(let i=0; i<count; i++) {
            let span = document.createElement('span');
            let size = Math.random() * 30 + 8;
            span.style.width = size + 'px';
            span.style.height = size + 'px';
            span.style.left = Math.random() * 100 + '%';
            span.style.top = Math.random() * 100 + '%';
            span.style.animationDuration = Math.random() * 12 + 6 + 's';
            span.style.animationDelay = Math.random() * 5 + 's';
            span.style.opacity = Math.random() * 0.4 + 0.1;
   
