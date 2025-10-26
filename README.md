## Hi there 👋

<!--
**bryanchiru/bryanchiru** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
¡Absolutamente! Aquí tienes el código completo de la página web, unificado en un solo bloque de texto.

Este formato está diseñado para que lo copies y pegues en dos archivos separados en tu repositorio de GitHub:
Entendido. El código anterior no funcionó exactamente como esperabas. Vamos a crear un nuevo formato más vistoso, fácil de leer y estructurado para GitHub Pages, con todos los apartados específicos que solicitaste para Bryan Chiru V.

Este diseño utilizará una estructura moderna de una sola página con enlaces a secciones (los "sublinks") y se dividirá, nuevamente, en dos archivos esenciales: index.html y style.css.

1. Archivo: index.html (Estructura)
Copia este código y guárdalo como index.html.

HTML

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bryan Chiru V. - Ingeniero Biomédico y AI</title>
    
    <link rel="stylesheet" href="style.css">
    
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>

    <section id="inicio" class="hero-section">
        <div class="content-wrapper">
            <p class="greeting">Hola, soy</p>
            <h1>Bryan Chiru</h1>
            <h2 class="subtitle">Ingeniería Biomédica | Inteligencia Artificial</h2>
            <p class="summary">
                Apasionado por la **Ingeniería Biomédica**, enfocado en la aplicación de la **Inteligencia Artificial** para crear soluciones innovadoras en el diagnóstico y tratamiento médico. Combino el análisis de datos con el conocimiento biológico para impulsar la tecnología de la salud.
            </p>
            <a href="#proyectos" class="btn-action">Ver Proyectos Destacados <i class="fas fa-arrow-down"></i></a>
        </div>
    </section>

    <section id="proyectos" class="projects-section">
        <div class="content-wrapper">
            <h2 class="section-title">Proyectos y Trabajos de IA</h2>
            <p class="section-description">
                Explora los temas clave y las implementaciones desarrolladas en el curso de Inteligencia Artificial.
            </p>
            
            <div class="project-grid">

                <div class="project-card">
                    <i class="fas fa-folder-open card-icon"></i>
                    <h3>Repositorio y Overview</h3>
                    <p>Documentación general del proyecto de IA y estructura inicial del código en GitHub.</p>
                    <a href="repositorio.html" class="btn-detail">
                        Ir al Tema →
                    </a>
                </div>

                <div class="project-card">
                    <i class="fas fa-brain card-icon"></i>
                    <h3>Clasificación Binaria</h3>
                    <p>Implementación de modelos de Machine Learning para problemas de clasificación binaria.</p>
                    <a href="clasificacion.html" class="btn-detail">
                        Ir al Tema →
                    </a>
                </div>

                <div class="project-card">
                    <i class="fas fa-chart-bar card-icon"></i>
                    <h3>Análisis de Datos</h3>
                    <p>Procesamiento, limpieza y visualización de grandes conjuntos de datos para la toma de decisiones.</p>
                    <a href="analisis.html" class="btn-detail">
                        Ir al Tema →
                    </a>
                </div>

            </div>
        </div>
    </section>

    <section id="resena" class="info-section">
        <div class="content-wrapper">
            <h2 class="section-title">Información Personal (Reseña)</h2>
            <div class="info-details">
                <p><span>Nombre Completo:</span> Bryan Chiru V</p>
                <p><span>Cédula:</span> 8-957-855</p>
                <p><span>Materia:</span> Inteligencia Artificial</p>
                <p><span>Carrera:</span> Ingeniería Biomédica</p>
            </div>
            <p class="contact-prompt">Conéctate conmigo en <a href="https://github.com/tu-usuario-github" target="_blank">GitHub</a>.</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Bryan Chiru V. | Todos los derechos reservados.</p>
    </footer>

</body>
</html>
2. Archivo: style.css (Estilos Vistosos)
Copia este código y guárdalo como style.css. Este código dará un diseño limpio, profesional y bien espaciado.

CSS

