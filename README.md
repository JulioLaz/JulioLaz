<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <title>Perfil de GitHub</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" integrity="sha512-jh0NnXGQkKOQobG4bULKl1wZmEzDm+I7DwSqf4xK+lv8+ms9kNlvwPprfk5toJsyM3I5RP1gj6tjyu9oZdze7Q==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            line-height: 1.6;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }

        header img {
            border-radius: 50%;
            width: 150px;
            height: 150px;
            margin-bottom: 10px;
        }

        section {
            background-color: #fff;
            padding: 20px;
            margin: 20px 0;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        h1{
         margin: 0 !important;
        }
        
        h2 {
           color: #333;
           border-bottom: 2px solid #ccc;
           padding-bottom: 10px;
           margin-bottom: 20px;
         }
         
         h3{
          font-size: 1.8rem;
          margin: 0 !important;
         }

        .info {
            margin-bottom: 20px;
            display: flex;
            flex-direction: row;
            justify-content: center;
        }

        .info h3 {
            margin-bottom: 10px;
        }

        .info p {
            margin: 0 10px;
        }

        .info a {
            color: #007bff;
            text-decoration: none;
        }

        .info a:hover {
            text-decoration: underline;
        }

        ul {
            list-style: none;
            padding: 0;
        }

        ul li {
            margin-bottom: 5px;
        }
        .encabezado{
         display: flex;
         flex-direction: row;
        }
        .img_name_redes{
         width: 30vw !important;
         /* display: flex;
         flex-direction: row; */
         
        }
    </style>
</head>
<body>
    <header>
      <div class="encabezado">
         <div class="img_name_redes">
               <img src="https://avatars.githubusercontent.com/u/108642139?v=4" alt="Perfil">
               <h1 id="nombre"></h1>
               <h3 id="profesion"></h3>
               <div class="info">
                  <p id="linkedin"></p>
                  <p id="github"></p>
                  <p id="email"></p>
                  <p id="web"></p>
            </div>
         </div>
         <div style="width: 40%;text-align: justify;">
            <p id="about_me"></p>
         </div>
      </div>
    </header>
    <section id="educacion">
        <h2>Educación</h2>
    </section>
    <section id="experiencia">
        <h2>Experiencia Laboral</h2>
    </section>
    <section id="habilidades">
        <h2>Habilidades</h2>
    </section>
    <section id="proyectos">
        <h2>Proyectos Destacados</h2>
    </section>

    <script>
document.addEventListener("DOMContentLoaded", function () {
    var perfil = {
        "persona": {
            "nombre": "Julio Alberto Lazarte",
            "apellido": "Lazarte",
            "email": "julioalbertolazarte00@gmail.com",
            "email_00": "julioalazarte@yahoo.com",
            "profesion": "Data Scientist",
            "profesion_00": "Data Scientist & Full Stack Developer Jr",
            "title_about": "Sobre mi vida:",
            "edad": "46 años",
            "city": "Argentina, Tucumán",
            "img": "https://avatars.githubusercontent.com/u/108642139?v=4",
            "about_me": "Soy Julio Lazarte, científico de datos especializado en el análisis, visualización, machine learning, business intelligence. Mi objetivo es lograr insight que aporten valor a las necesidades de empresas, para optimizar recursos, reducir gastos, prevenir pérdidas, generar mayores ingresos económico.\nMi formación tiene distintos pilares, por un lado en ciencias exactas con ingeniería, y por otro lado con formación humanística con filosofía.\nAdemás de formarme como Full stack Developer, actualmente me estoy profesionalizando en Ciencias de Datos en donde encontré mi pasión.",
        },
        "educacion": [
            {
                "id": 1,
                "titlee": "Bootcamp Data Science",
                "schoole": "El profe Alejo",
                "starte": "2023",
                "ende": "2024",
                "citye": "Online",
                "timee": "12 meses",
                "estadoe": "Cursando",
                "imge": "https://i.imgur.com/uFyPLXv.png",
                "url": "https://bootcampxperience.com/"
            },
            {
                "id": 19,
                "titlee": "Bootcamp Data Science",
                "schoole": "Alura Latan",
                "starte": "2023",
                "ende": "2023",
                "citye": "Online",
                "timee": "6 meses",
                "estadoe": "Completado",
                "imge": "https://i.imgur.com/BNCHUv5.png",
                "url": "https://www.aluracursos.com/bootcamp-datos"
            },
            // Resto de la educación
        ],
        "experiencia": [
            {
                "id": 5,
                "title": "Docente de Filosofía",
                "company": "Ministerio de Educación",
                "start": "1997",
                "end": "Presente",
                "city": "Tucumán, Argentina",
                "description": "Impartir clases de Filosofía en distintos niveles educativos, desde secundario hasta universitario."
            },
            // Resto de la experiencia laboral
        ],
        "habilidades": {
            "programacion": {
                "HTML": 90,
                "CSS": 85,
                "JavaScript": 85,
                "Python": 80,
                "Java": 70,
                "C++": 60
            },
            // Resto de las habilidades
        },
        "proyectos": [
            {
                "id": 1,
                "title": "Sistema de Gestión Escolar",
                "description": "Desarrollo de un sistema web para la gestión de estudiantes, docentes, asignaturas, notas, y demás aspectos relacionados con una institución educativa. Tecnologías utilizadas: Node.js, Express.js, MongoDB, Angular.",
                "url": "https://github.com/tuproject/sistema-gestion-escolar"
            },
            // Resto de los proyectos
        ],
        "redes": {
            "linkedin": "https://www.linkedin.com/in/julio-lazarte-developer/",
            "github": "https://github.com/JulioLaz",
            "email": "julioalbertolazarte00@gmail.com",
            "web": "https://cv-lazarte-julio.web.app/"
        }
    };

    // Llenar los datos estáticos
    document.getElementById("nombre").textContent += perfil.persona.nombre;
    document.getElementById("about_me").textContent += perfil.persona.about_me;
    document.getElementById("profesion").textContent += perfil.persona.profesion;
   document.getElementById("linkedin").innerHTML += `<a href="${perfil.redes.linkedin}"><svg width="24px" height="24px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M6.5 8C7.32843 8 8 7.32843 8 6.5C8 5.67157 7.32843 5 6.5 5C5.67157 5 5 5.67157 5 6.5C5 7.32843 5.67157 8 6.5 8Z" fill="#518ef0"></path> <path d="M5 10C5 9.44772 5.44772 9 6 9H7C7.55228 9 8 9.44771 8 10V18C8 18.5523 7.55228 19 7 19H6C5.44772 19 5 18.5523 5 18V10Z" fill="#518ef0"></path> <path d="M11 19H12C12.5523 19 13 18.5523 13 18V13.5C13 12 16 11 16 13V18.0004C16 18.5527 16.4477 19 17 19H18C18.5523 19 19 18.5523 19 18V12C19 10 17.5 9 15.5 9C13.5 9 13 10.5 13 10.5V10C13 9.44771 12.5523 9 12 9H11C10.4477 9 10 9.44772 10 10V18C10 18.5523 10.4477 19 11 19Z" fill="#518ef0"></path> <path fill-rule="evenodd" clip-rule="evenodd" d="M20 1C21.6569 1 23 2.34315 23 4V20C23 21.6569 21.6569 23 20 23H4C2.34315 23 1 21.6569 1 20V4C1 2.34315 2.34315 1 4 1H20ZM20 3C20.5523 3 21 3.44772 21 4V20C21 20.5523 20.5523 21 20 21H4C3.44772 21 3 20.5523 3 20V4C3 3.44772 3.44772 3 4 3H20Z" fill="#518ef0"></path> </g></svg></a>`; //color #518ef0
    document.getElementById("email").innerHTML += `<a href="${perfil.redes.linkedin}"><svg width="28px" height="28px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M4 7.00005L10.2 11.65C11.2667 12.45 12.7333 12.45 13.8 11.65L20 7" stroke="#518ef0" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path> <rect x="3" y="5" width="18" height="14" rx="2" stroke="#518ef0" stroke-width="2" stroke-linecap="round"></rect> </g></svg></a>`;
    document.getElementById("web").innerHTML += `<a href="${perfil.redes.linkedin}"><svg width="30px" height="30px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path fill-rule="evenodd" clip-rule="evenodd" d="M9.83824 18.4467C10.0103 18.7692 10.1826 19.0598 10.3473 19.3173C8.59745 18.9238 7.07906 17.9187 6.02838 16.5383C6.72181 16.1478 7.60995 15.743 8.67766 15.4468C8.98112 16.637 9.40924 17.6423 9.83824 18.4467ZM11.1618 17.7408C10.7891 17.0421 10.4156 16.1695 10.1465 15.1356C10.7258 15.0496 11.3442 15 12.0001 15C12.6559 15 13.2743 15.0496 13.8535 15.1355C13.5844 16.1695 13.2109 17.0421 12.8382 17.7408C12.5394 18.3011 12.2417 18.7484 12 19.0757C11.7583 18.7484 11.4606 18.3011 11.1618 17.7408ZM9.75 12C9.75 12.5841 9.7893 13.1385 9.8586 13.6619C10.5269 13.5594 11.2414 13.5 12.0001 13.5C12.7587 13.5 13.4732 13.5593 14.1414 13.6619C14.2107 13.1384 14.25 12.5841 14.25 12C14.25 11.4159 14.2107 10.8616 14.1414 10.3381C13.4732 10.4406 12.7587 10.5 12.0001 10.5C11.2414 10.5 10.5269 10.4406 9.8586 10.3381C9.7893 10.8615 9.75 11.4159 9.75 12ZM8.38688 10.0288C8.29977 10.6478 8.25 11.3054 8.25 12C8.25 12.6946 8.29977 13.3522 8.38688 13.9712C7.11338 14.3131 6.05882 14.7952 5.24324 15.2591C4.76698 14.2736 4.5 13.168 4.5 12C4.5 10.832 4.76698 9.72644 5.24323 8.74088C6.05872 9.20472 7.1133 9.68686 8.38688 10.0288ZM10.1465 8.86445C10.7258 8.95042 11.3442 9 12.0001 9C12.6559 9 13.2743 8.95043 13.8535 8.86447C13.5844 7.83055 13.2109 6.95793 12.8382 6.2592C12.5394 5.69894 12.2417 5.25156 12 4.92432C11.7583 5.25156 11.4606 5.69894 11.1618 6.25918C10.7891 6.95791 10.4156 7.83053 10.1465 8.86445ZM15.6131 10.0289C15.7002 10.6479 15.75 11.3055 15.75 12C15.75 12.6946 15.7002 13.3521 15.6131 13.9711C16.8866 14.3131 17.9412 14.7952 18.7568 15.2591C19.233 14.2735 19.5 13.1679 19.5 12C19.5 10.8321 19.233 9.72647 18.7568 8.74093C17.9413 9.20477 16.8867 9.6869 15.6131 10.0289ZM17.9716 7.46178C17.2781 7.85231 16.39 8.25705 15.3224 8.55328C15.0189 7.36304 14.5908 6.35769 14.1618 5.55332C13.9897 5.23077 13.8174 4.94025 13.6527 4.6827C15.4026 5.07623 16.921 6.08136 17.9716 7.46178ZM8.67765 8.55325C7.61001 8.25701 6.7219 7.85227 6.02839 7.46173C7.07906 6.08134 8.59745 5.07623 10.3472 4.6827C10.1826 4.94025 10.0103 5.23076 9.83823 5.5533C9.40924 6.35767 8.98112 7.36301 8.67765 8.55325ZM15.3224 15.4467C15.0189 16.637 14.5908 17.6423 14.1618 18.4467C13.9897 18.7692 13.8174 19.0598 13.6527 19.3173C15.4026 18.9238 16.921 17.9186 17.9717 16.5382C17.2782 16.1477 16.3901 15.743 15.3224 15.4467ZM12 21C16.9706 21 21 16.9706 21 12C21 7.02944 16.9706 3 12 3C7.02944 3 3 7.02944 3 12C3 16.9706 7.02944 21 12 21Z" fill="#518ef0"></path> </g></svg></a>`;
    document.getElementById("github").innerHTML += `<a href="${perfil.redes.github}"><svg width="26px" height="26px" viewBox="0 0 20 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" fill="#000000" stroke="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <title>github [#142]</title> <desc>Created with Sketch.</desc> <defs> </defs> <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd"> <g id="Dribbble-Light-Preview" transform="translate(-140.000000, -7559.000000)" fill="#518ef0"> <g id="icons" transform="translate(56.000000, 160.000000)"> <path d="M94,7399 C99.523,7399 104,7403.59 104,7409.253 C104,7413.782 101.138,7417.624 97.167,7418.981 C96.66,7419.082 96.48,7418.762 96.48,7418.489 C96.48,7418.151 96.492,7417.047 96.492,7415.675 C96.492,7414.719 96.172,7414.095 95.813,7413.777 C98.04,7413.523 100.38,7412.656 100.38,7408.718 C100.38,7407.598 99.992,7406.684 99.35,7405.966 C99.454,7405.707 99.797,7404.664 99.252,7403.252 C99.252,7403.252 98.414,7402.977 96.505,7404.303 C95.706,7404.076 94.85,7403.962 94,7403.958 C93.15,7403.962 92.295,7404.076 91.497,7404.303 C89.586,7402.977 88.746,7403.252 88.746,7403.252 C88.203,7404.664 88.546,7405.707 88.649,7405.966 C88.01,7406.684 87.619,7407.598 87.619,7408.718 C87.619,7412.646 89.954,7413.526 92.175,7413.785 C91.889,7414.041 91.63,7414.493 91.54,7415.156 C90.97,7415.418 89.522,7415.871 88.63,7414.304 C88.63,7414.304 88.101,7413.319 87.097,7413.247 C87.097,7413.247 86.122,7413.234 87.029,7413.87 C87.029,7413.87 87.684,7414.185 88.139,7415.37 C88.139,7415.37 88.726,7417.2 91.508,7416.58 C91.513,7417.437 91.522,7418.245 91.522,7418.489 C91.522,7418.76 91.338,7419.077 90.839,7418.982 C86.865,7417.627 84,7413.783 84,7409.253 C84,7403.59 88.478,7399 94,7399" id="github-[#142]"> </path> </g> </g> </g> </g></svg></a>`;

    // Llenar la educación
    var educacionHTML = '';
    perfil.educacion.forEach(function (educacion) {
        educacionHTML += `
            <div>
                <h3>${educacion.titlee}</h3>
                <p>${educacion.schoole} - ${educacion.citye}</p>
                <p>${educacion.starte} - ${educacion.ende}</p>
                <p>${educacion.estadoe}</p>
            </div>
        `;
    });
    document.getElementById("educacion").innerHTML += educacionHTML;

    // Llenar la experiencia laboral
    var experienciaHTML = '';
    perfil.experiencia.forEach(function (experiencia) {
        experienciaHTML += `
            <div>
                <h3>${experiencia.title}</h3>
                <p>${experiencia.company} - ${experiencia.city}</p>
                <p>${experiencia.start} - ${experiencia.end}</p>
                <p>${experiencia.description}</p>
            </div>
        `;
    });
    document.getElementById("experiencia").innerHTML += experienciaHTML;

    // Llenar las habilidades
    var habilidadesHTML = '';
    habilidadesHTML += `
        <h3>Programación</h3>
        <ul>
    `;
    for (var lenguaje in perfil.habilidades.programacion) {
        habilidadesHTML += `<li>${lenguaje} - ${perfil.habilidades.programacion[lenguaje]}%</li>`;
    }
    habilidadesHTML += '</ul>';

    document.getElementById("habilidades").innerHTML += habilidadesHTML;

    // Llenar los proyectos
    var proyectosHTML = '';
    perfil.proyectos.forEach(function (proyecto) {
        proyectosHTML += `
            <div>
                <h3>${proyecto.title}</h3>
                <p>${proyecto.description}</p>
                <p><a href="${proyecto.url}">Ver en GitHub</a></p>
            </div>
        `;
    });
    document.getElementById("proyectos").innerHTML += proyectosHTML;
});    </script>
</body>
</html>
