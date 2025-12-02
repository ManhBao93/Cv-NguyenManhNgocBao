<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Trang web cá nhân của TS. Nguyễn Mạnh Ngọc Bảo - Giảng viên, Nhà nghiên cứu">
    <title>TS. Nguyễn Mạnh Ngọc Bảo | Trang cá nhân</title>
    
    <!-- ===== CSS NHÚNG ===== -->
    <style>
        /* ===== RESET & BASE STYLES ===== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.7;
            color: #333;
            background-color: #fafbfc;
        }

        /* ===== CONTAINER CHÍNH ===== */
        .container {
            max-width: 1150px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* ===== HEADER & NAVBAR ===== */
        header {
            background: #ffffff;
            box-shadow: 0 2px 10px rgba(0,0,0,0.08);
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
            max-width: 1150px;
            margin: 0 auto;
        }

        .logo {
            font-size: 1.3rem;
            font-weight: 700;
            color: #2563eb;
            text-decoration: none;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 25px;
            align-items: center;
        }

        .nav-links a {
            text-decoration: none;
            color: #555;
            font-size: 0.95rem;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: #2563eb;
        }

        .btn-cv {
            background: #2563eb;
            color: #fff !important;
            padding: 8px 18px;
            border-radius: 6px;
            transition: background 0.3s ease, transform 0.2s ease;
        }

        .btn-cv:hover {
            background: #1d4ed8;
            transform: translateY(-2px);
        }

        /* Mobile menu button */
        .menu-toggle {
            display: none;
            flex-direction: column;
            cursor: pointer;
            gap: 5px;
        }

        .menu-toggle span {
            width: 25px;
            height: 3px;
            background: #333;
            border-radius: 3px;
            transition: 0.3s;
        }

        /* ===== HERO SECTION - GIỚI THIỆU ===== */
        #about {
            padding: 140px 0 80px;
            background: linear-gradient(135deg, #f8fafc 0%, #e8f4f8 100%);
        }

        .hero-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }

        /* Ảnh chân dung bo tròn */
        .profile-photo {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid #e0e0e0;
            margin-bottom: 25px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
        }

        .hero-content h1 {
            font-size: 2.2rem;
            color: #1e293b;
            margin-bottom: 10px;
        }

        .hero-content .title {
            font-size: 1.15rem;
            color: #2563eb;
            font-weight: 600;
            margin-bottom: 8px;
        }

        .hero-content .affiliation {
            font-size: 1rem;
            color: #64748b;
            margin-bottom: 25px;
        }

        .hero-content .affiliation span {
            display: block;
        }

        .intro-text {
            max-width: 800px;
            font-size: 1.05rem;
            color: #475569;
            line-height: 1.8;
            margin-bottom: 30px;
            text-align: justify;
        }

        /* Social links / Icon liên kết */
        .social-links {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
            justify-content: center;
        }

        .social-links a {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 10px 18px;
            background: #fff;
            border: 1px solid #e2e8f0;
            border-radius: 8px;
            text-decoration: none;
            color: #475569;
            font-size: 0.9rem;
            transition: all 0.3s ease;
        }

        .social-links a:hover {
            background: #2563eb;
            color: #fff;
            border-color: #2563eb;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(37,99,235,0.3);
        }

        .social-links svg {
            width: 18px;
            height: 18px;
        }

        /* ===== SECTION CHUNG ===== */
        section {
            padding: 80px 0;
        }

        section:nth-child(even) {
            background: #fff;
        }

        .section-title {
            font-size: 1.8rem;
            color: #1e293b;
            margin-bottom: 40px;
            text-align: center;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background: #2563eb;
            margin: 15px auto 0;
            border-radius: 2px;
        }

        /* ===== LÝ LỊCH KHOA HỌC ===== */
        #profile {
            background: #fff;
        }

        .profile-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 40px;
        }

        .profile-card {
            background: #f8fafc;
            padding: 30px;
            border-radius: 12px;
            border-left: 4px solid #2563eb;
        }

        .profile-card h3 {
            font-size: 1.25rem;
            color: #1e293b;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .profile-card h3 svg {
            width: 24px;
            height: 24px;
            color: #2563eb;
        }

        .profile-card ul {
            list-style: none;
        }

        .profile-card li {
            padding: 10px 0;
            border-bottom: 1px solid #e2e8f0;
            color: #475569;
            font-size: 0.95rem;
        }

        .profile-card li:last-child {
            border-bottom: none;
        }

        .profile-card li strong {
            color: #1e293b;
        }

        /* Research interests - full width */
        .research-interests {
            grid-column: 1 / -1;
            background: linear-gradient(135deg, #eff6ff 0%, #f0fdf4 100%);
            border-left-color: #10b981;
        }

        .research-interests h3 svg {
            color: #10b981;
        }

        .research-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 15px;
        }

        .research-list li {
            background: #fff;
            padding: 15px 20px;
            border-radius: 8px;
            border-bottom: none;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05);
        }

        /* ===== CÔNG BỐ KHOA HỌC ===== */
        #publications {
            background: #f8fafc;
        }

        .pub-category {
            margin-bottom: 40px;
        }

        .pub-category h3 {
            font-size: 1.2rem;
            color: #2563eb;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid #e2e8f0;
        }

        .publication-item {
            background: #fff;
            padding: 20px 25px;
            margin-bottom: 15px;
            border-radius: 10px;
            border-left: 3px solid #10b981;
            box-shadow: 0 2px 8px rgba(0,0,0,0.04);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .publication-item:hover {
            transform: translateX(5px);
            box-shadow: 0 5px 20px rgba(0,0,0,0.08);
        }

        .publication-item p {
            color: #475569;
            font-size: 0.95rem;
            line-height: 1.7;
        }

        /* ===== GIẢNG DẠY ===== */
        #teaching {
            background: #fff;
        }

        .teaching-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 20px;
            margin-bottom: 40px;
        }

        .course-card {
            background: #f8fafc;
            padding: 25px;
            border-radius: 12px;
            transition: transform 0.3s ease;
        }

        .course-card:hover {
            transform: translateY(-5px);
        }

        .course-card h4 {
            color: #1e293b;
            font-size: 1.05rem;
            margin-bottom: 10px;
        }

        .course-card .level {
            display: inline-block;
            background: #dbeafe;
            color: #2563eb;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            margin-bottom: 10px;
        }

        .course-card .role {
            color: #64748b;
            font-size: 0.9rem;
        }

        .teaching-philosophy {
            background: linear-gradient(135deg, #eff6ff 0%, #f0fdf4 100%);
            padding: 35px;
            border-radius: 12px;
            border-left: 4px solid #2563eb;
        }

        .teaching-philosophy h3 {
            color: #1e293b;
            margin-bottom: 15px;
            font-size: 1.2rem;
        }

        .teaching-philosophy p {
            color: #475569;
            font-style: italic;
            line-height: 1.8;
        }

        /* ===== DỰ ÁN - HỢP TÁC ===== */
        #projects {
            background: #f8fafc;
        }

        .project-item {
            background: #fff;
            padding: 30px;
            margin-bottom: 20px;
            border-radius: 12px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }

        .project-item:hover {
            transform: translateY(-3px);
        }

        .project-item h4 {
            color: #1e293b;
            font-size: 1.1rem;
            margin-bottom: 15px;
        }

        .project-meta {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 15px;
        }

        .project-meta span {
            display: flex;
            align-items: center;
            gap: 6px;
            color: #64748b;
            font-size: 0.9rem;
        }

        .project-meta svg {
            width: 16px;
            height: 16px;
            color: #2563eb;
        }

        .collaboration-invite {
            background: linear-gradient(135deg, #2563eb 0%, #10b981 100%);
            color: #fff;
            padding: 40px;
            border-radius: 12px;
            margin-top: 40px;
            text-align: center;
        }

        .collaboration-invite h3 {
            font-size: 1.3rem;
            margin-bottom: 15px;
        }

        .collaboration-invite p {
            max-width: 700px;
            margin: 0 auto;
            line-height: 1.8;
            opacity: 0.95;
        }

        /* ===== LIÊN HỆ ===== */
        #contact {
            background: #fff;
        }

        .contact-wrapper {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
        }

        .contact-info h3 {
            color: #1e293b;
            font-size: 1.3rem;
            margin-bottom: 25px;
        }

        .contact-item {
            display: flex;
            align-items: flex-start;
            gap: 15px;
            margin-bottom: 20px;
        }

        .contact-item svg {
            width: 22px;
            height: 22px;
            color: #2563eb;
            flex-shrink: 0;
            margin-top: 3px;
        }

        .contact-item div {
            color: #475569;
        }

        .contact-item strong {
            display: block;
            color: #1e293b;
            margin-bottom: 3px;
        }

        .contact-item a {
            color: #2563eb;
            text-decoration: none;
        }

        .contact-item a:hover {
            text-decoration: underline;
        }

        /* Form liên hệ */
        .contact-form h3 {
            color: #1e293b;
            font-size: 1.3rem;
            margin-bottom: 25px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            color: #475569;
            margin-bottom: 8px;
            font-weight: 500;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #e2e8f0;
            border-radius: 8px;
            font-size: 1rem;
            font-family: inherit;
            transition: border-color 0.3s ease, box-shadow 0.3s ease;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #2563eb;
            box-shadow: 0 0 0 3px rgba(37,99,235,0.1);
        }

        .form-group textarea {
            min-height: 120px;
            resize: vertical;
        }

        .btn-submit {
            background: #2563eb;
            color: #fff;
            border: none;
            padding: 14px 35px;
            font-size: 1rem;
            font-weight: 600;
            border-radius: 8px;
            cursor: pointer;
            transition: background 0.3s ease, transform 0.2s ease;
        }

        .btn-submit:hover {
            background: #1d4ed8;
            transform: translateY(-2px);
        }

        /* ===== FOOTER ===== */
        footer {
            background: #1e293b;
            color: #94a3b8;
            text-align: center;
            padding: 30px 20px;
        }

        footer p {
            font-size: 0.9rem;
        }

        /* ===== RESPONSIVE DESIGN ===== */
        @media (max-width: 992px) {
            .profile-grid {
                grid-template-columns: 1fr;
            }

            .contact-wrapper {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 768px) {
            .menu-toggle {
                display: flex;
            }

            .nav-links {
                position: absolute;
                top: 100%;
                left: 0;
                right: 0;
                background: #fff;
                flex-direction: column;
                padding: 20px;
                gap: 15px;
                box-shadow: 0 10px 20px rgba(0,0,0,0.1);
                display: none;
            }

            .nav-links.active {
                display: flex;
            }

            .hero-content h1 {
                font-size: 1.8rem;
            }

            .section-title {
                font-size: 1.5rem;
            }

            section {
                padding: 60px 0;
            }

            #about {
                padding: 120px 0 60px;
            }

            .teaching-grid {
                grid-template-columns: 1fr;
            }

            .project-meta {
                flex-direction: column;
                gap: 10px;
            }

            .social-links {
                flex-direction: column;
                align-items: center;
            }

            .social-links a {
                width: 100%;
                max-width: 280px;
                justify-content: center;
            }
        }

        @media (max-width: 480px) {
            .navbar {
                padding: 12px 15px;
            }

            .logo {
                font-size: 1.1rem;
            }

            .profile-photo {
                width: 140px;
                height: 140px;
            }

            .hero-content h1 {
                font-size: 1.5rem;
            }

            .profile-card,
            .project-item,
            .teaching-philosophy {
                padding: 20px;
            }
        }
    </style>
