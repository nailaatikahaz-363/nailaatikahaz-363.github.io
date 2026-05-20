<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Naila Atikah Adya Zahra</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@600;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* --- JANGAN LUPA RESET --- */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

/* --- BUAT CONTAINER FLEKSIBEL --- */
.container {
    max-width: 1100px; /* Batas lebar maksimal di laptop */
    width: 90%;       /* Saat layar kecil, ambil 90% lebar layar */
    margin: 0 auto;   /* Tengahkan otomatis */
    padding: 0 15px;
}

/* --- BUAT GAMBAR RESPONSIF --- */
img {
    max-width: 100%;  /* Gambar tidak akan pernah lebih lebar dari container */
    height: auto;     /* Tinggi mengikuti proporsi aslinya */
}

/* --- LAYOUT FLEKSIBEL (Gunakan Flexbox) --- */
.flex-container {
    display: flex;
    flex-wrap: wrap; /* Bungkus ke bawah kalau layar sempit */
    gap: 20px;
}

/* --- KOLOM OTOMATIS (CSS Grid) --- */
.grid-konten {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

/* --- NAVIGASI RESPONSIF --- */
/* Jika layar maks 768px (HP/Tablet), ubah menu jadi vertikal */
@media (max-width: 768px) {
    nav {
        flex-direction: column;
        text-align: center;
    }
    
    nav ul {
        flex-direction: column;
        padding: 0;
        list-style: none;
    }
    
    nav ul li {
        margin: 10px 0;
    }
}
        /* --- PALET WARNA PASTEL --- */
        :root {
            /* Biru Pastel */
            --blue-pastel: #BDE0FE;
            --blue-medium: #AED6F1;
            --blue-dark: #5DADE2; /* Biru lebih kuat untuk teks */
            --blue-navy: #2874A6; /* Untuk kontras teks */

            /* Kuning Pastel */
            --yellow-pastel: #FEF9E7;
            --yellow-bright: #F7DC6F;
            --yellow-gold: #F4D03F;

            /* Netral */
            --white: #FFFFFF;
            --off-white: #FDFBF7;
            --text-dark: #2C3E50;
            
            --transisi: all 0.3s ease;
        }
    /* --- PRESTASI SECTION --- */
    #achievements {
        background-color: var(--yellow-pastel);
        padding: 5rem 10%;
    }

    .achievement-container {
        max-width: 1000px;
        margin: 0 auto;
    }

    .section-title {
        font-family: 'Montserrat', sans-serif;
        font-size: 2.5rem;
        color: var(--blue-navy);
        text-align: center;
        margin-bottom: 3rem;
    }

    /* Tampilan Tabel/Kotak */
    .prestige-table {
        width: 100%;
        border-collapse: separate;
        border-spacing: 0 15px; /* Jarak antar kotak */
    }

    .prestige-table th {
        text-align: left;
        padding: 10px 20px;
        color: var(--blue-navy);
        font-size: 0.9rem;
        text-transform: uppercase;
        letter-spacing: 1px;
    }

    .prestige-row {
        background: var(--white);
        box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        transition: all 0.3s ease;
        border-radius: 15px;
    }
    
    .prestige-row:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        background: var(--blue-pastel);
    }

    .prestige-table td {
        padding: 20px;
        vertical-align: middle;
        color: var(--text-dark);
    }

    /* Kolom Pertama: Tahun */
    .col-year {
        font-weight: 700;
        color: var(--blue-navy);
        background: var(--blue-pastel);
        border-radius: 15px 0 0 15px;
        width: 100px;
        text-align: center;
    }

    /* Kolom Kedua: Nama Prestasi */
    .col-title {
        font-weight: 600;
        font-size: 1.1rem;
        color: var(--blue-navy);
    }

    /* Kolom Ketiga: Penyelenggara */
    .col-event {
        font-size: 0.95rem;
        color: #666;
    }

    /* Kolom Keempat: Peringkat/Gelar */
    .col-rank {
        text-align: center;
        font-weight: 700;
        color: var(--yellow-gold);
        text-shadow: 1px 1px 0 var(--blue-navy);
        font-size: 1.2rem;
    }

    /* Responsif HP */
    @media (max-width: 768px) {
        .prestige-table thead { display: none; }
        .prestige-table, .prestige-table tbody, .prestige-table tr, .prestige-table td {
            display: block;
            width: 100%;
        }
        .prestige-table tr {
            margin-bottom: 20px;
            border: 1px solid #eee;
            border-radius: 15px;
            overflow: hidden;
        }
        .prestige-table td {
            text-align: right;
            padding: 10px 20px;
            border-bottom: 1px solid #f9f9f9;
        }
        .prestige-table td::before {
            content: attr(data-label);
            float: left;
            font-weight: 700;
            color: var(--blue-navy);
        }
        .col-year { border-radius: 15px 15px 0 0; width: 100%; display: block; padding: 10px; }
    }
        /* --- RESET & BASE --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--off-white);
            color: var(--text-dark);
            line-height: 1.7;
            overflow-x: hidden;
        }

        a { text-decoration: none; color: inherit; }
        ul { list-style: none; }
        img { max-width: 100%; display: block; }

        /* --- NAVIGASI --- */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(10px);
            z-index: 1000;
            box-shadow: 0 2px 15px rgba(0,0,0,0.03);
        }

        .logo {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 1.5rem;
            color: var(--blue-navy);
        }

        .logo span { color: var(--yellow-gold); }

        .nav-links {
            display: flex;
            gap: 2rem;
        }

        .nav-links a {
            font-size: 0.9rem;
            font-weight: 600;
            color: var(--blue-navy);
            position: relative;
            transition: var(--transisi);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -3px;
            left: 0;
            background: var(--yellow-gold);
            transition: var(--transisi);
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        /* --- HERO SECTION --- */
        header {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 20px;
            /* Latar Belakang Gradien Pastel Biru-Kuning */
            background: linear-gradient(135deg, var(--blue-pastel) 0%, var(--yellow-pastel) 100%);
            position: relative;
        }

        /* Bola-bola Dekorasi */
        .blob {
            position: absolute;
            border-radius: 50%;
            filter: blur(40px);
            z-index: -1;
        }
        .blob-1 {
            width: 400px; height: 400px;
            background: rgba(255,255,255, 0.5);
            top: -100px; left: -100px;
        }
        .blob-2 {
            width: 300px; height: 300px;
            background: var(--blue-medium);
            bottom: 50px; right: -50px;
            opacity: 0.5;
        }

        .hero-title {
            font-family: 'Montserrat', sans-serif;
            font-size: 4rem;
            color: var(--blue-navy);
            margin-bottom: 0.5rem;
            animation: fadeUp 1s ease;
        }

        .hero-subtitle {
            font-size: 1.3rem;
            color: var(--blue-navy);
            opacity: 0.8;
            margin-bottom: 2rem;
            animation: fadeUp 1s ease 0.2s backwards;
        }

        .btn-hero {
            padding: 12px 35px;
            background-color: var(--blue-navy);
            color: var(--white);
            border-radius: 50px;
            font-weight: 600;
            animation: fadeUp 1s ease 0.4s backwards;
            transition: var(--transisi);
            box-shadow: 0 5px 15px rgba(40, 116, 166, 0.3);
        }

        .btn-hero:hover {
            transform: translateY(-3px);
            background-color: var(--blue-dark);
        }

        .scroll-hint {
            position: absolute;
            bottom: 30px;
            font-size: 0.9rem;
            color: var(--blue-navy);
            animation: bounce 2s infinite;
        }

        /* --- SECTION STYLES --- */
        section {
            padding: 5rem 10%;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
        }

        .section-title {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.5rem;
            color: var(--blue-navy);
            text-align: center;
            margin-bottom: 3rem;
        }

        .section-line {
            width: 60px;
            height: 5px;
            background: var(--yellow-gold);
            margin: -2rem auto 3rem auto;
            border-radius: 10px;
        }

        /* --- ABOUT --- */
        #about {
            background-color: var(--white);
        }

        .about-layout {
            display: grid;
            grid-template-columns: 1fr 1.2fr;
            gap: 4rem;
            align-items: center;
        }

        .photo-box {
            width: 100%;
            aspect-ratio: 3/4;
            background: var(--blue-pastel);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 25px 25px 0 var(--yellow-bright);
            position: relative;
        }
        
        .photo-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .about-text h3 {
            font-size: 1.8rem;
            color: var(--blue-navy);
            margin-bottom: 1.2rem;
        }

        .about-text p {
            color: #555;
            margin-bottom: 1.5rem;
            text-align: justify;
        }

        /* --- KEAHLIAN / KETERAMPILAN --- */
        #skills {
            background: linear-gradient(to bottom, var(--white), var(--yellow-pastel));
        }

        .skill-wrapper {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
        }

        .skill-chip {
            background: var(--white);
            padding: 12px 25px;
            border-radius: 30px;
            font-weight: 600;
            color: var(--blue-navy);
            border: 2px solid var(--blue-medium);
            transition: var(--transisi);
        }

        .skill-chip:hover {
            background: var(--blue-pastel);
            border-color: var(--blue-navy);
            transform: translateY(-5px);
            cursor: pointer;
        }

        /* --- PENGALAMAN / TIMELINE --- */
        #experience {
            background-color: var(--white);
        }

        .exp-list {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .exp-card {
            background: var(--blue-pastel);
            padding: 1.5rem;
            border-radius: 15px;
            border-left: 6px solid var(--yellow-gold);
            transition: var(--transisi);
        }

        .exp-card:hover {
            transform: translateX(10px);
            background: var(--blue-medium);
        }

        .exp-card h3 {
            color: var(--blue-navy);
            margin-bottom: 0.5rem;
        }

        .exp-date {
            font-size: 0.85rem;
            font-weight: 700;
            color: var(--blue-dark);
            margin-bottom: 1rem;
            display: block;
        }

        /* --- PRESTASI --- */
        #achievements {
            background-color: var(--yellow-pastel);
        }

        .ach-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .ach-card {
            background: var(--white);
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: var(--transisi);
        }

        .ach-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }

        .ach-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
            color: var(--yellow-gold);
        }

        .ach-card h3 {
            color: var(--blue-navy);
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }

        .ach-card p {
            font-size: 0.9rem;
            color: #666;
        }

        /* --- FOOTER / PENUTUP --- */
        footer {
            background-color: var(--blue-navy);
            color: var(--white);
            text-align: center;
            padding: 5rem 20px;
        }

        .footer-content h2 {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .footer-content p {
            max-width: 600px;
            margin: 0 auto;
            opacity: 0.9;
        }

        .socials {
            margin-top: 2.5rem;
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        .socials a {
            width: 50px; height: 50px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 1.2rem;
            transition: var(--transisi);
        }

        .socials a:hover {
            background: var(--yellow-gold);
            color: var(--blue-navy);
            transform: rotate(360deg);
        }

        .copyright {
            margin-top: 4rem;
            font-size: 0.8rem;
            opacity: 0.5;
        }

        /* --- ANIMASI --- */
        @keyframes fadeUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(10px); }
        }

        /* RESPONSIF HP */
        @media (max-width: 768px) {
            .hero-title { font-size: 2.8rem; }
            .about-layout { grid-template-columns: 1fr; gap: 2rem; }
            .photo-box { max-width: 320px; margin: 0 auto; }
            .nav-links { display: none; }
        }
    </style>
