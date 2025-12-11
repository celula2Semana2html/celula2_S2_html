# MiniOS

MiniOS es un prototipo de "sistema operativo" web construido únicamente con **HTML y CSS**, sin JavaScript. La interfaz principal (`index.html`) actúa como el escritorio/base y carga las distintas "aplicaciones" dentro de `iframe`, simulando componentes del sistema operativo (notas, clima, calculadora, tareas, calendario, etc.).

---

## 🔎 Propósito

El proyecto busca demostrar cómo estructurar y modularizar una interfaz multipestaña simulada usando solo HTML y CSS (por ejemplo: `:target`, `checkbox`, `radio` o `<select>` para controlar la navegación). Es un ejercicio pedagógico para practicar accesibilidad, organización de archivos y despliegue en GitHub Pages, sin usar lógica de programación.

---

## 📁 Estructura del proyecto

La estructura del proyecto sigue esta organización:

```
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
│   └── ... iconos usados por el escritorio
└── README.md
```

Imagen de referencia:

<img width="1066" height="469" alt="image" src="https://github.com/user-attachments/assets/1ef4bcfe-41ff-445a-921f-2745d3d2d90b" />

> **Nota:** En el `index.html` aparecen iconos y ventanas que cargan `iframe` apuntando a `apps/*.html`. Asegúrate de que los nombres de archivo dentro de `apps/` coincidan con los `src` de los `iframe`.

---

## 📌 Cómo visualizar el proyecto localmente

1. Clona el repositorio:

```bash
git clone https://github.com/celula2Semana2html/celula2_S2_html.git
cd celula2_S2_html
```

2. Abre `index.html` en tu navegador (doble clic o "Abrir con...").

> No se necesita servidor ni dependencias. Si deseas usar un servidor local para evitar posibles bloqueos de `iframe`, puedes ejecutar:

```bash
python -m http.server 8000
```

Luego abre en tu navegador:

```
http://localhost:8000
```

---

## 🧭 Navegación (cómo funciona)

* `index.html` actúa como el "escritorio" del sistema.
* Cada ícono funciona como un enlace que muestra una ventana (`div.window`).
* Cada ventana carga un archivo independiente dentro de un `iframe`, desde la carpeta `apps/`.

### Métodos HTML utilizados para navegar sin JavaScript

* Uso de `:target` con anclas como `#app1`, `#app2`, etc.
* Uso de `input[type="radio"]` o `checkbox` con `label` para mostrar/ocultar ventanas.
* Uso de un `<select>` que apunta a anclas o secciones controladas por CSS.

---

## 🔗 Enlaces

* **Repositorio GitHub:** [https://github.com/celula2Semana2html/celula2_S2_html](https://github.com/celula2Semana2html/celula2_S2_html)
* **GitHub Pages:** [https://celula2Semana2html.github.io/celula2_S2_html/](https://celula2Semana2html.github.io/celula2_S2_html/)

---

## 👥 Créditos

Equipo de desarrollo:

* **Camilo Urrego**
* **Juan Pablo**
* **Sebastián**
* **Valeria**
* **Tomás**

---