</head>
<body>

    <!-- ===== HEADER & THANH MENU ===== -->
    <header>
        <nav class="navbar">
            <!-- Logo chữ -->
            <a href="#about" class="logo">TS. Nguyễn Mạnh Ngọc Bảo</a>
            
            <!-- Nút menu mobile -->
            <div class="menu-toggle" onclick="toggleMenu()">
                <span></span>
                <span></span>
                <span></span>
            </div>
            
            <!-- Danh sách menu -->
            <ul class="nav-links" id="navLinks">
                <li><a href="#about">Giới thiệu</a></li>
                <li><a href="#profile">Lý lịch khoa học</a></li>
                <li><a href="#publications">Công bố khoa học</a></li>
                <li><a href="#teaching">Giảng dạy</a></li>
                <li><a href="#projects">Dự án – Hợp tác</a></li>
                <li><a href="#contact">Liên hệ</a></li>
                <li><a href="cv.pdf" class="btn-cv" target="_blank">Tải CV</a></li>
            </ul>
        </nav>
    </header>

    <!-- ===== PHẦN GIỚI THIỆU (Hero Section) ===== -->
    <section id="about">
        <div class="container">
            <div class="hero-content">
                <!-- Ảnh chân dung -->
                <img 
                    src="https://drive.google.com/thumbnail?id=1MSWEwEKwoUpo5q5p7sqpssGa0toAf6k3&sz=w400" 
                    alt="TS. Nguyễn Mạnh Ngọc Bảo" 
                    class="profile-photo"
                >
                
                <!-- Họ tên -->
                <h1>TS. Nguyễn Mạnh Ngọc Bảo</h1>
                
                <!-- Chức danh -->
                <p class="title">Tổng giám đốc | Giảng viên</p>
                
                <!-- Đơn vị công tác -->
                <p class="affiliation">
                    <span>Công ty TNHH MTV An Bảo Đặc khu Phú Quốc</span>
                    <span>Khoa Khoa học Ứng dụng và Công nghệ, Trường Đại học Nguyễn Tất Thành</span>
                </p>
                
                <!-- Đoạn giới thiệu ngắn -->
                <p class="intro-text">
                    Tôi là Tiến sĩ Nguyễn Mạnh Ngọc Bảo, Tổng giám đốc Công ty TNHH MTV An Bảo đặc khu Phú Quốc, kiêm giảng viên trường đại học Nguyễn Tất Thành và là nhà nghiên cứu trong lĩnh vực Công nghệ thực phẩm và logistics, quản lý chuỗi cung ứng và phát triển bền vững. Mối quan tâm nghiên cứu của tôi tập trung vào định hướng ứng dụng phát triển những sản phẩm thực phẩm bền vững, tận dụng phụ phẩm trong nông nghiệp để phát triển sản phẩm mới, cải thiện giá trị sản phẩm. Thêm vào đó, tôi có kinh nghiệm trong logistics xanh, chuỗi cung ứng nông sản tại Đồng bằng sông Cửu Long và mô hình phát triển bền vững cho các đảo du lịch như Phú Quốc.
                </p>
                
                <!-- Icon liên kết nhanh -->
                <div class="social-links">
                    <a href="mailto:nmnbao@ntt.edu.vn">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/>
                        </svg>
                        Email
                    </a>
                    <a href="https://scholar.google.com/citations?user=lygtBUwAAAAJ&hl=vi" target="_blank">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M12 24a7 7 0 110-14 7 7 0 010 14zm0-24L0 9.5l4.838 3.94A8 8 0 0112 9a8 8 0 017.162 4.44L24 9.5 12 0z"/>
                        </svg>
                        Google Scholar
                    </a>
                    <a href="https://orcid.org/0009-0007-7609-9616" target="_blank">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M12 0C5.372 0 0 5.372 0 12s5.372 12 12 12 12-5.372 12-12S18.628 0 12 0zM7.369 4.378a.815.815 0 110 1.63.815.815 0 010-1.63zm-.625 3.056h1.25v8.505h-1.25V7.434zm3.625 0h3.379c3.057 0 4.502 2.096 4.502 4.252 0 2.398-1.727 4.253-4.502 4.253h-3.379V7.434zm1.25 1.055v6.395h2.003c2.241 0 3.378-1.412 3.378-3.198 0-1.78-1.137-3.197-3.378-3.197h-2.003z"/>
                        </svg>
                        ORCID
                    </a>
                    <a href="https://www.linkedin.com/in/bao-nguyen-54861337a" target="_blank">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
                        </svg>
                        LinkedIn
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- ===== PHẦN LÝ LỊCH KHOA HỌC ===== -->
    <section id="profile">
        <div class="container">
            <h2 class="section-title">Lý lịch khoa học</h2>
            
            <div class="profile-grid">
                <!-- Học vấn -->
                <div class="profile-card">
                    <h3>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path d="M12 14l9-5-9-5-9 5 9 5z"/>
                            <path d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"/>
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14l9-5-9-5-9 5 9 5zm0 0l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14zm-4 6v-7.5l4-2.222"/>
                        </svg>
                        Học vấn
                    </h3>
                    <ul>
                        <li><strong>Tiến sĩ Quản lý Công nghệ</strong><br>Trường Đại học Akamai, Hoa Kỳ</li>
                        <li><strong>Tiến sĩ Quản lý</strong><br>Trường Đại học Quốc tế Châu Âu, Pháp</li>
                        <li><strong>Thạc sĩ Phát triển sản phẩm Công-Nông nghiệp</strong><br>Đại học Kasetsart, Thái Lan</li>
                        <li><strong>Kỹ sư Công nghệ Thực phẩm tiên tiến</strong><br>Trường Đại học Nông Lâm TP.HCM</li>
                        <li><strong>Cử nhân ngành Luật</strong><br>Đại học Đà Nẵng</li>
                        <li><strong>Cử nhân Ngôn ngữ Anh</strong><br>Đại học Đà Nẵng</li>
                        <li><strong>Cử nhân Kế Toán</strong><br>Đại học Đà Nẵng</li>
                    </ul>
                </div>

                <!-- Quá trình công tác -->
                <div class="profile-card">
                    <h3>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/>
                        </svg>
                        Quá trình công tác
                    </h3>
                    <ul>
                        <li><strong>2023 – nay:</strong> Giảng viên, Khoa Khoa học Ứng dụng và Công nghệ, Trường Đại học Nguyễn Tất Thành Việt Nam</li>
                        <li><strong>2019 – nay:</strong> Tổng giám đốc, lĩnh vực Xây dựng, Xăng Dầu, Nghiên cứu khoa học, Du lịch, Kinh doanh nhà hàng khách sạn resort, Công ty TNHH MTV An Bảo - Đặc khu Phú Quốc</li>
                        <li><strong>2025 – nay:</strong> Nghiên cứu sinh, ngành Vận tải và Logistics, Đại học Khoa học công nghệ Malaysia</li>
                        <li><strong>2025 – nay:</strong> Nghiên cứu sinh, ngành Công nghệ thực phẩm, Đại học Cần Thơ</li>
                        <li><strong>2019 – 2022:</strong> Nhân viên kiểm nghiệm, Kiểm nghiệm thực phẩm, môi trường, nghiên cứu khoa học, Trung tâm Ứng Dụng Khoa học Công nghệ và Môi trường - CN Phú Quốc</li>
                    </ul>
                </div>

                <!-- Hướng nghiên cứu chính -->
                <div class="profile-card research-interests">
                    <h3>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z"/>
                        </svg>
                        Hướng nghiên cứu chính
                    </h3>
                    <ul class="research-list">
                        <li>Phát triển sản phẩm mới trong thực phẩm, tận dụng phụ phẩm trong nông nghiệp để phát triển sản phẩm bền vững</li>
                        <li>Phân tích và tối ưu chuỗi cung ứng nông sản, đặc biệt là sầu riêng vùng Đồng bằng sông Cửu Long</li>
                        <li>Phát triển hạ tầng và dịch vụ logistics hỗ trợ du lịch và thương mại tại các đảo như Phú Quốc</li>
                        <li>Ứng dụng công nghệ số và dữ liệu lớn trong quản trị chuỗi cung ứng</li>
                        <li>Kết nối logistics – du lịch – bất động sản trong phát triển địa phương bền vững</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- ===== PHẦN CÔNG BỐ KHOA HỌC ===== -->
    <section id="publications">
        <div class="container">
            <h2 class="section-title">Công bố khoa học</h2>
            
            <!-- Bài báo quốc tế -->
            <div class="pub-category">
                <h3>Bài báo quốc tế (ISI/Scopus)</h3>
                
                <div class="publication-item">
                    <p>Nguyen, B. M. N., & Pirak, T. (2019). Physicochemical properties and antioxidant activities of white dragon fruit peel pectin extracted with conventional and ultrasound-assisted extraction. <em>Cogent Food & Agriculture</em>, 5(1), 1633076.</p>
                </div>
                
                <div class="publication-item">
                    <p>Thai, L. T., Nguyen, A. T., Nguyen, B. M. N., Truong, H. T., & Le, A. Q. (2025). Role of mangrovian biodiversity, ecological distribution and abundance, for promising sea reclamation: A case study in sea west of Kien Giang Province. In <em>Geography, Earth Science and Environment: Research Highlights</em> (Vol. 4, pp. 166–194). BP International.</p>
                </div>
                
                <div class="publication-item">
                    <p>Thai, L. T., Danh, M., Dang, N. T. H., Ngo, T. V., Nguyen, B. M. N., & Truong, H. T. (2024). Researching the structure of species to propose exploitation the potential to expand natural land by polder from mangroves in the Western Mekong Delta of Vietnam. <em>International Journal of Membrane Science and Technology</em>, 11(1), 857–870.</p>
                </div>
                
                <div class="publication-item">
                    <p>Thai, T. T., & Nguyen, B. M. N. (2024). Researching the structure of species to propose exploitation the potential for food and medicine and to expand natural land by polder from mangroves in the Western Mekong Delta of Vietnam. <em>Preprints</em>, 2024, 202401.1552.</p>
                </div>
                
                <div class="publication-item">
                    <p>Thai, L. T., Danh, M., Dang, N. T. H., Ngo, T. V., Nguyen, B. M. N., Truong, H. T., & Le, A. Q. (2024). Researching the structure of species to propose exploitation the potential to expand natural land by polder from mangroves in the Western Mekong Delta of Vietnam. <em>Research Square</em> (preprint), doi:10.21203/rs.3.rs-5309474.v1.</p>
                </div>
                
                <div class="publication-item">
                    <p>Dang, N. T. H., Thai, L. T., Danh, M., Ngo, T. V., & Nguyen, B. M. N. (2025). Biochar of reed (Phragmites autralis) on representative locations in Mekong Delta of Vietnam. <em>Journal of Ecohumanism</em>, 4(1), 499–516.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- ===== PHẦN GIẢNG DẠY ===== -->
    <section id="teaching">
        <div class="container">
            <h2 class="section-title">Giảng dạy</h2>
            
            <!-- Danh sách học phần -->
            <div class="teaching-grid">
                <div class="course-card">
                    <span class="level">Bậc Đại học</span>
                    <h4>Đánh giá cảm quan, phát triển sản phẩm mới</h4>
                    <p class="role">Giảng viên phụ trách chính</p>
                </div>
                
                <div class="course-card">
                    <span class="level">Bậc Đại học</span>
                    <h4>Logistics trong kinh doanh nông sản thực phẩm</h4>
                    <p class="role">Giảng viên phụ trách chính</p>
                </div>
                
                <div class="course-card">
                    <span class="level">Bậc Đại học</span>
                    <h4>Quản trị vận tải và phân phối</h4>
                    <p class="role">Đồng giảng</p>
                </div>
                
                <div class="course-card">
                    <span class="level">Bậc Sau đại học</span>
                    <h4>Phân tích dữ liệu trong logistics và chuỗi cung ứng</h4>
                    <p class="role">Giảng viên phụ trách</p>
                </div>
                
                <div class="course-card">
                    <span class="level">Bậc Sau đại học</span>
                    <h4>Phương pháp nghiên cứu khoa học trong kinh doanh và logistics</h4>
                    <p class="role">Giảng viên phụ trách</p>
                </div>
            </div>
            
            <!-- Triết lý giảng dạy -->
            <div class="teaching-philosophy">
                <h3>Quan điểm & Triết lý giảng dạy</h3>
                <p>"Tôi ưu tiên phương pháp giảng dạy gắn với thực tiễn doanh nghiệp, khuyến khích sinh viên tự học, tự nghiên cứu và làm việc nhóm. Các tình huống thực tế từ chuỗi cung ứng nông sản, logistics tại đảo Phú Quốc và vùng Đồng bằng sông Cửu Long được tích hợp vào bài giảng nhằm giúp người học hiểu sâu vấn đề và rèn luyện năng lực giải quyết vấn đề."</p>
            </div>
        </div>
    </section>

    <!-- ===== PHẦN DỰ ÁN - HỢP TÁC ===== -->
    <section id="projects">
        <div class="container">
            <h2 class="section-title">Dự án – Hợp tác</h2>
            
            <!-- Danh sách dự án -->
            <div class="project-item">
                <h4>Phân tích và tối ưu chuỗi cung ứng sầu riêng vùng Đồng bằng sông Cửu Long</h4>
                <div class="project-meta">
                    <span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"/>
                        </svg>
                        Vai trò: Chủ nhiệm đề tài
                    </span>
                    <span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"/>
                        </svg>
                        Thời gian: 2022–2024
                    </span>
                    <span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/>
                        </svg>
                        Nguồn tài trợ: Quỹ nghiên cứu cấp Bộ
                    </span>
                </div>
            </div>
            
            <div class="project-item">
                <h4>Phát triển mô hình logistics xanh hỗ trợ du lịch bền vững tại đảo Phú Quốc</h4>
                <div class="project-meta">
                    <span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"/>
                        </svg>
                        Vai trò: Đồng chủ nhiệm
                    </span>
                    <span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"/>
                        </svg>
                        Thời gian: 2021–2023
                    </span>
                    <span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/>
                        </svg>
                        Nguồn tài trợ: Đề tài cấp tỉnh
                    </span>
                </div>
            </div>
            
            <div class="project-item">
                <h4>Ứng dụng công nghệ số trong quản trị tồn kho và vận tải cho doanh nghiệp xăng dầu ven biển</h4>
                <div class="project-meta">
                    <span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"/>
                        </svg>
                        Vai trò: Thành viên chính
                    </span>
                    <span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"/>
                        </svg>
                        Thời gian: 2019–2021
                    </span>
                    <span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/>
                        </svg>
                        Nguồn tài trợ: Doanh nghiệp
                    </span>
                </div>
            </div>
            
            <!-- Lời mời hợp tác -->
            <div class="collaboration-invite">
                <h3>Cơ hội hợp tác</h3>
                <p>Tôi sẵn sàng hợp tác nghiên cứu và tư vấn trong các lĩnh vực Xăng dầu, kinh doanh – du lịch tại đặc khu Phú Quốc, Công nghệ thực phẩm, logistics, quản lý chuỗi cung ứng, phát triển bền vững nông nghiệp – du lịch và chuyển đổi số trong logistics. Các tổ chức, doanh nghiệp và đồng nghiệp quan tâm có thể liên hệ để trao đổi thêm về cơ hội hợp tác đầu tư, nghiên cứu, đào tạo và chuyển giao.</p>
            </div>
        </div>
    </section>

    <!-- ===== PHẦN LIÊN HỆ ===== -->
    <section id="contact">
        <div class="container">
            <h2 class="section-title">Liên hệ</h2>
            
            <div class="contact-wrapper">
                <!-- Thông tin liên hệ -->
                <div class="contact-info">
                    <h3>Thông tin liên hệ</h3>
                    
                    <div class="contact-item">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"/>
                        </svg>
                        <div>
                            <strong>Họ tên</strong>
                            TS. Nguyễn Mạnh Ngọc Bảo
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4"/>
                        </svg>
                        <div>
                            <strong>Đơn vị</strong>
                            Công ty TNHH MTV An Bảo Đặc khu Phú Quốc<br>
                            Khoa Khoa học Ứng dụng và Công nghệ, Trường Đại học Nguyễn Tất Thành Việt Nam
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/>
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/>
                        </svg>
                        <div>
                            <strong>Địa chỉ cơ quan</strong>
                            Tổ 1, khu phố Xóm Mới, Đặc khu Phú Quốc, tỉnh Kiên Giang
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/>
                        </svg>
                        <div>
                            <strong>Email</strong>
                            <a href="mailto:manhbaopetrol@gmail.com">manhbaopetrol@gmail.com</a><br>
                            <a href="mailto:nmnbao@ntt.edu.vn">nmnbao@ntt.edu.vn</a>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/>
                        </svg>
                        <div>
                            <strong>Điện thoại (công việc)</strong>
                            (+84) 038 2345676
                        </div>
                    </div>
                </div>
                
                <!-- Form liên hệ -->
                <div class="contact-form">
                    <h3>Gửi thông điệp</h3>
                    <form id="contactForm" onsubmit="handleSubmit(event)">
                        <div class="form-group">
                            <label for="name">Họ và tên</label>
                            <input type="text" id="name" name="name" required placeholder="Nhập họ và tên của bạn">
                        </div>
                        
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" id="email" name="email" required placeholder="Nhập địa chỉ email">
                        </div>
                        
                        <div class="form-group">
                            <label for="subject">Tiêu đề</label>
                            <input type="text" id="subject" name="subject" required placeholder="Nhập tiêu đề">
                        </div>
                        
                        <div class="form-group">
                            <label for="message">Nội dung</label>
                            <textarea id="message" name="message" required placeholder="Nhập nội dung thông điệp..."></textarea>
                        </div>
                        
                        <button type="submit" class="btn-submit">Gửi thông điệp</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- ===== FOOTER ===== -->
    <footer>
        <div class="container">
            <p>&copy; 2025 TS. Nguyễn Mạnh Ngọc Bảo. Tất cả quyền được bảo lưu.</p>
        </div>
    </footer>

    <!-- ===== JAVASCRIPT ===== -->
    <script>
        // Toggle menu mobile
        function toggleMenu() {
            const navLinks = document.getElementById('navLinks');
            navLinks.classList.toggle('active');
        }

        // Đóng menu khi click vào link (mobile)
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                const navLinks = document.getElementById('navLinks');
                navLinks.classList.remove('active');
            });
        });

        // Xử lý form submit (chỉ demo, không có backend)
        function handleSubmit(event) {
            event.preventDefault();
            
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const subject = document.getElementById('subject').value;
            const message = document.getElementById('message').value;
            
            // Hiển thị thông báo (demo)
            alert(`Cảm ơn ${name}!\n\nThông điệp của bạn đã được ghi nhận.\nChúng tôi sẽ phản hồi qua email: ${email}`);
            
            // Reset form
            document.getElementById('contactForm').reset();
        }

        // Hiệu ứng header khi scroll
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if (window.scrollY > 50) {
                header.style.boxShadow = '0 2px 20px rgba(0,0,0,0.12)';
            } else {
                header.style.boxShadow = '0 2px 10px rgba(0,0,0,0.08)';
            }
        });
    </script>

</body>
</html>
