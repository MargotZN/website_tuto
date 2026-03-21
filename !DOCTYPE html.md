<!DOCTYPE html>  
<html lang="fr">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>Margot Zongo - Coach Sportive</title>  
  
<!-- Google Fonts -->  
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Barlow:wght@300;400;600&display=swap" rel="stylesheet">  
  
<style>  
:root {  
    --black: #080808;  
    --red: #CC0000;  
    --white: #ffffff;  
}  
  
* {  
    margin: 0;  
    padding: 0;  
    box-sizing: border-box;  
    cursor: none;  
}  
  
body {  
    font-family: 'Barlow', sans-serif;  
    background: var(--black);  
    color: var(--white);  
    overflow-x: hidden;  
}  
  
/* Cursor */  
.cursor {  
    width: 12px;  
    height: 12px;  
    background: var(--red);  
    position: fixed;  
    border-radius: 50%;  
    pointer-events: none;  
    z-index: 9999;  
    box-shadow: 0 0 15px var(--red), 0 0 30px var(--red);  
}  
  
/* Navbar */  
nav {  
    position: fixed;  
    width: 100%;  
    padding: 20px 60px;  
    display: flex;  
    justify-content: space-between;  
    z-index: 1000;  
    backdrop-filter: blur(10px);  
}  
  
.logo {  
    font-family: 'Bebas Neue', sans-serif;  
    font-size: 28px;  
    letter-spacing: 2px;  
}  
  
nav a {  
    color: var(--white);  
    text-decoration: none;  
    margin-left: 30px;  
    transition: 0.3s;  
}  
  
nav a:hover {  
    color: var(--red);  
}  
  
/* Hero */  
.hero {  
    height: 100vh;  
    display: flex;  
    align-items: center;  
    padding: 0 10%;  
    position: relative;  
}  
  
.hero-content h1 {  
    font-family: 'Bebas Neue', sans-serif;  
    font-size: 90px;  
    letter-spacing: 3px;  
}  
  
.hero-content h2 {  
    font-size: 22px;  
    margin: 20px 0;  
    color: #ccc;  
}  
  
.cta {  
    display: inline-block;  
    padding: 15px 40px;  
    border: 2px solid var(--red);  
    color: var(--white);  
    text-decoration: none;  
    margin-top: 20px;  
    transition: 0.3s;  
    box-shadow: 0 0 10px var(--red);  
}  
  
.cta:hover {  
    background: var(--red);  
    box-shadow: 0 0 25px var(--red);  
}  
  
/* Sections */  
section {  
    padding: 100px 10%;  
}  
  
/* About */  
.about p {  
    max-width: 700px;  
    line-height: 1.6;  
    color: #aaa;  
}  
  
/* Cards */  
.cards {  
    display: grid;  
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));  
    gap: 30px;  
}  
  
.card {  
    padding: 30px;  
    border: 1px solid #222;  
    transition: 0.4s;  
    position: relative;  
}  
  
.card:hover {  
    transform: translateY(-10px);  
    border-color: var(--red);  
    box-shadow: 0 0 20px rgba(204,0,0,0.5);  
}  
  
.card h3 {  
    margin-bottom: 10px;  
    font-family: 'Bebas Neue';  
}  
  
/* Timeline */  
.timeline {  
    border-left: 2px solid var(--red);  
    padding-left: 20px;  
}  
  
.timeline-item {  
    margin-bottom: 30px;  
}  
  
/* Contact */  
form {  
    max-width: 500px;  
}  
  
input, textarea {  
    width: 100%;  
    padding: 12px;  
    margin-bottom: 15px;  
    background: #111;  
    border: 1px solid #333;  
    color: white;  
}  
  
button {  
    padding: 12px 30px;  
    background: var(--red);  
    border: none;  
    color: white;  
    cursor: none;  
    box-shadow: 0 0 15px var(--red);  
}  
  
