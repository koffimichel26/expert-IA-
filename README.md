# expert-IA-
Logiciel de solution pour entreprises 

<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Michel IA | AI Architect</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600;800&display=swap" rel="stylesheet">

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Poppins', sans-serif;
    background: #0a0f1c;
    color: white;
    scroll-behavior: smooth;
}

/* NAVIGATION */
nav {
    position: fixed;
    width: 100%;
    padding: 15px 50px;
    background: rgba(0,0,0,0.8);
    display: flex;
    justify-content: space-between;
    z-index: 1000;
}

nav a {
    color: white;
    text-decoration: none;
    margin-left: 20px;
    font-weight: 600;
}

nav a:hover {
    color: #00f2ff;
}

/* HERO */
.hero {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #000428, #004e92);
    text-align: center;
    padding: 20px;
}

.hero h1 {
    font-size: 60px;
    animation: fadeIn 2s ease;
}

.hero span {
    color: #00f2ff;
}

.hero p {
    margin-top: 20px;
    font-size: 20px;
    opacity: 0.8;
}

.btn {
    margin-top: 30px;
    padding: 15px 35px;
    border-radius: 30px;
    background: #00f2ff;
    color: black;
    text-decoration: none;
    font-weight: bold;
    transition: 0.3s;
}

.btn:hover {
    background: white;
}

/* SECTION */
section {
    padding: 100px 20px;
    max-width: 1200px;
    margin: auto;
}

h2 {
    text-align: center;
    margin-bottom: 50px;
    color: #00f2ff;
}

.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
}

.card {
    background: #111827;
    padding: 30px;
    border-radius: 15px;
    transition: 0.4s;
}

.card:hover {
    transform: translateY(-10px);
    box-shadow: 0 15px 30px rgba(0,242,255,0.3);
}

/* COUNTER */
.counter {
    text-align: center;
    font-size: 50px;
    font-weight: 800;
    color: #00f2ff;
}

/* FOOTER */
footer {
    text-align: center;
    padding: 30px;
    background: black;
}

/* ANIMATION */
@keyframes fadeIn {
    from {opacity: 0; transform: translateY(30px);}
    to {opacity: 1; transform: translateY(0);}
}

@media(max-width:768px){
    .hero h1 { font-size: 40px; }
}
</style>
</head>

<body>

<nav>
    <div><strong>Michel IA</strong></div>
    <div>
        <a href="#expertise">Expertise</a>
        <a href="#impact">Impact</a>
        <a href="#publications">Publications</a>
        <a href="#contact">Contact</a>
    </div>
</nav>

<div class="hero">
    <h1>Michel <span>AI Architect</span></h1>
    <p>Créateur de solutions intelligentes pour transformer l’Afrique par l’IA</p>
    <a href="#contact" class="btn">Collaborons</a>
</div>

<section id="expertise">
    <h2>Expertise</h2>
    <div class="grid">
        <div class="card">
            <h3>Machine Learning</h3>
            <p>Développement de modèles prédictifs avancés.</p>
        </div>
        <div class="card">
            <h3>Automatisation IA</h3>
            <p>Chatbots intelligents & systèmes automatisés.</p>
        </div>
        <div class="card">
            <h3>Data Strategy</h3>
            <p>Transformation des données en décisions stratégiques.</p>
        </div>
    </div>
</section>

<section id="impact">
    <h2>Impact</h2>
    <div class="grid">
        <div class="card">
            <div class="counter" id="projects">0</div>
            <p>Projets IA développés</p>
        </div>
        <div class="card">
            <div class="counter" id="clients">0</div>
            <p>Organisations accompagnées</p>
        </div>
        <div class="card">
            <div class="counter" id="students">0</div>
            <p>Personnes formées</p>
        </div>
    </div>
</section>

<section id="publications">
    <h2>Conférences & Publications</h2>
    <div class="grid">
        <div class="card">
            <h3>IA & Éducation en Afrique</h3>
            <p>Conférence sur l'intégration des systèmes intelligents dans les écoles.</p>
        </div>
        <div class="card">
            <h3>Automatisation Gouvernementale</h3>
            <p>Étude sur l’optimisation des services publics via l’IA.</p>
        </div>
    </div>
</section>

<section id="contact">
    <h2>Contact</h2>
    <div class="card">
        <p>Email : michel@email.com</p>
        <p>WhatsApp : +225 XX XX XX XX</p>
        <a href="#" class="btn">Me contacter</a>
    </div>
</section>

<footer>
© 2026 Michel IA | Future AI Leader
</footer>

<script>
function animateCounter(id, target) {
    let count = 0;
    let increment = target / 200;
    let interval = setInterval(() => {
        count += increment;
        if(count >= target){
            count = target;
            clearInterval(interval);
        }
        document.getElementById(id).innerText = Math.floor(count);
    }, 10);
}

window.onload = function(){
    animateCounter("projects", 25);
    animateCounter("clients", 12);
    animateCounter("students", 300);
}
</script>

</body>
</html>
