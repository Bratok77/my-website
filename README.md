<!DOCTYPE html>
<html lang="tk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Biznesiň Sahypasy</title>
    <style>
        /* CSS Stilleri */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #f9f9f9;
            line-height: 1.6;
        }
        header {
            background: linear-gradient(to right, #2c3e50, #3498db);
            color: white;
            text-align: center;
            padding: 2em;
        }
        nav {
            background-color: #2c3e50;
            padding: 1em;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 1.5em;
            font-weight: bold;
        }
        nav a:hover {
            color: #3498db;
            border-bottom: 2px solid #3498db;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        .hero {
            text-align: center;
            margin-bottom: 2em;
        }
        .hero img {
            width: 100%;
            max-height: 400px;
            object-fit: cover;
            border-radius: 10px;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
            margin: 2em 0;
        }
        .gallery img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 8px;
            transition: transform 0.3s;
        }
        .gallery img:hover {
            transform: scale(1.05);
        }
        .form-section {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            margin: 2em 0;
        }
        .form-section input, .form-section textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        .form-section button {
            background-color: #3498db;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .form-section button:hover {
            background-color: #2c3e50;
        }
        .map-section {
            margin: 2em 0;
        }
        .social-links {
            text-align: center;
            margin: 2em 0;
        }
        .social-links a {
            margin: 0 1em;
            color: #3498db;
            font-size: 1.5em;
            text-decoration: none;
        }
        .social-links a:hover {
            color: #2c3e50;
        }
        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 1em;
        }
        @media (max-width: 768px) {
            nav a {
                display: block;
                margin: 0.5em 0;
            }
            .gallery {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Başlyk -->
    <header>
        <h1>Biznesiň Ady</h1>
        <p>Professional hyzmatlar we ýokary hilli çözgütler</p>
    </header>

    <!-- Navigasiýa Paneli -->
    <nav>
        <a href="#home">Baş Sahypa</a>
        <a href="#about">Biz Barada</a>
        <a href="#services">Hyzmatlar</a>
        <a href="#gallery">Galereýa</a>
        <a href="#contact">Habarlaşmak</a>
    </nav>

    <!-- Esasy Bölüm -->
    <div class="container">
        <!-- Hero Bölümi -->
        <div class="hero" id="home">
            <img src="https://via.placeholder.com/1200x400" alt="Biznes Banner">
            <h2>Hoş Geldiňiz!</h2>
            <p>Biz siziň üçin iň gowy hyzmatlary hödürleýäris.</p>
        </div>

        <!-- Biz Barada -->
        <section id="about">
            <h2>Biz Barada</h2>
            <p>Biz 10 ýyldan gowrak tejribesi bolan, müşderilere ýokary hilli hyzmatlar hödürleýän kompaniýa. Maksadymyz, siziň üstünligiňiz!</p>
        </section>

        <!-- Hyzmatlar -->
        <section id="services">
            <h2>Hyzmatlarymyz</h2>
            <ul>
                <li>Web Dizaýn we Ösüş</li>
                <li>Marketing we SEO</li>
                <li>Konsultasiýa Hyzmatlary</li>
                <li>Mobil Programmalar</li>
            </ul>
        </section>

        <!-- Galereýa -->
        <section id="gallery">
            <h2>Galereýa</h2>
            <div class="gallery">
                <img src="https://via.placeholder.com/300" alt="Proýekt 1">
                <img src="https://via.placeholder.com/300" alt="Proýekt 2">
                <img src="https://via.placeholder.com/300" alt="Proýekt 3">
                <img src="https://via.placeholder.com/300" alt="Proýekt 4">
            </div>
        </section>

        <!-- Habarlaşma Formasy -->
        <section id="contact" class="form-section">
            <h2>Biz bilen Habarlaşyň</h2>
            <form action="/submit" method="post" id="contact-form">
                <label for="name">Adyňyz:</label>
                <input type="text" id="name" name="name" placeholder="Adyňyzy ýazyň" required>
                <label for="email">E-poçta:</label>
                <input type="email" id="email" name="email" placeholder="E-poçtaňyzy ýazyň" required>
                <label for="message">Hatyňyz:</label>
                <textarea id="message" name="message" rows="5" placeholder="Hatyňyzy ýazyň" required></textarea>
                <button type="submit">Ugrat</button>
            </form>
        </section>

        <!-- Ýerleşýän Ýeriň Kartasy -->
        <section class="map-section">
            <h2>Ýerleşýän Ýerimiz</h2>
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3153.086!2d-122.4194155!3d37.7749295!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x80858147439b7747%3A0x7945b3a8e876d6e7!2sSan%20Francisco%2C%20CA%2C%20USA!5e0!3m2!1sen!2s!4v1698765432100!5m2!1sen!2s" width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
        </section>

        <!-- Sosial Media Linkleri -->
        <div class="social-links">
            <a href="https://facebook.com" target="_blank">Facebook</a>
            <a href="https://twitter.com" target="_blank">Twitter</a>
            <a href="https://instagram.com" target="_blank">Instagram</a>
            <a href="https://linkedin.com" target="_blank">LinkedIn</a>
        </div>
    </div>

    <!-- Aşakky Bölüm -->
    <footer>
        <p>&copy; 2025 Biznesiň Ady. Ähli hukuklar goragly.</p>
    </footer>

    <!-- JavaScript -->
    <script>
        // Formanyň ugradylmagyny dolandyrmak
        document.getElementById('contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Hat ugradyldy! Tezlik bilen size jogap bereris.');
            this.reset();
        });

        // Navigasiýa paneliniň ýapylmagyny dolandyrmak (mobil üçin)
        window.addEventListener('scroll', function() {
            const nav = document.querySelector('nav');
            if (window.scrollY > 50) {
                nav.style.backgroundColor = '#1a252f';
            } else {
                nav.style.backgroundColor = '#2c3e50';
            }
        });
    </script>
</body>
</html>
