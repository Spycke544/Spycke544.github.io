<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arkhavel Dorne — Background & Candidature</title>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700;900&family=Cinzel+Decorative:wght@400;700;900&family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500&display=swap" rel="stylesheet">
    <style>
/* ============================================================
   RESET & BASE
   ============================================================ */
*, *::before, *::after {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --bg-deep: #0a0611;
    --bg-dark: #110b1e;
    --bg-card: #160f24;
    --bg-card-hover: #1c1430;
    --purple-dark: #2d0a4e;
    --purple: #6c3fa0;
    --purple-light: #a66de2;
    --purple-glow: #b47aed;
    --gold: #d4a01e;
    --gold-light: #f0cc5b;
    --gold-pale: #f5e6a3;
    --text-primary: #e8e0f0;
    --text-secondary: #b8a8d0;
    --text-muted: #7a6a92;
    --border-subtle: rgba(108, 63, 160, 0.2);
    --border-gold: rgba(212, 160, 30, 0.3);
}

html {
    scroll-behavior: smooth;
    scrollbar-width: thin;
    scrollbar-color: var(--purple) var(--bg-deep);
}

body {
    font-family: 'Cormorant Garamond', Georgia, serif;
    background: var(--bg-deep);
    color: var(--text-primary);
    overflow-x: hidden;
    min-height: 100vh;
}

::-webkit-scrollbar { width: 8px; }
::-webkit-scrollbar-track { background: var(--bg-deep); }
::-webkit-scrollbar-thumb {
    background: var(--purple);
    border-radius: 4px;
}

#particles {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 0;
    pointer-events: none;
}

.ambient-runes {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 0;
    pointer-events: none;
    overflow: hidden;
}

.rune {
    position: absolute;
    font-size: 1.8rem;
    color: var(--purple);
    opacity: 0;
    animation: runeFloat 12s ease-in-out infinite;
    text-shadow: 0 0 15px var(--purple-glow);
}

.r1 { left: 5%;  top: 15%; animation-delay: 0s; }
.r2 { left: 90%; top: 25%; animation-delay: 1.5s; }
.r3 { left: 12%; top: 55%; animation-delay: 3s; }
.r4 { left: 85%; top: 65%; animation-delay: 4.5s; }
.r5 { left: 50%; top: 10%; animation-delay: 6s; }
.r6 { left: 30%; top: 80%; animation-delay: 7.5s; }
.r7 { left: 75%; top: 85%; animation-delay: 9s; }
.r8 { left: 60%; top: 45%; animation-delay: 10.5s; }

@keyframes runeFloat {
    0%, 100% {
        opacity: 0;
        transform: translateY(0) scale(0.8);
    }
    20% {
        opacity: 0.15;
    }
    50% {
        opacity: 0.25;
        transform: translateY(-30px) scale(1);
    }
    80% {
        opacity: 0.15;
    }
}

.hero {
    position: relative;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    background:
        radial-gradient(ellipse at 50% 30%, rgba(108, 63, 160, 0.15) 0%, transparent 60%),
        radial-gradient(ellipse at 20% 80%, rgba(45, 10, 78, 0.2) 0%, transparent 50%),
        radial-gradient(ellipse at 80% 70%, rgba(212, 160, 30, 0.05) 0%, transparent 40%),
        var(--bg-deep);
}

.hero-overlay {
    position: absolute;
    inset: 0;
    background:
        repeating-linear-gradient(
            0deg,
            transparent,
            transparent 2px,
            rgba(108, 63, 160, 0.02) 2px,
            rgba(108, 63, 160, 0.02) 4px
        );
    pointer-events: none;
}

.hero-content {
    position: relative;
    z-index: 2;
    text-align: center;
    padding: 2rem;
}

.arcane-circle {
    width: 180px;
    height: 180px;
    margin: 0 auto 2rem;
    animation: floatGentle 6s ease-in-out infinite;
}

.circle-svg {
    width: 100%;
    height: 100%;
    filter: drop-shadow(0 0 20px rgba(212, 160, 30, 0.3));
}

.outer-ring {
    fill: none;
    stroke: var(--gold);
    stroke-width: 1;
    stroke-dasharray: 8 4;
    opacity: 0.6;
    animation: spinSlow 30s linear infinite;
    transform-origin: center;
}