</head>
<body>

    <!-- Nav -->
    <nav>
        <div class="logo">Naila's Profile<span>.</span></div>
        <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Talent</a></li>
            <li><a href="#experience">Class</a></li>
            <li><a href="#achievements">Achievements</a></li>
        </ul>
    </nav>

    <!-- Hero -->
    <header>
        <div class="blob blob-1"></div>
        <div class="blob blob-2"></div>
        
        <h1 class="hero-title">Halo! Aku Naila Atikah Adya Zahra</h1>
        <p class="hero-subtitle">I'm a student. A learner. A Technology & Creative Enthusiast. </p>
        <a href="#about" class="btn-hero">Lihat Profil</a>
        
        <div class="scroll-hint">↓ Scroll Down</div>
    </header>

    <!-- Tentang Saya -->
    <section id="about">
        <div class="container">
            <h2 class="section-title">About Me</h2>
            <div class="section-line"></div>

            <div class="about-layout">
                <!-- Foto -->
                <div class="photo-box">
                    <img src="https://drive.google.com/file/d/1OoEesEEvTXFXBbYZUpaLZK-vTHT-tiNB/view?usp=drivesdk" alt="Foto Profil">
                    <!-- Ganti Link Atas dengan link foto asli kamu Contoh: <img src="images/foto-saya.jpg"> -->
                </div>

                <!-- Teks -->
                <div class="about-text">
                    <h3>Perkenalan Singkat</h3>
                    <p>
                        Aku adalah siswa kelas X di SMA Negeri 2 Bandar Lampung. I love to do design, poetry, writing, and speaking. Aku juga memiliki ketertarikan besar di front-end developing.
                    </p>
                    <p>
                        Aku percaya bahwa belajar adalah proses tanpa henti. Lewat website ini, aku ingin memperkenalkan diri ku secara personal, menunjukkan prestasi dan karya-karya yang telah aku buat dengan sepenuh hati.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Bakat / Skills -->
    <section id="skills">
        <div class="container">
            <h2 class="section-title">Bakat & Minat</h2>
            <div class="section-line"></div>

            <div class="skill-wrapper">
                <div class="skill-chip">💻 Coding</div>
                <div class="skill-chip">🎨 Desain</div>
                <div class="skill-chip">🎤 Public Speaking</div>
                <div class="skill-chip">📷 Fotografi, Sinematografi</div>
                <div class="skill-chip">📝 Menulis</div>
            </div>
        </div>
    </section>

    <!-- Pengalaman / Kelas -->
    <section id="experience">
        <div class="container">
            <h2 class="section-title">Jalur Pendidikan</h2>
            <div class="section-line"></div>

            <div class="exp-list">
                <div class="exp-card">
                    <h3>SMA Negeri 2 Bandar Lampung</h3>
                    <span class="exp-date">2025 - Sekarang</span>
                    <p>Mengambil Jurusan IPA. Aktif di organisasi dalam sekolah (OSIS) sebagai anggota Seksi Bidang 3: Pembinaan Kepribadian Unggul, Wawasan Kebangsaan, dan Bela Negara. Aktif dalam organisasi luar sekolah yaitu Forum Pelajar Lampung. Mengikuti ekstrakurikuler BARA (Bahasa dan Sastra) spesifiknya di bidang Debat Bahasa Indonesia. Terpilih sebagai Teenagers of Prestige (T.O.P) atau Duta Sekolah SMAN 2 Bandar Lampung.</p>
                </div>
                <div class="exp-card">
                    <h3>SMP Muhammadiyah Ahmad Dahlan Metro</h3>
                    <span class="exp-date">2022 - 2025</span>
                    <p>Berkontribusi di berbagai organisasi dalam sekolah, seperti IPM (Ikatan Pelajar Muhammadiyah) selaku anggota bidang Perkaderan saat kelas 7, dan selaku Sekretaris Umum di periode selanjutnya. Aktif di organisasi Paskibra tingkat sekolah selaku Danton Polisi Pasukan, bertugas sebagai Danton Pasukan 45 di Upacara Bendera HUT Kemerdekaan RI ke-78 2023, dan Danton Pasukan 8 di tahun berikutnya. Menjabat sebagai koordinator ekstrakurikuler Sastra. Lulus sebagai ranking 8 nilai rapor secara paralel dari 300+ murid seangkatan. Nominasi siswa berprestasi Non-Akademik dan Organisasi. </p>
                </div>
                <div class="exp-card">
                    <h3>SD Muhammadiyah Metro Pusat</h3>
                    <span class="exp-date">2016-2022</span>
                    <p>Aktif dalam ekstrakurikuler akademik maupun non-akademik, yaitu MIPA dan Sastra. Berpartisipasi dalam banyak ajang olimpiade Matematika dan IPA, dan menjuarai belasan lomba mencipta dan membaca puisi.</p>
                </div>
            </div>
        </div>
    </section>

   <!-- Section Prestasi -->
