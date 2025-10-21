index.html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Administrasi Sistem Jaringan XII TKJ D</title>

  <style>
    /* === CSS & ANIMASI === */
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #e0f2ff, #f8fbff);
      margin: 0;
      padding: 0;
      color: #333;
      scroll-behavior: smooth;
    }

    header {
      background: linear-gradient(90deg, #0077cc, #00b4d8);
      color: white;
      text-align: center;
      padding: 25px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.2);
      animation: slideDown 1s ease-out;
    }

    nav {
      background: #f0f0f0;
      text-align: center;
      padding: 12px 0;
      position: sticky;
      top: 0;
      z-index: 10;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    nav a {
      text-decoration: none;
      color: #0077cc;
      margin: 0 15px;
      font-weight: bold;
      transition: 0.3s;
    }

    nav a:hover {
      color: #005999;
      text-shadow: 0 0 5px #a7d8ff;
    }

    section {
      padding: 40px 20px;
      text-align: center;
      animation: fadeIn 1s ease-in;
    }

    section:nth-child(even) {
      background: #f9fbff;
    }

    .content h2 {
      color: #0077cc;
      margin-bottom: 10px;
      animation: slideUp 0.8s ease-out;
    }

    .bio {
      margin-top: 15px;
      line-height: 1.8;
    }

    .foto {
      width: 160px;
      border-radius: 50%;
      border: 4px solid #0077cc;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      transition: transform 0.5s ease;
    }

    .foto:hover {
      transform: scale(1.08);
    }

    .gambar {
      width: 60%;
      max-width: 500px;
      border-radius: 10px;
      margin: 20px auto;
      display: block;
      box-shadow: 0 3px 10px rgba(0,0,0,0.2);
      transition: transform 0.5s ease, box-shadow 0.5s ease;
    }

    .gambar:hover {
      transform: scale(1.03);
      box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    }

    ul {
      text-align: left;
      display: inline-block;
      margin-top: 10px;
      line-height: 1.8;
    }

    footer {
      background: linear-gradient(90deg, #0077cc, #00b4d8);
      color: white;
      text-align: center;
      padding: 12px;
      margin-top: 30px;
      font-size: 14px;
      letter-spacing: 0.5px;
    }

    /* === ANIMASI KEYFRAMES === */
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes slideDown {
      from { transform: translateY(-50px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    @keyframes slideUp {
      from { transform: translateY(50px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    /* === RESPONSIVE === */
    @media (max-width: 600px) {
      .gambar { width: 90%; }
      .foto { width: 120px; }
      nav a { display: inline-block; margin: 5px; }
    }
  </style>
</head>

<body>
  <header>
    <h1>Administrasi Sistem Jaringan XII TKJ D</h1>
  </header>

  <nav>
    <a href="#identitas">Identitas</a>
    <a href="#controlpanel">Control Panel</a>
    <a href="#hosting">Pengantar Hosting</a>
  </nav>

  <!-- Identitas Pribadi -->
  <section id="identitas" class="content">
    <h2>Identitas Pribadi</h2>
    <img src="fotoku.jpg" alt="Foto Saya" class="foto">
    <div class="bio">
      <p><b>Nama:</b> [Muhamad Daffa]</p>
      <p><b>Alamat:</b> [KP Cipedak,srengseng sawah]</p>
      <p><b>Cita-cita:</b> [membahagiakan orang tua,masinis ]</p>
      <p><b>Hobi:</b> [mendengarkan musik]</p>
    </div>
  </section>

  <!-- Control Panel Hosting -->
  <section id="controlpanel" class="content">
    <h2>Rangkuman Materi Control Panel Hosting</h2>
    <p>
      Control Panel (cPanel) adalah antarmuka berbasis web untuk mengelola layanan hosting.
      Dengan cPanel, kita bisa mengatur domain, file, database, email, dan backup dengan mudah.
    </p>
    <img src="cpanel.png" alt="Tampilan cPanel" class="gambar">
    <ul>
      <li>File Manager — Mengatur file website.</li>
      <li>MySQL Database — Mengelola database website.</li>
      <li>Email — Membuat email dengan nama domain sendiri.</li>
      <li>Backup — Menyimpan salinan data website.</li>
    </ul>
  </section>

  <!-- Pengantar Hosting -->
  <section id="hosting" class="content">
    <h2>Pengantar Hosting</h2>
    <p>
      Hosting adalah layanan untuk menyimpan file website agar bisa diakses secara online.
      Semua file disimpan di server yang selalu aktif di internet.
    </p>
    <img src="hosting.png" alt="Ilustrasi Hosting" class="gambar">
    <ul>
      <li><b>Shared Hosting:</b> Server digunakan bersama banyak pengguna.</li>
      <li><b>VPS Hosting:</b> Server virtual dengan kontrol penuh.</li>
      <li><b>Cloud Hosting:</b> Menggunakan beberapa server agar lebih stabil.</li>
    </ul>
  </section>

  <footer>
    &copy; 2025 XII TKJ D | Website Pribadi
  </footer>
</body>
</html>