.inner-ring {
    fill: none;
    stroke: var(--purple-light);
    stroke-width: 1.5;
    stroke-dasharray: 15 5 5 5;
    opacity: 0.5;
    animation: spinSlow 20s linear infinite reverse;
    transform-origin: center;
}

.core-ring {
    fill: none;
    stroke: var(--gold-light);
    stroke-width: 0.8;
    opacity: 0.4;
    animation: pulseRing 4s ease-in-out infinite;
    transform-origin: center;
}

.circle-rune {
    font-size: 14px;
    fill: var(--gold);
    opacity: 0.7;
    font-family: serif;
}

@keyframes spinSlow {
    to { transform: rotate(360deg); }
}

@keyframes pulseRing {
    0%, 100% { opacity: 0.3; stroke-width: 0.8; }
    50% { opacity: 0.7; stroke-width: 1.5; }
}

@keyframes floatGentle {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-12px); }
}

.hero-pre {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.1rem;
    font-style: italic;
    color: var(--text-muted);
    letter-spacing: 0.3em;
    margin-bottom: 0.5rem;
    opacity: 0;
    animation: fadeInUp 1s ease 0.3s forwards;
}

.hero-title {
    font-family: 'Cinzel Decorative', 'Cinzel', serif;
    font-weight: 900;
    line-height: 1.1;
    margin-bottom: 1.2rem;
    opacity: 0;
    animation: fadeInUp 1s ease 0.6s forwards;
}

.title-line {
    display: block;
    font-size: clamp(3rem, 8vw, 5.5rem);
    color: var(--text-primary);
    text-shadow:
        0 0 40px rgba(108, 63, 160, 0.3),
        0 2px 10px rgba(0, 0, 0, 0.5);
}

.title-line.accent {
    font-size: clamp(3.5rem, 9vw, 6.5rem);
    background: linear-gradient(135deg, var(--gold-light), var(--gold), var(--gold-pale), var(--gold));
    background-size: 300% 300%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: shimmerGold 6s ease-in-out infinite;
    filter: drop-shadow(0 2px 15px rgba(212, 160, 30, 0.4));
}

@keyframes shimmerGold {
    0%, 100% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
}

.hero-subtitle {
    font-family: 'Cinzel', serif;
    font-size: clamp(0.85rem, 2vw, 1.1rem);
    color: var(--text-secondary);
    letter-spacing: 0.25em;
    text-transform: uppercase;
    opacity: 0;
    animation: fadeInUp 1s ease 0.9s forwards;
}

.scroll-indicator {
    margin-top: 3rem;
    opacity: 0;
    animation: fadeInUp 1s ease 1.2s forwards;
}

.scroll-indicator span {
    display: inline-block;
    font-size: 1.5rem;
    color: var(--gold);
    animation: bounce 2s ease-in-out infinite;
    text-shadow: 0 0 15px rgba(212, 160, 30, 0.4);
}

@keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(10px); }
}