<section id="achievements">
    <div class="achievement-container">
        <h2 class="section-title">🏆 My Achievements</h2>
        
        <table class="prestige-table">
            <thead>
                <tr>
                    <th>Tahun</th>
                    <th>Prestasi</th>
                    <th>Penyelenggara</th>
                    <th>Juara</th>
                </tr>
            </thead>
            <tbody>
                <!-- Data 1 -->
                <tr class="prestige-row">
                    <td data-label="Tahun" class="col-year">2026</td>
                    <td data-label="Prestasi" class="col-title">Juara 1 Pidato B. Indonesia</td>
                    <td data-label="Penyelenggara" class="col-event">Festival Lingkungan Green Generation</td>
                    <td data-label="Peringkat" class="col-rank">🥇</td>
                </tr>

                <!-- Data 2 -->
                <tr class="prestige-row">
                    <td data-label="Tahun" class="col-year">2025</td>
                    <td data-label="Prestasi" class="col-title">Juara 3 Pidato B. Indonesia</td>
                    <td data-label="Penyelenggara" class="col-event">HMD HUMAS FISIP Universitas Lampung</td>
                    <td data-label="Peringkat" class="col-rank">🥇</td>
                </tr>

                <!-- Data 3 -->
                <tr class="prestige-row">
                    <td data-label="Tahun" class="col-year">2025</td>
                    <td data-label="Prestasi" class="col-title">Juara 1 Baca Puisi/Deklamasi</td>
                    <td data-label="Penyelenggara" class="col-event">AMUSE XV SMA S Al Kautsar Bandar Lampung</td>
                    <td data-label="Peringkat" class="col-rank">🥇</td>
                </tr>

                <!-- Data 4 -->
                <tr class="prestige-row">
                    <td data-label="Tahun" class="col-year">2024</td>
                    <td data-label="Prestasi" class="col-title">Gold Medal Sya'ir</td>
                    <td data-label="Penyelenggara" class="col-event">International Olympiad of Qur'an and Science, Jakarta</td>
                    <td data-label="Peringkat" class="col-rank">🥇</td>
                </tr>
                 <!-- Data 5 -->
                <tr class="prestige-row">
                    <td data-label="Tahun" class="col-year">2024</td>
                    <td data-label="Prestasi" class="col-title">Medali Emas Dakwah Digital</td>
                    <td data-label="Penyelenggara" class="col-event">Olympic Ahmad Dahlan VII PP Muhammadiyah, Bandung</td>
                    <td data-label="Peringkat" class="col-rank">🥇</td>
                </tr>
                 <!-- Data 6 -->
                <tr class="prestige-row">
                    <td data-label="Tahun" class="col-year">2024</td>
                    <td data-label="Prestasi" class="col-title">Medali Emas Pidato B. Indonesia</td>
                    <td data-label="Penyelenggara" class="col-event">BEGAWI FEST MAN IC Lampung Timur 2024</td>
                    <td data-label="Peringkat" class="col-rank">🥇</td>
                </tr>
                 <!-- Data 7 -->
                <tr class="prestige-row">
                    <td data-label="Tahun" class="col-year">2024</td>
                    <td data-label="Prestasi" class="col-title">Juara 1 Cipta dan Baca Puisi</td>
                    <td data-label="Penyelenggara" class="col-event">SAPHORIA 2.0 MAN 1 Bandar Lampung</td>
                    <td data-label="Peringkat" class="col-rank">🥇</td>
                </tr>
            </tbody>
        </table>
    </div>
</section>
