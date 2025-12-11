# celula2_S2_html

MiniOS

MiniOS es un prototipo de "sistema operativo" web construido únicamente con HTML y CSS, sin JavaScript. La interfaz principal (index.html) actúa como el escritorio/base y carga las distintas "aplicaciones" dentro de iframe, simulando componentes del sistema operativo (notas, clima, calculadora, tareas, calendario, etc.).

🔎 Propósito

El proyecto busca demostrar cómo estructurar y modularizar una interfaz multipestaña simulada usando sólo HTML y CSS (por ejemplo: :target, checkbox, radio o <select> para controlar la navegación). Es un ejercicio pedagógico para practicar accesibilidad, organización de archivos y despliegue en GitHub Pages, sin recurrir a lógica de programación.


📁 Estructura del proyecto

mini-os/
├── index.html
├── apps/
│   ├── calculator.html
│   ├── weather.html
│   ├── calendar.html
│   ├── note.html
│   └── homework.html
├── styles/
│   └── main.css
├── img/
│   └── ... (iconos y logos usados por el escritorio)
└── README.md

Nota: En el index.html proporcionado aparecen iconos y ventanas que cargan iframe apuntando a apps/*.html. Asegúrate de que los nombres de archivo dentro de apps/ coincidan con los src de los iframe (por ejemplo apps/calculator.html, apps/weather.html, etc.).

📌 Cómo visualizar el proyecto localmente

Clona el repositorio:

git clone https://github.com/<TU_USUARIO>/<REPO>.git
cd <REPO>

Abre index.html con tu navegador (doble click o Abrir con...).

No se necesita servidor ni dependencias. Si prefieres usar un servidor local (para evitar problemas con iframe en algunos navegadores), puedes usar uno sencillo como python -m http.server 8000 desde la carpeta raíz del proyecto y abrir http://localhost:8000.


🧭 Navegación (cómo funciona)

index.html actúa como "escritorio". Cada ícono es un enlace que apunta a un id o controla un elemento iframe.

Las aplicaciones están en apps/ y son páginas HTML independientes. Al hacer clic sobre un icono se muestra la ventana correspondiente con su iframe.

Ejemplos de mecanismos HTML para cambiar vistas sin JS:

Usar :target con anclas (#app1, #app2).

Usar input[type="radio"] o checkbox combinados con label y CSS para mostrar/ocultar ventanas.

Usar un <select> cuya selección pueda apuntar a un ancla o a una sección estilo :target.



🔗 Enlaces (poner los tuyos)

GitHub Repo: https://github.com/celula2Semana2html/celula2_S2_html

GitHub Pages: https://<TU_USUARIO>.github.io/<REPO>/


👥 Créditos

Camilo Urrego - 
Juan Pablo - 
Sebastian -
Valeria -
Tomas -

