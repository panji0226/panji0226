<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Website Pribadi Saya</title>
    <style>
        /* Umum */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f4f8;
            color: #333;
            line-height: 1.6;
        }

        h1, h2 {
            font-family: 'Helvetica Neue', sans-serif;
            font-weight: 700;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        /* Header */
        header {
            background-color: #6c63ff;
            color: white;
            text-align: center;
            padding: 2em 0;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        header h1 {
            font-size: 3em;
        }

        header p {
            font-size: 1.2em;
            margin-top: 0.5em;
        }

        /* Navigasi */
        nav {
            display: flex;
            justify-content: center;
            background-color: #f8f8f8;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        nav a {
            color: #333;
            padding: 18px 30px;
            text-align: center;
            font-size: 1.1em;
            transition: background-color 0.3s, color 0.3s;
        }

        nav a:hover {
            background-color: #6c63ff;
            color: white;
        }

        /* Profil */
        .profile {
            text-align: center;
            margin: 3em 0;
            background: linear-gradient(135deg, #6c63ff 0%, #7e55ff 100%);
            padding: 2em;
            border-radius: 10px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.05);
        }

        .profile img {
            border-radius: 50%;
            width: 150px;
            height: 150px;
            object-fit: cover;
            border: 5px solid white;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
        }

        .profile h2 {
            margin-top: 1em;
            color: white;
            font-size: 2em;
        }

        .profile p {
            color: #f9f9f9;
            font-size: 1.2em;
            max-width: 80%;
            margin: 1em auto;
        }

        /* Galeri Foto */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin: 3em 0;
        }

        .gallery img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .gallery img:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 45px rgba(0, 0, 0, 0.2);
        }

        /* Kontak */
        .contact {
            background-color: #f7f7f7;
            padding: 2em;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            margin-bottom: 3em;
        }

        .contact h2 {
            font-size: 2.5em;
            color: #333;
            text-align: center;
            margin-bottom: 1em;
        }

        .contact ul {
            list-style: none;
            padding: 0;
            text-align: center;
        }

        .contact ul li {
            font-size: 1.2em;
            margin: 10px 0;
        }

        .social-links {
            text-align: center;
            margin-top: 1.5em;
        }

        .social-links a {
            margin: 0 15px;
            color: #333;
            font-size: 2em;
            transition: color 0.3s;
        }

        .social-links a:hover {
            color: #6c63ff;
        }

        /* Footer */
        footer {
            background-color: #000080;
            color: white;
            padding: 1.5em 0;
            text-align: center;
        }

    </style>
</head>
<body>

    <header>
        <h1>Website Pribadi Gue</h1>
        <p>Yokoso orang orang sdm Tinggi</p>
    </header>

    <nav>
        <a href="#about">Tentang Gue</a>
        <a href="#gallery">Galeri random</a>
        <a href="#contact">Kontak</a>
    </nav>

    <section id="about">
        <div class="profile">
            <img src="data:image/jpeg;base64,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" alt="Foto Profil">
            <h2>Panji syahputra</h2>
            <p>Seorang pelajar yang baru belajar membuat web walaupun masih html dan css jan di hujat bang wkwkwk,enjoy kasih rating web buatan gua wkwkwk,sebenernya ini bagian tentang diri gua cuma bingung isi apa (seterah dah gede)</p>
        </div>
    </section>

    <section id="projects">
        <h2>Lagu favorit</h2>
        <ul>
            <li>salvastore: <a href="#">lana del rey</a></li>
            <li>we can't be your friend: <a href="#">ariana grande</a></li>
            <li>A little of piece heaven: <a href="#">avenged sevenfold</a></li>
        </ul>
    </section>

    <section id="gallery">
        <h2>Galeri Foto</h2>
        <div class="gallery">
            <img src="https://i.pinimg.com/236x/44/a8/8b/44a88b1b16436ae421a9c50843b36f64.jpg" alt="Foto 1">
            <img src="https://i.pinimg.com/736x/9a/1c/77/9a1c779e8aa9296f987ab0d25c624f96.jpg" alt="Foto 2">
            <img src="https://i.redd.it/sung-jin-woo-vs-itarim-v0-aaxs7rkc0nod1.jpg?width=633&format=pjpg&auto=webp&s=5ecffb4ab07a5be31998160cba8cff8a64376cf3" alt="Foto 3">
            <img src="https://beta.tvarenasport.com/data/images/2023-03-24/2352_tan2023-03-2405183162-3_f.jpg" alt="Foto 4">
            <img src="https://i.scdn.co/image/ab67616d0000b273a6a1e52fb03a5f002108d914" alt="Foto 5">
            <img src="https://static.wikia.nocookie.net/vsbattles/images/1/12/AwakenedAkutoVol8DKD.png/revision/latest?cb=20221002070815" alt="Foto 6">
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Kontak gue</h2>
        <ul>
            <li>Email: <a href="matkiong2008@gmail.com">matkiong2008@gmail.com</a></li>
            <li>Telepon: +62 855 9127 0832</li>
        </ul>
        <div class="social-links">
            <a href="https://www.instagram.com/kennethcelloo?igsh=a2d6OGsxZjYyMWFy" target="_blank">Instagram</a>
            <a href="https://www.tiktok.com/@kenn.2602?_t=ZS-8u7sOVashuS&_r=1" target="_blank">TikTok</a>
            <a href="https://www.facebook.com/panji.syahputra.7311" target="_blank">Facebook</a>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Website Pribadi gua,hakcip di lindungi gua sendiri.</p>
    </footer>

</body>
</html>
