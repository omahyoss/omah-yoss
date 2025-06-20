<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>OMAHYOSS</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background: #f9f9f9; color: #222; }
    header { background: linear-gradient(to bottom, #000000, #555555); color: white; text-align: center; padding: 3em 1em; }
    header h1 { font-size: 2.5em; font-weight: bold; }
    header p { font-size: 1em; color: #ccc; margin-top: 0.5em; }

    nav { background-color: #111; padding: 1em; position: relative; }
    .menu-toggle { font-size: 1.5em; color: white; cursor: pointer; display: block; }
    .menu { display: none; flex-direction: column; position: absolute; top: 60px; left: 0; width: 100%; background-color: #222; z-index: 99; }
    .menu a { color: white; text-decoration: none; padding: 1em; border-bottom: 1px solid #444; transition: background 0.3s; }
    .menu a:hover { background-color: #555; }

    @media (min-width: 768px) {
      nav { display: flex; justify-content: space-between; align-items: center; }
      .menu-toggle { display: none; }
      .menu { display: flex; position: static; flex-direction: row; background-color: transparent; }
      .menu a { border: none; padding: 0 1em; }
    }

    .hero-image {
      width: 100%;
      height: 300px;
      background: url('https://source.unsplash.com/1600x900/?cafe,blackwhite') center/cover no-repeat;
      filter: grayscale(100%) contrast(90%);
    }

    section { padding: 2em 1em; max-width: 900px; margin: auto; }
    section h2 { font-size: 1.8em; margin-bottom: 1em; color: #111; }
    section h3 { font-size: 1.2em; margin-top: 1.5em; }
    ul { list-style: none; padding-left: 1em; }
    li { padding: 0.3em 0; }
    p { line-height: 1.6em; margin-bottom: 1em; }

    .contact p { font-weight: 500; }
  </style>
  <script>
    function toggleMenu() {
      var menu = document.getElementById('mainMenu');
      if (menu.style.display === 'flex') {
        menu.style.display = 'none';
      } else {
        menu.style.display = 'flex';
      }
    }
  </script>
</head>
<body>

<nav>
  <div class="menu-toggle" onclick="toggleMenu()">☰ Menu</div>
  <div id="mainMenu" class="menu">
    <a href="#home">Home</a>
    <a href="#produk">Produk</a>
    <a href="#informasi">Informasi</a>
    <a href="#kontak">Contact Us</a>
  </div>
</nav>

<header id="home">
  <h1>OMAHYOSS</h1>
  <p>Kedai dan Angkringan dengan suasana nyaman dan menu khas penuh cita rasa. Tempat berkumpul yang cocok untuk semua kalangan.</p>
</header>
<div class="hero-image"></div>

<section id="produk">
  <h2>Produk</h2>
  <h3>Kopi Panas :</h3>
  <ul>
    <li>Kopi Tubruk</li>
    <li>Kopi Susu Tubruk</li>
    <li>Kopi Vietnam Drip</li>
  </ul>
  <h3>Es Kopi :</h3>
  <ul>
    <li>Kopi Therecept</li>
    <li>Kopi Susu Yoss</li>
    <li>Kopi Susu Gula Aren</li>
    <li>Kopi Susu Klasik</li>
  </ul>
  <h3>Non Kopi :</h3>
  <ul>
    <li>Teh Klasik</li>
    <li>Coklat</li>
    <li>Teh Lemon</li>
    <li>Teh Leci</li>
    <li>Milo Susu</li>
    <li>Mangga Yakult</li>
    <li>Melon Yakult</li>
    <li>Matcha</li>
  </ul>
</section>

<section id="informasi">
  <h2>Informasi</h2>
  <p>OmahYoss adalah kedai dan angkringan yang terletak di Jl. Yos Sudarso No.84a Sidoarjo. Kami menghadirkan cita rasa khas dalam setiap gelas dan suasana hangat untuk setiap kunjungan. Dibuka setiap hari mulai pukul 16.00 hingga tengah malam. Tersedia layanan dine-in, take-away, dan reservasi acara komunitas.</p>
</section>

<section id="kontak" class="contact">
  <h2>Contact Us</h2>
  <p>Email: omahyoss@kedai.id</p>
  <p>WhatsApp: +62 812-3456-7890</p>
  <p>Instagram: @omahyoss</p>
</section>

</body>
</html>