/* Variables de Estilo */
:root {
    --color-primary: #007bff; /* Azul vibrante */
    --color-secondary: #f4f4f4; /* Fondo suave */
    --color-dark: #333;
    --color-light: #fff;
    --font-family-main: 'Poppins', sans-serif;
    --padding-section: 80px 0;
}

/* Reset y Base */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: var(--font-family-main);
    line-height: 1.6;
    color: var(--color-dark);
    background-color: var(--color-secondary);
}

a {
    text-decoration: none;
    color: var(--color-primary);
}

.content-wrapper {
    max-width: 960px;
    margin: 0 auto;
    padding: 0 20px;
}

/* -------------------- 1. Sección Hero (Inicio / Saludo) -------------------- */
.hero-section {
    background: linear-gradient(135deg, var(--color-primary) 0%, #0056b3 100%); /* Degradado vistoso */
    color: var(--color-light);
    min-height: 100vh;
    display: flex;
    align-items: center;
    text-align: center;
    padding: var(--padding-section);
}

.hero-section .content-wrapper {
    max-width: 700px;
}

.greeting {
    font-size: 1.2rem;
    font-weight: 300;
    opacity: 0.8;
}

.hero-section h1 {
    font-size: 4rem;
    font-weight: 700;
    margin: 5px 0 10px 0;
}

.subtitle {
    font-size: 1.5rem;
    font-weight: 500;
    margin-bottom: 25px;
    color: #e0f0ff;
}

.summary {
    font-size: 1.1rem;
    margin-bottom: 40px;
    line-height: 1.8;
}

.btn-action {
    display: inline-block;
    background-color: var(--color-light);
    color: var(--color-primary);
    padding: 12px 25px;
    border-radius: 50px;
    font-weight: 700;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    transition: background-color 0.3s, transform 0.3s;
}

.btn-action:hover {
    background-color: var(--color-secondary);
    transform: translateY(-2px);
}

/* -------------------- 2. Sección Proyectos -------------------- */
.projects-section {
    padding: var(--padding-section);
    background-color: var(--color-light);
    text-align: center;
}

.section-title {
    font-size: 2.5rem;
    font-weight: 700;
    color: var(--color-primary);
    margin-bottom: 10px;
}

.section-description {
    font-size: 1.1rem;
    color: #666;
    margin-bottom: 50px;
}

.project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
}

.project-card {
    background-color: var(--color-secondary);
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
    transition: transform 0.3s, box-shadow 0.3s;
    text-align: left;
}

.project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
}

.card-icon {
    font-size: 2rem;
    color: var(--color-primary);
    margin-bottom: 15px;
}

.project-card h3 {
    font-size: 1.5rem;
    margin-bottom: 10px;
    color: var(--color-dark);
}

.btn-detail {
    display: inline-block;
    color: var(--color-primary);
    font-weight: 500;
    margin-top: 15px;
    transition: color 0.3s;
}

.btn-detail:hover {
    color: #0056b3;
}

/* -------------------- 3. Sección Reseña / Info -------------------- */
.info-section {
    padding: var(--padding-section);
    background-color: #e9ecef; /* Color de fondo contrastante */
    text-align: center;
}

.info-details {
    margin: 30px auto;
    max-width: 450px;
    padding: 20px;
    background-color: var(--color-light);
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    text-align: left;
}

.info-details p {
    margin-bottom: 10px;
    font-size: 1.1rem;
}

.info-details span {
    font-weight: 700;
    color: var(--color-primary);
    display: inline-block;
    width: 150px; /* Alineación de claves */
}

.contact-prompt {
    font-size: 1.1rem;
    margin-top: 30px;
}

/* -------------------- 4. Pie de Página -------------------- */
footer {
    background-color: var(--color-dark);
    color: var(--color-secondary);
    text-align: center;
    padding: 20px 0;
    font-size: 0.9rem;
}

/* Adaptación a Móviles */
@media (max-width: 768px) {
    .hero-section h1 {
        font-size: 3rem;
    }
    .subtitle {
        font-size: 1.2rem;
    }
    .section-title {
        font-size: 2rem;
    }
    .info-details span {
        display: block;
        width: 100%;
        margin-bottom: 0;
    }
    .info-details p {
        margin-bottom: 15px;
    }
}
