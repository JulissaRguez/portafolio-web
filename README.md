<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Currículum Julissa</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" crossorigin="anonymous" />
    <style>
        :root {
            --bg-main: #F1EFEC;
            --panel-bg: #D4C9BE;
            --accent: #123458;
            --text: #030303;
            --light: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--bg-main);
            color: var(--text);
            line-height: 1.6;
        }

        .container {
            max-width: 1100px;
            margin: 40px auto;
            display: grid;
            grid-template-columns: 1fr 2fr;
            background: var(--light);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.1);
            animation: fadeIn 1s ease-in-out;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .left-panel {
            background-color: var(--panel-bg);
            padding: 40px 30px;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }

            .left-panel img {
                width: 150px;
                height: 150px;
                object-fit: cover;
                border-radius: 50%;
                border: 5px solid var(--accent);
                margin-bottom: 20px;
            }

            .left-panel h2 {
                color: var(--accent);
                margin-bottom: 12px;
                font-size: 18px;
                text-transform: uppercase;
                letter-spacing: 1px;
            }

            .left-panel p {
                font-size: 14px;
                margin: 5px 0;
            }

            .left-panel .icon {
                color: var(--accent);
                margin-right: 8px;
            }

        .skills, .languages {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 8px;
            margin-top: 10px;
        }

            .skills span, .languages span {
                background: var(--accent);
                color: var(--light);
                padding: 6px 12px;
                border-radius: 20px;
                font-size: 12px;
            }

        .right-panel {
            padding: 50px;
        }

            .right-panel h1 {
                color: var(--accent);
                font-size: 34px;
                margin-bottom: 5px;
            }

        .section {
            margin-top: 25px;
            display: none;
            animation: fadeIn 0.5s ease-in-out;
        }

            .section.active {
                display: block;
            }

            .section h2 {
                font-size: 20px;
                color: var(--accent);
                margin-bottom: 10px;
                border-left: 4px solid var(--accent);
                padding-left: 10px;
                text-transform: uppercase;
            }

            .section p, .section li {
                font-size: 15px;
                margin-bottom: 8px;
            }

        .nav-buttons {
            display: flex;
            gap: 10px;
            margin-top: 20px;
        }

            .nav-buttons button {
                background: var(--accent);
                color: var(--light);
                border: none;
                padding: 10px 20px;
                border-radius: 10px;
                cursor: pointer;
                transition: background 0.3s ease;
            }

                .nav-buttons button:hover {
                    background: #0e2b48;
                }

        ul {
            margin-left: 20px;
        }

        @media (max-width: 768px) {
            .container {
                grid-template-columns: 1fr;
            }

            .right-panel {
                padding: 30px 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="left-panel">
            <img src="Img/jr.png" alt="Foto de Julissa" />
            <h2>Contacto</h2>
            <p><i class="fas fa-phone icon"></i> +52 631-116-6668</p>
            <p><i class="fas fa-envelope icon"></i> julissarguez02@gmail.com</p>
            <p><i class="fas fa-map-marker-alt icon"></i> Calle San Fernando #44, Col. San Carlos, Heroica Nogales, Sonora</p>

            <h2>Idiomas</h2>
            <div class="languages">
                <span>Español - Nativo</span>
                <span>Inglés - Intermedio</span>
            </div>

            <h2>Habilidades</h2>
            <div class="skills">
                <span>Comunicación</span>
                <span>Trabajo en equipo</span>
                <span>Bajo presión</span>
                <span>Resolución de problemas</span>
                <span>Office</span>
                <span>C#</span>
                <span>Python</span>
                <span>SQL Server</span>
                <span>MRP</span>
                <span>Inventarios</span>
            </div>
        </div>

        <div class="right-panel">
            <h1>Julissa Rodriguez Mendez</h1>
            <div class="nav-buttons">
                <button onclick="showSection('sobreMi')">Sobre mí</button>
                <button onclick="showSection('experiencia')">Experiencia</button>
                <button onclick="showSection('academico')">Académico</button>
            </div>

            <div id="sobreMi" class="section active">
                <h2>Sobre mí</h2>
                <p>Me defino por ser una persona con ganas de aprender cosas nuevas en cualquier ámbito. Soy muy dedicada con mis tareas asignadas y buen líder en equipos de trabajo.</p>
            </div>

            <div id="experiencia" class="section">
                <h2>Experiencia laboral</h2>
                <p><strong>Anderson Forest Products INC.</strong> | Julio 2023 - Marzo 2024</p>
                <p><em>Asistente de Sistemas</em></p>
                <ul>
                    <li>Cableado de redes</li>
                    <li>Soporte a computadoras e impresoras</li>
                    <li>Colocación de cámaras</li>
                    <li>Manejo de software MRP</li>
                    <li>Backups con SQL Server Management Studio</li>
                    <li>Servicio a servidor</li>
                </ul>

                <p><strong>Ancor Tools and Plastics</strong> | Enero 2025 - Actualmente</p>
                <p><em>Operadora de producción</em></p>
                <ul>
                    <li>Producción de ductos de aire acondicionado de carro Honda</li>
                    <li>Producción de porta vasos</li>
                    <li>Producción de cajas para pagar peajes</li>
                </ul>
            </div>

            <div id="academico" class="section">
                <h2>Datos académicos</h2>
                <p><strong>Cecyte Nogales Sonora</strong><br>Técnico en programación | 2018 - 2021</p>
                <p><strong>Instituto Tecnológico de Nogales Sonora</strong><br>Ingeniería en Sistemas Computacionales | 2021 - Actual</p>
                <p>Estudiante de 8vo semestre</p>
            </div>
        </div>
    </div>

    <script>function showSection(id) {
      document.querySelectorAll('.section').forEach(section => {
        section.classList.remove('active');
      });
      document.getElementById(id).classList.add('active');
    }</script>
</body>
</html>