@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(25px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

main {
    position: relative;
    z-index: 1;
}

.content-section {
    max-width: 800px;
    margin: 0 auto;
    padding: 4rem 2rem;
    opacity: 0;
    transform: translateY(40px);
    transition: opacity 0.8s ease, transform 0.8s ease;
}

.content-section.visible {
    opacity: 1;
    transform: translateY(0);
}

.section-header {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 1.5rem;
    margin-bottom: 3rem;
}

.section-header h2 {
    font-family: 'Cinzel', serif;
    font-weight: 700;
    font-size: clamp(1.5rem, 4vw, 2.2rem);
    color: var(--gold);
    text-transform: uppercase;
    letter-spacing: 0.15em;
    white-space: nowrap;
    text-shadow: 0 0 30px rgba(212, 160, 30, 0.2);
}

.ornament-line {
    flex: 1;
    height: 1px;
    max-width: 120px;
    position: relative;
}

.ornament-line::before {
    content: '';
    position: absolute;
    top: 0;
    width: 100%;
    height: 1px;
}

.ornament-line.left::before {
    right: 0;
    background: linear-gradient(to right, transparent, var(--gold));
}

.ornament-line.right::before {
    left: 0;
    background: linear-gradient(to left, transparent, var(--gold));
}

.section-body {
    position: relative;
    padding: 2.5rem;
    background:
        linear-gradient(135deg, rgba(22, 15, 36, 0.9), rgba(28, 20, 48, 0.8));
    border: 1px solid var(--border-subtle);
    border-radius: 4px;
    backdrop-filter: blur(10px);
}

.section-body::before {
    content: '';
    position: absolute;
    top: -1px;
    left: 10%;
    right: 10%;
    height: 1px;
    background: linear-gradient(to right, transparent, var(--gold), transparent);
}

.section-body::after {
    content: '';
    position: absolute;
    bottom: -1px;
    left: 10%;
    right: 10%;
    height: 1px;
    background: linear-gradient(to right, transparent, var(--purple-light), transparent);
}

.section-body p {
    font-size: 1.15rem;
    line-height: 1.9;
    color: var(--text-secondary);
    margin-bottom: 1.5rem;
    text-align: justify;
    text-indent: 2rem;
    hyphens: auto;
}

.section-body p:last-child {
    margin-bottom: 0;
}

/* Première lettre dorée */
.section-body p:first-child::first-letter {
    font-family: 'Cinzel Decorative', serif;
    font-size: 2.8rem;
    float: left;
    line-height: 1;
    margin-right: 0.04em;
    margin-top: 0.05em;
    color: var(--gold);
    text-shadow: 0 0 20px rgba(212, 160, 30, 0.3);
}

.section-body p:first-child {
    text-indent: 0;
}

.section-divider {
    text-align: center;
    padding: 2rem 0;
    position: relative;
}

.section-divider::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 300px;
    height: 1px;
    background: linear-gradient(to right, transparent, var(--border-gold), transparent);
}

.divider-rune {
    position: relative;
    z-index: 1;
    display: inline-block;
    font-size: 1.8rem;
    color: var(--gold);
    background: var(--bg-deep);
    padding: 0 1.5rem;
    text-shadow: 0 0 25px rgba(212, 160, 30, 0.4);
    animation: pulseGlow 3s ease-in-out infinite;
}

@keyframes pulseGlow {
    0%, 100% {
        text-shadow: 0 0 15px rgba(212, 160, 30, 0.3);
    }
    50% {
        text-shadow: 0 0 35px rgba(212, 160, 30, 0.6), 0 0 60px rgba(212, 160, 30, 0.2);
    }
}

.site-footer {
    text-align: center;
    padding: 4rem 2rem 3rem;
    position: relative;
}

.footer-ornament {
    font-size: 2.5rem;
    color: var(--gold);
    opacity: 0.4;
    margin-bottom: 1rem;
    text-shadow: 0 0 20px rgba(212, 160, 30, 0.3);
}

.footer-server {
    font-family: 'Cinzel', serif;
    font-size: 0.9rem;
    letter-spacing: 0.4em;
    text-transform: uppercase;
    color: var(--text-muted);
}

@media (max-width: 600px) {
    .section-body {
        padding: 1.5rem;
    }

    .section-body p {
        font-size: 1.05rem;
        text-indent: 1.2rem;
    }

    .content-section {
        padding: 3rem 1rem;
    }

    .section-header {
        gap: 0.8rem;
    }

    .ornament-line {
        max-width: 60px;
    }

    .arcane-circle {
        width: 130px;
        height: 130px;
    }
}
    </style>
</head>
<body>

<!-- Particules magiques -->
<canvas id="particles"></canvas>

<!-- Rune flottante ambiante -->
<div class="ambient-runes">
    <span class="rune r1">ᚨ</span>
    <span class="rune r2">ᛗ</span>
    <span class="rune r3">ᚠ</span>
    <span class="rune r4">ᛉ</span>
    <span class="rune r5">ᚦ</span>
    <span class="rune r6">ᛊ</span>
    <span class="rune r7">ᚲ</span>
    <span class="rune r8">ᛏ</span>
</div>

