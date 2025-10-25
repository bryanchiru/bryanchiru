## Hi there 👋

<!--
**bryanchiru/bryanchiru** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
¡Absolutamente! Aquí tienes el código completo de la página web, unificado en un solo bloque de texto.

Este formato está diseñado para que lo copies y pegues en dos archivos separados en tu repositorio de GitHub:

index.html (para la estructura)

style.css (para los estilos)

📄 Código Completo Unificado
1. Contenido del archivo index.html
HTML

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Josué M. - Estudiante de IA</title>

    <link rel="stylesheet" href="style.css">

    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>

    <header class="top-bar">
        <div class="container">
            <div class="logo">IA-ULAT</div>
        </div>
    </header>

    <section id="inicio" class="hero-claude">
        <div class="content-wrapper">
            <p class="subtitle">Estudiante de Inteligencia Artificial</p>
            <h1>Hola, soy <span>Josué M.</span></h1>
            <p class="tagline">Combino tecnología, datos e innovación.</p>

            <p class="description">
                Soy estudiante de Inteligencia Artificial en la Universidad Latina de Panamá, con una fuerte pasión por el aprendizaje automático, el análisis de datos y el desarrollo de soluciones inteligentes. Me interesa especialmente la aplicación de IA en problemas reales, desde clasificación y regresión hasta proyectos más complejos que integren múltiples técnicas de machine learning.
            </p>

            <a href="#proyectos" class="btn-proyectos">
                Ver Proyectos →
            </a>

            <div class="scroll-indicator"></div>
        </div>
    </section>

    <section id="proyectos" class="projects-section">
        <div class="content-wrapper">
            <h2>Proyectos y Trabajos</h2>
            <p class="section-subtitle">
                Repositorio de tareas y laboratorios del curso de IA
            </p>

            <div class="project-grid">

                <div class="project-card">
                    <div class="card-icon book-icon"></div>
                    <h3>Repositorio & Overview</h3>
                    <p class="card-description">
                        Configuración inicial del repositorio GitHub y documentación general del proyecto de Inteligencia Artificial.
                    </p>
                    <a href="#" class="btn-card-link">
                        Ver proyecto →
                    </a>
                </div>

                <div class="project-card">
                    <div class="card-icon brain-icon"></div>
                    <h3>Clasificación Binaria</h3>
                    <p class="card-description">
                        Implementación de algoritmos de clasificación binaria utilizando machine learning y análisis de datos.
                    </p>
                    <a href="#" class="btn-card-link">
                        Ver proyecto →
                    </a>
                </div>

                <div class="project-card">
                    <div class="card-icon chart-icon"></div>
                    <h3>Regresión</h3>
                    <p class="card-description">
                        Modelos de regresión para predicción de valores continuos y análisis estadístico de datos.
                    </p>
                    <a href="#" class="btn-card-link">
                        Ver proyecto →
                    </a>
                </div>

                <div class="project-card">
                    <div class="card-icon test-tube-icon"></div>
                    <h3>WebPage Lab</h3>
                    <p class="card-description">
                        Desarrollo de página web para presentación del portafolio de proyectos de IA.
                    </p>
                    <a href="#" class="btn-card-link">
                        Ver proyecto →
                    </a>
                </div>

            </div>
        </div>
    </section>

    <footer id="contacto">
        <div class="content-wrapper">
            <h2>Josué M.</h2>
            <p>Estudiante de Inteligencia Artificial</p>
            <p>Universidad Latina de Panamá</p>

            <div class="footer-icons">
                <a href="#proyectos" class="footer-link folder-icon" aria-label="Ir a Proyectos"></a>

                <a href="mailto:tu.correo@ejemplo.com" class="footer-link email-icon" aria-label="Enviar Correo"></a>

                <a href="#inicio" class="footer-link up-arrow-icon" aria-label="Volver Arriba"></a>
            </div>

            <p class="copyright">&copy; 2025 Josué M. – Todos los derechos reservados</p>
        </div>
    </footer>

</body>
</html>
2. Contenido del archivo style.css
CSS

/* Variables de color (ajustadas para el diseño) */
:root {
    --color-morado-oscuro: #2e084d;
    --color-morado-claro: #5a3c96;
    --color-blanco: #ffffff;
    --color-texto: #333;
    --color-acento: #4a90e2; /* Azul para resaltar Josué M. y enlaces */
    --color-fondo-claro: #eee;
}

/* -------------------- Estilos Generales y Reseteo -------------------- */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Roboto', sans-serif;
    color: var(--color-blanco);
    background-color: var(--color-morado-oscuro);
}

.container {
    max-width: 1100px;
    margin: auto;
    padding: 0 20px;
}

.content-wrapper {
    max-width: 600px; /* Ancho máximo para el contenido principal (simula un móvil) */
    margin: 0 auto;
    padding: 0 20px;
}

/* -------------------- 1. Cabecera (IA-ULAT) -------------------- */
.top-bar {
    background-color: #1f2a36; /* Color oscuro para la barra superior, diferente al fondo principal */
    padding: 15px 0;
    text-align: left;
    position: relative;
    z-index: 10;
}

.top-bar .logo {
    font-weight: 700;
    font-size: 1.2rem;
    padding-left: 20px;
}

