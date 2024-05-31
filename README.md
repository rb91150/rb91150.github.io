<!DOCTYPE html>

<html lang="fr">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Portfolio BTS SIO SLAM</title>

    <style>

        body {

            font-family: Arial, sans-serif;

            background-color: #f4f4f4;

            margin: 0;

            padding: 0;

            transition: background-color 0.3s, color 0.3s;

        }

        header {

            background-color: #333;

            color: #fff;

            padding: 20px;

            text-align: center;

            position: relative;

        }

        header h1 {

            margin: 0;

        }

        .theme-toggle {

            position: absolute;

            top: 20px;

            right: 20px;

            background: none;

            border: none;

            cursor: pointer;

        }

        nav {

            background-color: #444;

            overflow: hidden;

        }

        nav a {

            float: left;

            display: block;

            color: #fff;

            text-align: center;

            padding: 14px 20px;

            text-decoration: none;

        }

        nav a:hover {

            background-color: #ddd;

            color: black;

        }

        .container {

            padding: 20px;

        }

        .section {

            display: none;

        }

        .section.active {

            display: block;

        }

        .dark-mode {

            background-color: #1a1a1a;

            color: #00ff00;

        }

        .dark-mode header {

            background-color: #000;

            border-bottom: 2px dashed #00ff00;

        }

        .dark-mode nav {

            background-color: #000;

            border-bottom: 2px dashed #00ff00;

        }

        .dark-mode nav a {

            color: #00ff00;

        }

        .dark-mode nav a:hover {

            background-color: #00ff00;

            color: #000;

        }

        .logo {

            display: block;

            margin: 20px auto;

            width: 150px;

            height: auto;

        }

        .animated-screen {

            width: 100%;

            height: 300px;

            background: url('animated-screen.png') no-repeat center center;

            background-size: contain;

            animation: screenAnimation 3s infinite alternate;

        }

        @keyframes screenAnimation {

            0% {

                transform: scale(1);

            }

            100% {

                transform: scale(1.1);

            }

        }

        .theme-icon {

            width: 40px;

            height: 40px;

        }

    </style>

    <script>

        function showSection(sectionId) {

            var sections = document.getElementsByClassName('section');

            for (var i = 0; i < sections.length; i++) {

                sections[i].classList.remove('active');

            }

            document.getElementById(sectionId).classList.add('active');

        }



        function toggleTheme() {

            var body = document.body;

            body.classList.toggle('dark-mode');

            var themeIcon = document.getElementById('theme-icon');

            if (body.classList.contains('dark-mode')) {

                themeIcon.src = 'icons/sun-icon.png'; // Change to your light mode icon

            } else {

                themeIcon.src = 'icons/moon-icon.png'; // Change to your dark mode icon

            }

        }

    </script>

</head>

<body>



<header>

    <h1>Portfolio BTS SIO</h1>

    <button class="theme-toggle" onclick="toggleTheme()">

        <img id="theme-icon" src="icons/moon-icon.png" alt="Toggle Theme" class="theme-icon">

    </button>

</header>



<nav>

    <a href="#" onclick="showSection('accueil')">Accueil</a>

    <a href="#" onclick="showSection('apropos')">À propos</a>

    <a href="#" onclick="showSection('veille')">Veille technologique</a>

    <a href="#" onclick="showSection('notes')">Notes de synthèse</a>

    <a href="#" onclick="showSection('contact')">Contact</a>

</nav>



<div class="container">

    <img src="icons/animated-screen.png" alt="Logo" class="logo">

    <div id="accueil" class="section active">

        <h2>Accueil</h2>

        <p>Bienvenue sur le portfolio de Raphaël Boee Bosale, étudiant en première année de BTS Services Informatiques aux Organisations (SIO) spécialité SLAM.</p>

        <div class="animated-screen"></div>

    </div>

    <div id="apropos" class="section">

        <h2>À propos</h2>

        <p>Je suis un étudiant proactif, rigoureux et collaboratif à la recherche de nouvelles opportunités pour mettre à profit mes compétences en informatique. Actuellement en première année de BTS SIO à Étampes et en stage, je suis passionné par le développement web, la gestion de projets informatiques et la cybersécurité.</p>

        <p>Le BTS Services Informatiques aux Organisations (SIO) est une formation qui prépare aux métiers de l'informatique en entreprise. Il propose deux spécialités :</p>

        <ul>

            <li><strong>SISR (Solutions d’Infrastructure, Systèmes et Réseaux)</strong> : axée sur la gestion et la maintenance des infrastructures réseaux et systèmes.</li>

            <li><strong>SLAM (Solutions Logicielles et Applications Métiers)</strong> : orientée vers le développement de logiciels et d’applications pour répondre aux besoins spécifiques des entreprises.</li>

        </ul>

        <p>En choisissant la spécialité SLAM, j'ai acquis des compétences en programmation, en développement d'applications et en gestion de bases de données, me permettant de concevoir des solutions logicielles adaptées aux besoins des utilisateurs.</p>

    </div>

    <div id="veille" class="section">

        <h2>Veille technologique</h2>

        <p>Voici mes travaux de veille technologique.</p>

    </div>

    <div id="notes" class="section">

        <h2>Notes de synthèse</h2>

        <p>Vous trouverez ici les notes de synthèse rédigées dans le cadre de mon stage.</p>

        <ul>

            <li><a href="https://docs.google.com/document/d/1smSfE85Gs767iWNDNRyt_AsRA2Tn9lO6CrkGj_OgJ8M/edit?usp=sharing" target="_blank">Note de synthèse - Stage</a></li>

        </ul>

    </div>

    <div id="contact" class="section">

        <h2>Contact</h2>

        <p>Vous pouvez me contacter à l'adresse suivante :</p>

        <ul>

            <li>Téléphone : 06.24.99.94.30</li>

            <li>Email : raphael.boeebosale.pro@gmail.com</li>

        </ul>

    </div>

</div>



</body>

</html>
 