/* Animations */  
.fade {  
    opacity: 0;  
    transform: translateY(40px);  
    transition: 1s;  
}  
  
.fade.visible {  
    opacity: 1;  
    transform: translateY(0);  
}  
  
/* Background texture */  
body::before {  
    content: "";  
    position: fixed;  
    width: 100%;  
    height: 100%;  
    background: radial-gradient(circle at center, transparent 60%, black 100%);  
    opacity: 0.2;  
    z-index: -1;  
}  
</style>  
</head>  
  
<body>  
  
<div class="cursor"></div>  
  
<nav>  
    <div class="logo">MZ</div>  
    <div>  
        <a href="#about">À propos</a>  
        <a href="#specialites">Spécialités</a>  
        <a href="#parcours">Parcours</a>  
        <a href="#contact">Contact</a>  
    </div>  
</nav>  
  
<section class="hero">  
    <div class="hero-content">  
        <h1>Margot Zongo</h1>  
        <h2>Transforme ton corps. Transforme ta vie.</h2>  
        <a href="#contact" class="cta">Me contacter</a>  
    </div>  
</section>  
  
<section id="about" class="about fade">  
    <h2>À propos</h2>  
    <p>  
        Coach sportive basée à Lyon, spécialisée en recomposition corporelle, prise de muscle,  
        perte de poids et reprise du sport.   
        Actuellement en formation BPJEPS AF à l’IPMS Lyon (rentrée 2026),  
        j’accompagne chaque personne vers une transformation durable et adaptée.  
    </p>  
</section>  
  
<section id="specialites" class="fade">  
    <h2>Mes spécialités</h2>  
    <div class="cards">  
        <div class="card">  
            <h3>Recomposition</h3>  
            <p>Transformation physique globale : perte de gras + gain musculaire.</p>  
        </div>  
        <div class="card">  
            <h3>Prise de muscle</h3>  
            <p>Programmes ciblés pour construire un physique solide et esthétique.</p>  
        </div>  
        <div class="card">  
            <h3>Perte de poids</h3>  
            <p>Stratégies durables sans frustration ni régimes extrêmes.</p>  
        </div>  
        <div class="card">  
            <h3>Reprise du sport</h3>  
            <p>Accompagnement progressif pour reprendre confiance et forme.</p>  
        </div>  
    </div>  
</section>  
  
<section id="parcours" class="fade">  
    <h2>Mon parcours</h2>  
    <div class="timeline">  
        <div class="timeline-item">  
            <h4>2026</h4>  
            <p>Entrée en formation BPJEPS AF - IPMS Lyon</p>  
        </div>  
        <div class="timeline-item">  
            <h4>Aujourd’hui</h4>  
            <p>Coaching personnalisé et accompagnement transformation physique</p>  
        </div>  
    </div>  
</section>  
  
<section id="contact" class="fade">  
    <h2>Contact</h2>  
    <form>  
        <input type="text" placeholder="Nom">  
        <input type="email" placeholder="Email">  
        <textarea placeholder="Message"></textarea>  
        <button type="submit">Envoyer</button>  
    </form>  
</section>  
  
<script>  
// Cursor  
const cursor = document.querySelector('.cursor');  
document.addEventListener('mousemove', e => {  
    cursor.style.top = e.clientY + 'px';  
    cursor.style.left = e.clientX + 'px';  
});  
  
// Fade animation  
const faders = document.querySelectorAll('.fade');  
window.addEventListener('scroll', () => {  
    faders.forEach(el => {  
        const rect = el.getBoundingClientRect();  
        if(rect.top < window.innerHeight - 100){  
            el.classList.add('visible');  
        }  
    });  
});  
  
// Parallax  
window.addEventListener('scroll', () => {  
    document.querySelector('.hero').style.backgroundPositionY = window.scrollY * 0.5 + 'px';  
});  
</script>  
  
</body>  
</html>  
