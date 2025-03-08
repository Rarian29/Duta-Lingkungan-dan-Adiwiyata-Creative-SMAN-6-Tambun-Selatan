<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Duta Lingkungan & Adiwiyata Creative SMAN 6 Tambun Selatan</title>
    <style>
        /* Font imports */
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        /* Base styles */
        :root {
            --primary-color: #2e7d32;
            --secondary-color: #81c784;
            --accent-color: #388e3c;
            --text-color: #333;
            --bg-color: #f8f9fa;
            --light-green: #e8f5e9;
            --white: #ffffff;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            background-color: var(--primary-color);
            color: var(--white);
            padding: 20px 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo h1 {
            font-size: 24px;
            font-weight: 600;
        }
        
        .logo span {
            display: block;
            font-size: 14px;
            font-weight: 400;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 30px;
        }
        
        nav ul li a {
            color: var(--white);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--light-green);
        }
        
        .mobile-menu {
            display: none;
            font-size: 24px;
            cursor: pointer;
        }
        
        /* Hero section */
        .hero {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: var(--white);
            padding: 80px 0;
            text-align: center;
        }
        
        .hero h2 {
            font-size: 40px;
            margin-bottom: 20px;
            font-weight: 700;
        }
        
        .hero p {
            font-size: 18px;
            max-width: 800px;
            margin: 0 auto 30px;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--white);
            color: var(--primary-color);
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
            margin: 10px;
        }
        
        .btn:hover {
            background-color: var(--light-green);
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        /* About section */
        .about {
            padding: 80px 0;
            background-color: var(--white);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }
        
        .section-title h3 {
            font-size: 32px;
            font-weight: 600;
            color: var(--primary-color);
        }
        
        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background-color: var(--secondary-color);
            margin: 15px auto 0;
            border-radius: 2px;
        }
        
        .about-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 30px;
        }
        
        .about-text {
            flex: 1;
            min-width: 300px;
        }
        
        .about-text p {
            margin-bottom: 20px;
        }
        
        /* Green Project section */
        .green-project {
            padding: 80px 0;
            background-color: var(--light-green);
        }
        
        .project-card {
            background-color: var(--white);
            border-radius: 10px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
        }
        
        .project-card h4 {
            font-size: 22px;
            margin-bottom: 15px;
            color: var(--primary-color);
        }
        
        .project-card p {
            margin-bottom: 20px;
        }
        
        /* Duta section */
        .duta-section {
            padding: 80px 0;
            background-color: var(--white);
        }
        
        .duta-periods {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }
        
        .period {
            background-color: var(--light-green);
            border-radius: 10px;
            padding: 30px;
            width: 100%;
            max-width: 350px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .period h4 {
            font-size: 20px;
            margin-bottom: 20px;
            color: var(--primary-color);
            text-align: center;
        }
        
        .duta-name {
            margin-bottom: 10px;
            padding: 10px;
            background-color: var(--white);
            border-radius: 8px;
        }
        
        .duta-name p {
            margin-bottom: 5px;
            font-weight: 500;
        }
        
        .duta-name span {
            font-size: 14px;
            color: #666;
        }
        
        /* Video section */
        .video-section {
            padding: 80px 0;
            background-color: var(--light-green);
            text-align: center;
        }
        
        .video-container {
            margin-top: 30px;
        }
        
        /* Social Media section */
        .social-media {
            padding: 80px 0;
            background-color: var(--white);
        }
        
        .social-icons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 30px;
        }
        
        .social-icon {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
            background-color: var(--light-green);
            border-radius: 10px;
            width: 200px;
            transition: transform 0.3s;
            text-decoration: none;
            color: var(--text-color);
        }
        
        .social-icon:hover {
            transform: translateY(-5px);
        }
        
        .social-icon i {
            font-size: 36px;
            margin-bottom: 10px;
            color: var(--primary-color);
        }
        
        .social-icon h4 {
            margin-bottom: 5px;
        }
        
        .social-icon p {
            font-size: 14px;
            text-align: center;
        }
        
        /* Contact section */
        .contact {
            padding: 80px 0;
            background-color: var(--light-green);
        }
        
        .contact-info {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 40px;
            margin-top: 30px;
        }
        
        .contact-card {
            background-color: var(--white);
            border-radius: 10px;
            padding: 30px;
            width: 100%;
            max-width: 350px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            text-align: center;
        }
        
        .contact-card i {
            font-size: 36px;
            color: var(--primary-color);
            margin-bottom: 15px;
        }
        
        .contact-card h4 {
            margin-bottom: 10px;
            font-size: 20px;
        }
        
        .contact-card p, .contact-card a {
            color: #666;
            text-decoration: none;
        }
        
        .contact-card a:hover {
            color: var(--primary-color);
        }
        
        /* Footer */
        footer {
            background-color: var(--primary-color);
            color: var(--white);
            padding: 40px 0;
            text-align: center;
        }
        
        .footer-content {
            margin-bottom: 20px;
        }
        
        .copyright {
            font-size: 14px;
            border-top: 1px solid rgba(255,255,255,0.1);
            padding-top: 20px;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 20px;
                flex-wrap: wrap;
                justify-content: center;
            }
            
            nav ul li {
                margin: 5px 10px;
            }
            
            .hero h2 {
                font-size: 32px;
            }
            
            .about-content {
                flex-direction: column;
            }
            
            .period {
                max-width: 100%;
            }
            
            .social-icons {
                flex-direction: column;
                align-items: center;
            }
        }
        
        @media (max-width: 576px) {
            .btn {
                display: block;
                margin: 10px auto;
                max-width: 200px;
            }
            
            .section-title h3 {
                font-size: 28px;
            }
        }
    </style>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <h1>Duta Lingkungan & Adiwiyata Creative</h1>
                    <span>SMAN 6 Tambun Selatan</span>
                </div>
                <nav>
                    <ul>
                        <li><a href="#about">Tentang</a></li>
                        <li><a href="#green-project">Green Project</a></li>
                        <li><a href="#duta">Duta Lingkungan</a></li>
                        <li><a href="#video">Video</a></li>
                        <li><a href="#social">Media Sosial</a></li>
                        <li><a href="#contact">Kontak</a></li>
                    </ul>
                </nav>
                <div class="mobile-menu">
                    <i class="fas fa-bars"></i>
                </div>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h2>Peduli Lingkungan, Ciptakan Perubahan</h2>
            <p>Kami adalah tim Duta Lingkungan dan Adiwiyata Creative SMAN 6 Tambun Selatan yang berkomitmen untuk melestarikan lingkungan dan menciptakan kesadaran melalui berbagai kegiatan lingkungan yang kreatif.</p>
            <a href="#green-project" class="btn">Green Project</a>
            <a href="#contact" class="btn">Hubungi Kami</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <div class="container">
            <div class="section-title">
                <h3>Tentang Kami</h3>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <p>Duta Lingkungan SMAN 6 Tambun Selatan adalah perwakilan siswa terpilih yang berperan sebagai contoh dan penggerak dalam menjaga lingkungan sekolah. Mereka bertugas menginspirasi siswa lain untuk lebih peduli terhadap lingkungan sekitar.</p>
                    <p>Sementara itu, Tim Adiwiyata Creative adalah kelompok siswa kreatif yang mengembangkan konten dan kampanye digital untuk meningkatkan kesadaran lingkungan di kalangan siswa dan masyarakat.</p>
                    <p>Bersama-sama, Duta Lingkungan dan Tim Adiwiyata Creative bekerja sama untuk mewujudkan visi sekolah yang berwawasan lingkungan dengan menghadirkan berbagai program kreatif yang bermanfaat.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Green Project Section -->
    <section id="green-project" class="green-project">
        <div class="container">
            <div class="section-title">
                <h3>Green Project 🌿</h3>
            </div>
            <div class="project-card">
                <h4>Tentang Green Project</h4>
                <p>Green Project adalah inisiatif digital dari Tim Adiwiyata Creative dan Duta Lingkungan SMAN 6 Tambun Selatan. Program ini bertujuan untuk menyebarkan pesan-pesan kepedulian lingkungan melalui platform media sosial dan aktivitas digital lainnya.</p>
                <p>Melalui konten kreatif dan informatif, kami mengajak semua siswa dan masyarakat untuk lebih peduli terhadap lingkungan sekitar dan mulai melakukan aksi nyata untuk masa depan bumi yang lebih baik.</p>
                <a href="http://bit.ly/4icFdFg" class="btn" target="_blank">Kunjungi Green Project</a>
            </div>
        </div>
    </section>

    <!-- Duta Lingkungan Section -->
    <section id="duta" class="duta-section">
        <div class="container">
            <div class="section-title">
                <h3>Duta Lingkungan</h3>
            </div>
            <div class="duta-periods">
                <div class="period">
                    <h4>Periode 2021/2022</h4>
                    <div class="duta-name">
                        <p>Rizki Maulana</p>
                        <span>XII IPS 4</span>
                    </div>
                    <div class="duta-name">
                        <p>Vareza Maylina</p>
                        <span>XII IPA 5</span>
                    </div>
                </div>
                
                <div class="period">
                    <h4>Periode 2023/2024</h4>
                    <div class="duta-name">
                        <p>Raafi Febrian</p>
                        <span>XI.4</span>
                    </div>
                    <div class="duta-name">
                        <p>Kayla Putri Zafira</p>
                        <span>XII IPS 4</span>
                    </div>
                </div>
                
                <div class="period">
                    <h4>Periode 2024/2025</h4>
                    <div class="duta-name">
                        <p>Adhi Kurnia Nugraha</p>
                        <span>XI.3</span>
                    </div>
                    <div class="duta-name">
                        <p>Siregar, Tiara Anastasia Enjelika</p>
                        <span>XI.5</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Video Section -->
    <section id="video" class="video-section">
        <div class="container">
            <div class="section-title">
                <h3>Video Profil Sekolah Adiwiyata</h3>
            </div>
            <p>Lihat bagaimana SMAN 6 Tambun Selatan menerapkan program Adiwiyata dalam keseharian sekolah melalui video profil kami.</p>
            <div class="video-container">
                <a href="https://youtu.be/Q7H7QpRoF8U?si=PEtp1gWiC-ncEfTC" class="btn" target="_blank">Tonton Video Profil</a>
            </div>
        </div>
    </section>

    <!-- Social Media Section -->
    <section id="social" class="social-media">
        <div class="container">
            <div class="section-title">
                <h3>Media Sosial</h3>
            </div>
            <p>Ikuti aktivitas Duta Lingkungan SMAN 6 Tambun Selatan di media sosial untuk mendapatkan informasi terbaru tentang program dan kegiatan kami.</p>
            <div class="social-icons">
                <a href="https://www.instagram.com/dutalingkungan.smansix?igsh=cHVibnpyY3p4Y3Z2" class="social-icon" target="_blank">
                    <i class="fab fa-instagram"></i>
                    <h4>Instagram</h4>
                    <p>@dutalingkungan.smansix</p>
                </a>
                
                <a href="https://www.tiktok.com/@dutalingkungan.smansix?_t=ZS-8uWG2s" class="social-icon" target="_blank">
                    <i class="fab fa-tiktok"></i>
                    <h4>TikTok</h4>
                    <p>@dutalingkungan.smansix</p>
                </a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <div class="section-title">
                <h3>Kontak Kami</h3>
            </div>
            <div class="contact-info">
                <div class="contact-card">
                    <i class="fas fa-envelope"></i>
                    <h4>Email</h4>
                    <a href="mailto:dutalingkungansmansix@gmail.com">dutalingkungansmansix@gmail.com</a>
                </div>
                
                <div class="contact-card">
                    <i class="fas fa-school"></i>
                    <h4>Sekolah</h4>
                    <p>SMAN 6 Tambun Selatan</p>
                    <p>Jl. Raya Jatimulya, RT.001/RW.013, Jatimulya, Kec. Tambun Sel., Kota Bks, Jawa Barat 17510</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <h3>Duta Lingkungan & Adiwiyata Creative</h3>
                <p>SMAN 6 Tambun Selatan</p>
            </div>
            <div class="copyright">
                <p>&copy; 2025 Duta Lingkungan & Adiwiyata Creative SMAN 6 Tambun Selatan. Hak Cipta Dilindungi.</p>
            </div>
        </div>
    </footer>

    <script>
        // Simple mobile menu toggle
        document.querySelector('.mobile-menu').addEventListener('click', function() {
            document.querySelector('nav ul').classList.toggle('show');
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