/* -------------------- 2. Sección Hero (Fondo Degradado) -------------------- */
.hero-claude {
    /* Fondo degradado similar al de la imagen */
    background: linear-gradient(180deg, var(--color-morado-claro) 0%, var(--color-morado-oscuro) 100%);
    padding: 40px 0 80px 0;
    min-height: 85vh;
    position: relative;
    text-align: center;
}

.hero-claude .subtitle {
    font-size: 1rem;
    opacity: 0.8;
    margin-bottom: 5px;
}

.hero-claude h1 {
    font-size: 2.5rem;
    font-weight: 700;
    margin-bottom: 10px;
}

.hero-claude h1 span {
    color: var(--color-acento); /* Color para resaltar el nombre */
}

.hero-claude .tagline {
    font-size: 1.2rem;
    margin-bottom: 30px;
    opacity: 0.9;
}

.hero-claude .description {
    font-size: 1.1rem;
    line-height: 1.6;
    text-align: justify;
    margin-bottom: 40px;
    padding: 0 10px;
}

/* Botón "Ver Proyectos" */
.btn-proyectos {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 250px;
    padding: 15px 30px;
    background-color: var(--color-blanco);
    color: var(--color-morado-oscuro);
    text-decoration: none;
    font-weight: 700;
    font-size: 1.1rem;
    border-radius: 50px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
    transition: all 0.3s;
}

.btn-proyectos:hover {
    box-shadow: 0 6px 15px rgba(0, 0, 0, 0.3);
    transform: translateY(-2px);
}

.scroll-indicator {
    width: 20px;
    height: 5px;
    background-color: var(--color-blanco);
    opacity: 0.5;
    border-radius: 5px;
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
}

/* -------------------- 3. Sección de Proyectos -------------------- */
.projects-section {
    background-color: var(--color-morado-oscuro);
    padding: 60px 0;
    text-align: center;
}

.projects-section h2 {
    font-size: 2rem;
    font-weight: 700;
    color: var(--color-blanco);
    margin-bottom: 5px;
}

.projects-section .section-subtitle {
    font-size: 1.1rem;
    opacity: 0.7;
    margin-bottom: 40px;
    color: var(--color-blanco);
}

.project-grid {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
}

/* Estilo de la Tarjeta de Proyecto */
.project-card {
    background-color: var(--color-blanco);
    color: var(--color-texto);
    padding: 30px;
    width: 100%;
    max-width: 500px;
    border-radius: 15px;
    text-align: left;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.project-card:hover {
    transform: translateY(-5px);
}

/* -------------------- Iconos de las Tarjetas (Placeholders) -------------------- */
.card-icon {
    width: 40px;
    height: 40px;
    border-radius: 5px;
    margin-bottom: 15px;
    /* Para simular la forma del icono, se usa background-color */
}

.book-icon {
    background-color: #2196f3; /* Azul para libro */
}

.brain-icon {
    background-color: #e91e63; /* Rosa para cerebro */
}

.chart-icon {
    background: linear-gradient(90deg, #d32f2f 0%, #388e3c 45%, #1976d2 100%); /* Colores para gráfico */
}

.test-tube-icon {
    background-color: #00bcd4; /* Cyan para tubo de ensayo */
}

.project-card h3 {
    font-size: 1.5rem;
    margin-bottom: 10px;
}

.project-card .card-description {
    font-size: 1rem;
    line-height: 1.5;
    color: #666;
    margin-bottom: 20px;
}

/* Enlace "Ver proyecto →" */
.btn-card-link {
    color: var(--color-acento);
    text-decoration: none;
    font-weight: 700;
    transition: color 0.3s;
}

.btn-card-link:hover {
    color: var(--color-morado-claro);
}

/* -------------------- 4. Pie de Página (Footer) -------------------- */
footer {
    background-color: #2b3e50;
    color: var(--color-secundario);
    padding: 40px 0 20px 0;
    text-align: center;
}

footer h2 {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 5px;
    color: var(--color-blanco);
}

footer p {
    margin-bottom: 5px;
    opacity: 0.9;
}

.footer-icons {
    display: flex;
    justify-content: center;
    gap: 30px;
    margin: 20px 0;
}
/* Estilo para los Iconos del Footer */
.footer-link {
    display: block;
    width: 35px;
    height: 35px;
    border-radius: 5px;
    background-color: rgba(255, 255, 255, 0.1);
    transition: background-color 0.3s;
}

.footer-link:hover {
    background-color: rgba(255, 255, 255, 0.2);
}

/* Colores y formas para simular los iconos */
.folder-icon {
    background-color: #fbc02d; /* Carpeta */
}

.email-icon {
    background-color: #e57373; /* Correo */
}

.up-arrow-icon {
    background-color: #64b5f6; /* Flecha */
}

.copyright {
    font-size: 0.8rem;
    margin-top: 15px;
    opacity: 0.6;
}

/* -------------------- Adaptación a Móviles -------------------- */
@media (max-width: 650px) {
    .content-wrapper {
        padding: 0 10px;
    }
    
    .hero-claude h1 {
        font-size: 2rem;
    }

    .hero-claude .description {
        font-size: 1rem;
    }
    
    .project-card {
        padding: 20px;
    }
}