<!-- HERO -->
<header class="hero" id="hero">
    <div class="hero-overlay"></div>
    <div class="hero-content">
        <div class="arcane-circle">
            <svg viewBox="0 0 200 200" class="circle-svg">
                <circle cx="100" cy="100" r="90" class="outer-ring"/>
                <circle cx="100" cy="100" r="75" class="inner-ring"/>
                <circle cx="100" cy="100" r="60" class="core-ring"/>
                <text x="100" y="22" text-anchor="middle" class="circle-rune">ᚨ</text>
                <text x="178" y="105" text-anchor="middle" class="circle-rune">ᛗ</text>
                <text x="100" y="190" text-anchor="middle" class="circle-rune">ᚠ</text>
                <text x="22" y="105" text-anchor="middle" class="circle-rune">ᛉ</text>
            </svg>
        </div>
        <p class="hero-pre">— Présentation —</p>
        <h1 class="hero-title">
            <span class="title-line">Arkhavel</span>
            <span class="title-line accent">Dorne</span>
        </h1>
        <p class="hero-subtitle">Mage Ancien · Aspirant Conseiller du Conclave</p>
        <div class="scroll-indicator">
            <span>❧</span>
        </div>
    </div>
</header>

<!-- SECTION BACKGROUND -->
<main>
    <section class="content-section" id="background">
        <div class="section-header">
            <div class="ornament-line left"></div>
            <h2>Background</h2>
            <div class="ornament-line right"></div>
        </div>
        <div class="section-body">
            <p>Arkhavel Dorne est un mage humain ancien, dont l'âge exact reste difficile à déterminer. Depuis de nombreuses années, il s'est construit une expérience solide à travers différentes situations liées à l'usage de la magie, notamment dans des contextes instables ou mal maîtrisés.</p>
            <p>Sans appartenir officiellement à une institution, il a été amené à intervenir à plusieurs reprises lorsqu'il était question de conflits impliquant la magie. Il ne se place pas en première ligne, mais il ne reste jamais passif lorsque la situation l'exige.</p>
            <p>Au fil du temps, il s'est particulièrement intéressé aux règles qui encadrent l'usage de la magie, ainsi qu'aux conséquences qu'elle peut engendrer lorsqu'elle est utilisée sans cadre. Il s'est formé une bonne connaissance des principes anciens et des pratiques visant à limiter les dérives.</p>
            <p>Un événement marquant, survenu lors d'une expédition liée à une anomalie magique, a renforcé cette vision. Seul survivant, il en est revenu avec une approche plus mesurée, convaincu que la magie doit être encadrée pour éviter des situations incontrôlables.</p>
            <p>Aujourd'hui, Arkhavel reste quelqu'un de calme et réfléchi, mais capable de s'impliquer lorsque c'est nécessaire. Il privilégie l'analyse et le dialogue, tout en étant prêt à intervenir pour éviter que certaines situations ne dégénèrent.</p>
            <p>S'il souhaite aujourd'hui se rapprocher du Conclave, c'est pour mettre son expérience au service d'un cadre plus structuré, notamment dans l'encadrement et le jugement des pratiques magiques. Il estime pouvoir apporter une vision cohérente et mesurée dans des situations où les décisions doivent être prises avec recul.</p>
        </div>
    </section>

    <div class="section-divider">
        <span class="divider-rune">⚜</span>
    </div>

    <!-- SECTION CANDIDATURE -->
    <section class="content-section" id="candidature">
        <div class="section-header">
            <div class="ornament-line left"></div>
            <h2>Candidature Conseiller Conclave</h2>
            <div class="ornament-line right"></div>
        </div>
        <div class="section-body">
            <p>Je souhaite proposer mon personnage, Arkhavel Dorne, au rôle de conseiller du Conclave car il correspond à une position de recul, d'analyse et surtout de compréhension des règles qui encadrent la magie.</p>
            <p>Arkhavel est un mage ancien qui, avec le temps, s'est davantage tourné vers l'étude des lois et des pratiques liées à l'usage de la magie plutôt que vers sa simple utilisation. Il s'intéresse particulièrement aux dérives, aux anomalies et aux conséquences que peuvent entraîner certaines décisions. Cette approche me semble cohérente avec un rôle impliquant de juger ou d'accompagner des situations complexes.</p>
            <p>Je vois le rôle de conseiller comme une forme de garant de cohérence, notamment lors de conflits ou de situations nécessitant un cadre clair. L'objectif n'est pas de s'imposer dans les scènes, mais d'apporter une lecture posée et réfléchie, en s'appuyant sur les règles établies et les traditions du Conclave.</p>
            <p>En jeu, je souhaite utiliser ce rôle pour intervenir lors de situations liées à l'usage abusif ou dangereux de la magie, participer aux prises de décisions importantes, et aider à structurer un RP autour de la justice et de la responsabilité. L'idée est d'apporter un cadre sans bloquer les autres joueurs, mais en veillant à ce que les actions restent cohérentes avec l'univers.</p>
            <p>Cela fait plusieurs années que je pratique le roleplay, et je privilégie toujours la cohérence, le respect des autres joueurs et la qualité des interactions. Je ne cherche pas à être au centre, mais à jouer un rôle utile et structurant.</p>
            <p>Le rôle de conseiller correspond donc à la fois à mon personnage et à ma manière de jouer : observer, analyser, et intervenir avec mesure, en accord avec les lois et les principes du Conclave.</p>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="site-footer">
        <div class="footer-ornament">⚝</div>
        <p class="footer-server">Outland RP</p>
    </footer>
