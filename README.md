<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Perfil de Wuider Joseph</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Arial', sans-serif;
            color: #f0f0f0;
            background-color: #0f0f1f;
            margin: 0;
            padding: 0;
        }

        header {
            text-align: center;
            padding: 2rem;
            background-color: #1a1a2e;
        }

        h1, h2, h3 {
            color: #08f7fe;
            text-shadow: 0 0 10px #08f7fe;
        }

        .highlight {
            color: #ff2e63;
        }

        section {
            margin: 2rem 0;
            padding: 2rem;
            background-color: #1a1a2e;
            border-radius: 15px;
            box-shadow: 0 0 15px #08f7fe;
        }

        ul {
            list-style: none;
            padding: 0;
        }

        ul li {
            margin-bottom: 0.5rem;
        }

        /* Projects */
        .project {
            margin-bottom: 1rem;
            padding: 1rem;
            background-color: #162447;
            border-left: 5px solid #08f7fe;
        }

        /* Contact Section */
        a {
            color: #ff2e63;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }

        footer {
            text-align: center;
            padding: 2rem;
            background-color: #1a1a2e;
            color: #f0f0f0;
        }

        /* Animations */
        @keyframes neon-glow {
            0% {
                text-shadow: 0 0 5px #08f7fe, 0 0 10px #08f7fe;
            }
            50% {
                text-shadow: 0 0 20px #08f7fe, 0 0 30px #08f7fe;
            }
            100% {
                text-shadow: 0 0 5px #08f7fe, 0 0 10px #08f7fe;
            }
        }

        h1 {
            animation: neon-glow 2s infinite alternate;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            section {
                padding: 1rem;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Wuider Joseph Chancahuaña Garcia</h1>
    <p class="highlight">"No te juzgues por tus caídas, juzga por cómo te levantarás"</p>
</header>

<section id="about">
    <h2>Sobre Mí</h2>
    <p>Soy estudiante de programación en la carrera de Computación e Informática, egresado del Instituto Fibertel. Actualmente, estoy iniciando en el mundo del Front-End. Mi objetivo es crecer cada día más como programador.</p>
</section>

<section id="skills">
    <h2>Habilidades</h2>
    <ul>
        <li>Java</li>
        <li>Python</li>
        <li>PHP</li>
        <li>MySQL</li>
        <li>SQL Server</li>
        <li>Desarrollo de CRUD</li>
        <li>APIs</li>
        <li>Arquitectura de Sistemas</li>
        <li>Principios SOLID</li>
    </ul>
</section>

<section id="projects">
    <h2>Proyectos</h2>
    <div class="project">
        <h3>CRUD de Productos</h3>
        <p>Aplicación de CRUD completa que permite registrar, listar, editar y eliminar productos con imágenes almacenadas.</p>
    </div>
    <div class="project">
        <h3>CRUD de Alimentos</h3>
        <p>Un sistema de CRUD enfocado en la gestión de alimentos, aplicando principios de arquitectura limpia y patrones de diseño.</p>
    </div>
</section>

<section id="contact">
    <h2>Contacto</h2>
    <p>Email: <a href="mailto:wuider29@gmail.com">wuider29@gmail.com</a></p>
    <p>Teléfono: <a href="tel:+123456789">+123456789</a></p>
    <button id="contact-button">¡Contáctame!</button>
</section>

<footer>
    <p>Creado por Wuider Joseph Chancahuaña Garcia</p>
</footer>

<script>
    document.addEventListener("DOMContentLoaded", () => {
        const contactButton = document.querySelector("#contact-button");

        if (contactButton) {
            contactButton.addEventListener("click", () => {
                alert("Gracias por tu interés! Te responderé lo antes posible.");
            });
        }

        const projectCards = document.querySelectorAll(".project");
        projectCards.forEach((card) => {
            card.addEventListener("mouseover", () => {
                card.style.transform = "scale(1.05)";
                card.style.transition = "transform 0.2s";
            });

            card.addEventListener("mouseout", () => {
                card.style.transform = "scale(1)";
            });
        });
    });
</script>

</body>
</html>
