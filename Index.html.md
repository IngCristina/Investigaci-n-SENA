<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SENA - Orientar Investigación Formativa</title>
    <!-- Tailwind CSS para diseño moderno -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Work Sans y Montserrat (Moderno y Profesional) -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Work+Sans:wght@300;400;600&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        :root {
            --sena-green: #39A900;
            --sena-black: #000000;
            --sena-white: #FFFFFF;
            --sena-gray: #F4F4F4;
        }

        body {
            font-family: 'Work Sans', sans-serif;
            background-color: var(--sena-gray);
            color: #333;
        }

        h1, h2, h3, .nav-title {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
        }

        .sena-gradient {
            background: linear-gradient(135deg, var(--sena-green) 0%, #2e8600 100%);
        }

        .card-hover:hover {
            transform: translateY(-5px);
            transition: all 0.3s ease;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .instructor-img {
            border: 4px solid var(--sena-green);
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        ::-webkit-scrollbar-thumb {
            background: var(--sena-green);
            border-radius: 10px;
        }

        .animate-fade-in {
            animation: fadeIn 1s ease-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body class="antialiased">

    <!-- Navegación -->
    <nav class="bg-white shadow-md sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20 items-center">
                <div class="flex items-center space-x-4">
                    <img src="https://www.sena.edu.co/Style%20Library/alayout/images/logoSena.png" alt="Logo SENA" class="h-12 w-auto">
                    <div class="hidden md:block">
                        <span class="text-xs text-gray-500 block">Investigación</span>
                        <span class="text-sm font-bold text-gray-800 uppercase tracking-wider">SENA</span>
                    </div>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#inicio" class="text-gray-600 hover:text-green-600 font-medium transition">Inicio</a>
                    <a href="#competencia" class="text-gray-600 hover:text-green-600 font-medium transition">Competencia</a>
                    <a href="#resultados" class="text-gray-600 hover:text-green-600 font-medium transition">Resultados</a>
                    <a href="#instructor" class="text-gray-600 hover:text-green-600 font-medium transition">Instructor</a>
                    <a href="#recursos" class="bg-green-600 text-white px-4 py-2 rounded-lg hover:bg-green-700 transition flex items-center">
                        <i data-lucide="folder-open" class="w-4 h-4 mr-2"></i> Recursos
                    </a>
                </div>
                <!-- Botón móvil -->
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-button" class="text-gray-600">
                        <i data-lucide="menu" class="w-6 h-6"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Menú móvil -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-gray-100 p-4 space-y-4">
            <a href="#inicio" class="block text-gray-600 font-medium">Inicio</a>
            <a href="#competencia" class="block text-gray-600 font-medium">Competencia</a>
            <a href="#resultados" class="block text-gray-600 font-medium">Resultados</a>
            <a href="#instructor" class="block text-gray-600 font-medium">Instructor</a>
            <a href="#recursos" class="block text-green-600 font-bold">Recursos</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <header id="inicio" class="sena-gradient text-white py-20 px-4">
        <div class="max-w-5xl mx-auto text-center animate-fade-in">
            <div class="inline-block bg-white/20 backdrop-blur-md px-4 py-1 rounded-full text-sm font-semibold mb-6">
                Guía de Aprendizaje
            </div>
            <h1 class="text-4xl md:text-6xl font-extrabold mb-6 leading-tight">
                Orientar Investigación Formativa según Referentes Técnicos
            </h1>
            <p class="text-lg md:text-xl text-green-50 mb-8 max-w-3xl mx-auto leading-relaxed">
                "La investigación no es solo un proceso académico, sino una herramienta poderosa para la toma de decisiones, la resolución de problemas y la innovación."
            </p>
            <div class="flex flex-wrap justify-center gap-4">
                <div class="flex items-center bg-black/20 px-6 py-3 rounded-xl border border-white/30">
                    <i data-lucide="clock" class="w-5 h-5 mr-3"></i>
                    <span><strong>48 Horas</strong> (34 Dir. + 14 Aut.)</span>
                </div>
                <div class="flex items-center bg-black/20 px-6 py-3 rounded-xl border border-white/30">
                    <i data-lucide="search" class="w-5 h-5 mr-3"></i>
                    <span>Orientar investigación formativa según referentes técnicos</span>
                </div>
            </div>
        </div>
    </header>

    <!-- Mensaje de Bienvenida -->
    <section class="py-16 px-4 bg-white">
        <div class="max-w-4xl mx-auto">
            <div class="bg-gray-50 p-8 rounded-3xl border-l-8 border-green-600 shadow-sm">
                <h2 class="text-2xl font-bold text-gray-800 mb-4 flex items-center">
                    <i data-lucide="sparkles" class="text-green-600 mr-2"></i> Bienvenida al Proceso Formativo
                </h2>
                <div class="text-gray-700 leading-relaxed space-y-4 text-lg italic">
                    <p>
                        "¡Bienvenido a este desafío de innovación!. Investigar no es solo un ejercicio académico; es la herramienta clave para transformar tu entorno profesional."            </p>
                    <p>
                        "El desarrollo de la competencia de investigación te permite potenciar tu capacidad de cuestionamiento y construcción de conocimiento. Esta guía ha sido diseñada para orientar tu aprendizaje de forma organizada, integrando tus conocimientos previos con metodologías sólidas útiles para identificar necesidades reales en los sectores productivos y a estructurar proyectos que no solo funcionen en el papel, sino que impacten positivamente en la eficiencia y la sostenibilidad de las organizaciones"
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Competencia y Resultados -->
    <section id="competencia" class="py-20 px-4 bg-gray-50">
        <div class="max-w-6xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-900 mb-4">Competencia a Desarrollar</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Orientar la investigación formativa de acuerdo a referencias técnicas para impactar el sector productivo logístico.</p>
            </div>

            <div id="resultados" class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Resultado 1 -->
                <div class="bg-white p-6 rounded-2xl shadow-sm card-hover border-b-4 border-green-500">
                    <div class="w-12 h-12 bg-green-100 rounded-lg flex items-center justify-center mb-4">
                        <i data-lucide="bar-chart-3" class="text-green-600"></i>
                    </div>
                    <h3 class="font-bold text-gray-800 mb-2">Contexto Productivo</h3>
                    <p class="text-sm text-gray-600">Analizar el contexto productivo según sus características y necesidades específicas.</p>
                </div>

                <!-- Resultado 2 -->
                <div class="bg-white p-6 rounded-2xl shadow-sm card-hover border-b-4 border-blue-500">
                    <div class="w-12 h-12 bg-blue-100 rounded-lg flex items-center justify-center mb-4">
                        <i data-lucide="layout" class="text-blue-600"></i>
                    </div>
                    <h3 class="font-bold text-gray-800 mb-2">Estructuración</h3>
                    <p class="text-sm text-gray-600">Estructurar el proyecto de investigación de acuerdo con los criterios técnicos.</p>
                </div>

                <!-- Resultado 3 -->
                <div class="bg-white p-6 rounded-2xl shadow-sm card-hover border-b-4 border-purple-500">
                    <div class="w-12 h-12 bg-purple-100 rounded-lg flex items-center justify-center mb-4">
                        <i data-lucide="book-open" class="text-purple-600"></i>
                    </div>
                    <h3 class="font-bold text-gray-800 mb-2">Argumentación</h3>
                    <p class="text-sm text-gray-600">Argumentar aspectos teóricos basados en referencias nacionales e internacionales.</p>
                </div>

                <!-- Resultado 4 -->
                <div class="bg-white p-6 rounded-2xl shadow-sm card-hover border-b-4 border-orange-500">
                    <div class="w-12 h-12 bg-orange-100 rounded-lg flex items-center justify-center mb-4">
                        <i data-lucide="lightbulb" class="text-orange-600"></i>
                    </div>
                    <h3 class="font-bold text-gray-800 mb-2">Solución</h3>
                    <p class="text-sm text-gray-600">Proponer soluciones innovadoras a partir de los resultados obtenidos.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Información del Instructor -->
    <section id="instructor" class="py-20 px-4 bg-white">
        <div class="max-w-5xl mx-auto flex flex-col md:flex-row items-center gap-12">
            <div class="md:w-1/3 text-center">
                <div class="relative inline-block">
                    <div class="w-48 h-48 rounded-full bg-gray-200 overflow-hidden mx-auto instructor-img shadow-xl">
                        <!-- Imagen representativa -->
                         <img src="https://media.licdn.com/dms/image/v2/D4E03AQEq1l-q5PgUXQ/profile-displayphoto-scale_200_200/B4EZiFqO_1GYAY-/0/1754589102696?e=2147483647&v=beta&t=dJDitGoTZAcbEaRUpxMju-WhZAAt7rAjJAOrAZL6HZU">
                    </div>
                    <div class="absolute bottom-2 right-2 bg-green-600 p-2 rounded-full text-white shadow-lg">
                        <i data-lucide="badge-check" class="w-6 h-6"></i>
                    </div>
                </div>
            </div>
            <div class="md:w-2/3">
                <span class="text-green-600 font-bold uppercase tracking-widest text-sm">Instructor Líder</span>
                <h2 class="text-4xl font-bold text-gray-900 mt-2 mb-4">Cristina Ramírez M.</h2>
                <p class="text-xl text-gray-700 mb-6 leading-relaxed">
                   Magíster en Ingeniería Industrial, Investigadora Junior, Instructora y docente universitaria. Con sólida experiencia liderando grupos de investigación y ejecutando proyectos de I+D+i en el sector productivo y académico.
                </p>
                <div class="grid grid-cols-2 gap-4">
                    <div class="flex items-center space-x-2 text-gray-600">
                        <a href="https://scholar.google.com/citations?user=wJNamvsAAAAJ&hl=es" class="flex items-center space-x-2 text-gray-600" target="_blank">
                            <i data-lucide="graduation-cap" class="w-5 h-5 text-green-600"></i>
                            <span>Publicaciones</span>
                        </a>
                    </div>
                    <div class="flex items-center space-x-2 text-gray-600">
                        <i data-lucide="microscope" class="w-5 h-5 text-green-600"></i>
                        <span>Investigadora</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Recursos -->
    <section id="recursos" class="py-20 px-4 sena-gradient">
        <div class="max-w-4xl mx-auto text-center text-white ">
            <h2 class="text-3xl font-bold mb-8">Repositorio de Aprendizaje</h2>
            <p class="text-xl mb-10 opacity-90">Accede a las guías, plantillas, bibliografía y formatos necesarios para el desarrollo de tu proyecto de investigación.</p>
            <div class="flex justify-center gap-6 mb-8">
                <a href="https://gemini.google.com/share/15ba3cf6e630">
                    <i data-lucide="external-link" class="mr-3"></i>
                    Abrir Carpeta de Materiales
                </a>
                <button id="btn" class="inline-flex items-center bg-white text-green-700 font-bold px-10 py-5 rounded-2xl shadow-2xl hover:bg-gray-100 transition-all transform hover:scale-105">🔊 Escuchar audio</button>
                <audio id="audio" src="https://www.dropbox.com/scl/fi/mel5n1gel5isvlopvflu2/De_operarios_a_innovadores_en_el_SENA.mp3?rlkey=2oyj5u344qbgbwtdoexek0hf2&st=hv531vxd&dl=1"></audio>
                <button id="btnEnlaces" class="inline-flex items-center bg-white text-green-700 font-bold px-10 py-5 rounded-2xl shadow-2xl hover:bg-gray-100 transition-all transform hover:scale-105">Enlaces</button>
            </div>
        </div>
    </section>


    <!-- Modal Enlaces -->

    <div id="modalEnlaces" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50 hidden">
        <div class="bg-white rounded-xl max-w-md w-full p-6 relative">
            <h3 class="text-xl font-bold mb-4 text-green-700">Recursos y Enlaces</h3>

            <!-- Lista de enlaces -->
            <ul id="listaEnlaces" class="space-y-3"></ul>

            <div id="paginacion" class="flex justify-between mt-4 hidden">
                <button id="prevPage" class="px-3 py-1 bg-gray-200 rounded hover:bg-gray-300">⬅ Anterior</button>
                <span id="pageInfo" class="text-gray-700 font-bold"></span>
                <button id="nextPage" class="px-3 py-1 bg-gray-200 rounded hover:bg-gray-300">Siguiente ➡</button>
            </div>


            <!-- Botón cerrar -->
            <button id="cerrarModal" class="absolute top-3 right-3 text-gray-500 hover:text-gray-800 font-bold text-xl">&times;</button>
        </div>
    </div>


    <!-- Footer -->
    <footer class="bg-black text-white py-12 px-4">
        <div class="max-w-7xl mx-auto grid md:grid-cols-3 gap-8 border-b border-gray-800 pb-10">
            <div>
                <img src="https://upload.wikimedia.org/wikipedia/commons/8/83/Sena_Colombia_logo.svg" alt="SENA" class="h-16 invert mb-6">
                <p class="text-gray-400">Servicio Nacional de Aprendizaje - SENA. Centro de Gestión de Mercados, Logística y TI.</p>
            </div>
            <div>
                <h4 class="font-bold text-lg mb-4">Secciones</h4>
                <ul class="space-y-2 text-gray-400">
                    <li><a href="#inicio" class="hover:text-green-500 transition">Inicio</a></li>
                    <li><a href="#competencia" class="hover:text-green-500 transition">Competencia</a></li>
                    <li><a href="#resultados" class="hover:text-green-500 transition">Aprendizaje</a></li>
                </ul>
            </div>
            <div>
                <h4 class="font-bold text-lg mb-4">Contacto</h4>
                <p class="text-gray-400 italic">"Aquí nace la innovación que transforma al país."</p>
                <div class="mt-4 flex space-x-4">
                    <i data-lucide="mail" class="text-green-500"></i>
                    <span class="text-gray-400">Sennova </span>
                </div>
            </div>
        </div>
        <div class="text-center mt-10 text-gray-500 text-sm">
            &copy; 2025 SENA - Todos los derechos reservados.
        </div>
    </footer>

    <script>
        // Inicializar Iconos Lucide
        lucide.createIcons();

        // Control del menú móvil
        const menuBtn = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        const btnEnlaces = document.getElementById("btnEnlaces");
        const modalEnlaces = document.getElementById("modalEnlaces");
        const cerrarModal = document.getElementById("cerrarModal");
        const audio = document.getElementById("audio");
        const btn = document.getElementById("btn");
        let playing = false;

        const listaEnlaces = document.getElementById("listaEnlaces");
        const prevPage = document.getElementById("prevPage");
        const nextPage = document.getElementById("nextPage");
        const pageInfo = document.getElementById("pageInfo");
        const paginacion = document.getElementById("paginacion");
        

        // AGREGAR ENLACES AQUI!!
        const enlaces = [
            { nombre: "Un mundo sin Ciencia", url: "https://www.youtube.com/watch?v=ENLicID9Tew" },
            { nombre: "CONPES 4069", url: "https://minciencias.gov.co/conpes-4069-nueva-politica-ciencia-tecnologia-e-innovacion-2022-2031" },
            { nombre: "Investigación-SENA", url: "https://www.sena.edu.co/es-co/formacion/Paginas/Competitividad-y-Desarrollo-Tecnologico-Productivo.aspx" },
            { nombre: "Fake news sobre cambio climático", url: "https://www.bbc.com/mundo/articles/cg3p1xy93z7o" },
            { nombre: "El Cambio climático no existe", url: "https://www.youtube.com/shorts/MqxVLWjw428" },
            { nombre: "El cementerio de ropa usada ", url: "https://www.youtube.com/watch?v=0HZl9_MhwFc" },
            { nombre: "Islas de plástico en los océanos", url: "https://www.youtube.com/watch?v=Yd5RNwmLQ8w" },
            { nombre: "Basura electrónica", url: "https://www.youtube.com/watch?v=Aadj-IEZWZg" },
            { nombre: "La verdad sobre la moda rápida", url: "https://www.youtube.com/watch?v=7Y18UAF8M68" },
            { nombre: "Tecnologías Emergentes", url: "https://es.weforum.org/stories/2025/06/top-10-tecnologias-emergentes-2025/" },
            { nombre: "5 reglas para salir de la ignoracia", url: "https://www.youtube.com/watch?v=RHdSvrePu-c" },
            { nombre: "Últimos Inventos", url: "https://technologyreview.es/" }

        ];

        let paginaActual = 1;
        const itemsPorPag = 5;
        const totalPag = Math.ceil(enlaces.length / itemsPorPag);



        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Cerrar menú móvil al hacer clic en un enlace
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // Smooth Scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        btn.addEventListener("click", () => {
            if (!playing) {
                audio.play();
                btn.textContent = "⏸ Pausar audio";
            } else {
                audio.pause();
                btn.textContent = "🔊 Escuchar audio";
            }
            playing = !playing;
        });

        // Abrir modal
        btnEnlaces.addEventListener("click", () => {
            modalEnlaces.classList.remove("hidden");
        });

        // Cerrar modal
        cerrarModal.addEventListener("click", () => {
            modalEnlaces.classList.add("hidden");
        });

        // Cerrar modal al hacer click fuera del contenido
        modalEnlaces.addEventListener("click", (e) => {
            if(e.target === modalEnlaces){
                modalEnlaces.classList.add("hidden");
            }
        });

        function renderPag(pag) {
            listaEnlaces.innerHTML = "";

            const start = (pag - 1) * itemsPorPag;
            const end = start + itemsPorPag;
            const pageItems = enlaces.slice(start, end);

            pageItems.forEach(item => {
                const li = document.createElement("li");
                li.className = "flex justify-between items-center bg-gray-100 px-3 py-2 rounded-lg";
                li.innerHTML = `
                    <span>${item.nombre}</span>
                    <a href="${item.url}" target="_blank" class="text-green-700 font-bold hover:underline">🔗</a>
                `;
                listaEnlaces.appendChild(li);
            });

            pageInfo.textContent = `Página ${paginaActual} de ${totalPag}`;
            paginacion.classList.toggle("hidden", totalPag <= 1);

            prevPage.disabled = paginaActual === 1;
            nextPage.disabled = paginaActual === totalPag;
        }

        prevPage.addEventListener("click", () => {
            if (paginaActual > 1) {
                paginaActual--;
                renderPag(paginaActual);
            }
        });

        nextPage.addEventListener("click", () => {
            if (paginaActual < totalPag) {
                paginaActual++;
                renderPag(paginaActual);
            }
        });

        renderPag(paginaActual);
    </script>
</body>
</html>