</main>

<script>
(function () {
    const canvas = document.getElementById('particles');
    const ctx = canvas.getContext('2d');
    let particles = [];
    let mouse = { x: -1000, y: -1000 };

    function resize() {
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;
    }
    resize();
    window.addEventListener('resize', resize);

    document.addEventListener('mousemove', (e) => {
        mouse.x = e.clientX;
        mouse.y = e.clientY;
    });

    class Particle {
        constructor() {
            this.reset();
        }
        reset() {
            this.x = Math.random() * canvas.width;
            this.y = Math.random() * canvas.height;
            this.size = Math.random() * 2 + 0.5;
            this.speedX = (Math.random() - 0.5) * 0.3;
            this.speedY = (Math.random() - 0.5) * 0.3 - 0.15;
            this.opacity = Math.random() * 0.5 + 0.1;
            this.fadeSpeed = Math.random() * 0.003 + 0.001;
            this.growing = Math.random() > 0.5;
            const isGold = Math.random() > 0.7;
            if (isGold) {
                this.r = 212; this.g = 160; this.b = 30;
            } else {
                this.r = 150; this.g = 100; this.b = 220;
            }
        }
        update() {
            this.x += this.speedX;
            this.y += this.speedY;
            const dx = mouse.x - this.x;
            const dy = mouse.y - this.y;
            const dist = Math.sqrt(dx * dx + dy * dy);
            if (dist < 200) {
                this.x += dx * 0.001;
                this.y += dy * 0.001;
                this.opacity = Math.min(this.opacity + 0.01, 0.8);
            }
            if (this.growing) {
                this.opacity += this.fadeSpeed;
                if (this.opacity >= 0.6) this.growing = false;
            } else {
                this.opacity -= this.fadeSpeed;
                if (this.opacity <= 0.05) this.reset();
            }
            if (this.x < 0 || this.x > canvas.width || this.y < 0 || this.y > canvas.height) {
                this.reset();
            }
        }
        draw() {
            ctx.beginPath();
            ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
            ctx.fillStyle = `rgba(${this.r},${this.g},${this.b},${this.opacity})`;
            ctx.shadowBlur = 15;
            ctx.shadowColor = `rgba(${this.r},${this.g},${this.b},0.5)`;
            ctx.fill();
            ctx.shadowBlur = 0;
        }
    }

    const count = Math.min(80, Math.floor(window.innerWidth / 15));
    for (let i = 0; i < count; i++) {
        particles.push(new Particle());
    }

    function animate() {
        ctx.clearRect(0, 0, canvas.width, canvas.height);
        particles.forEach(p => {
            p.update();
            p.draw();
        });
        requestAnimationFrame(animate);
    }
    animate();
})();

(function () {
    const sections = document.querySelectorAll('.content-section');
    const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.classList.add('visible');
            }
        });
    }, {
        threshold: 0.15,
        rootMargin: '0px 0px -50px 0px'
    });
    sections.forEach(s => observer.observe(s));
})();

(function () {
    const heroContent = document.querySelector('.hero-content');
    window.addEventListener('scroll', () => {
        const scrolled = window.scrollY;
        if (scrolled < window.innerHeight) {
            const opacity = 1 - scrolled / (window.innerHeight * 0.8);
            const translateY = scrolled * 0.3;
            heroContent.style.transform = `translateY(${translateY}px)`;
            heroContent.style.opacity = Math.max(0, opacity);
        }
    });
})();
</script>
</body>
</html>
