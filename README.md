# 🎬 CinePlus - Proyecto Web


## 📌 Descripción del proyecto

CinePlus es una aplicación web que permite visualizar películas en cartelera, consultar detalles, ver tráilers, leer reseñas y realizar la renta de películas de manera interactiva. El proyecto utiliza tecnologías web básicas como HTML, CSS, JavaScript y AJAX para cargar contenido dinámicamente.

---

## 🚀 Funcionalidades implementadas

### 🎬 Gestión de películas

* Carga dinámica de películas desde `peliculas.json` usando AJAX.
* Estructura completa de datos:

  * id, título, géneros, imagen, sinopsis, tráiler, fecha de estreno y precios.
* Visualización de tarjetas de películas con animación.
* Botón para ver detalles de cada película.
* Botón para ver tráiler en ventana flotante.

---

### 💰 Sistema de precios dinámico

* Cálculo automático del precio según la fecha actual:

  * 🔴 Estreno → precio mayor
  * 🟢 Normal → precio regular
* Indicador visual (badge) en la página de detalle.

---

### ⏳ Simulación de carga

* Uso de `setTimeout` para simular carga AJAX de 5 segundos.
* Spinner de carga mientras se obtienen los datos.

---

### 🎥 Tráilers

* Visualización de tráilers en ventana flotante (overlay).
* Reproducción embebida desde YouTube.

---

### 📝 Página de detalle

* Información completa de la película:

  * Imagen, sinopsis, géneros y tráiler.
* Indicador dinámico de estado (estreno o normal).
* Precio actualizado.

---

### ⭐ Sistema de reseñas

* Carga de reseñas desde `resenas.json`.
* Filtrado por película.
* Visualización de calificación con estrellas (Bootstrap Icons).
* Entre 3 y 5 reseñas por película.

---

### 🍿 Sistema de renta

* Página `renta.html`.
* Selección dinámica de películas (sin hardcodear).
* Selección múltiple de películas.
* Elección de forma de pago.
* Cálculo automático del total según días y tipo de película.
* Modal con resumen de compra:

  * Cliente
  * Películas seleccionadas
  * Días
  * Total a pagar

---

### 📩 Formulario de contacto

* Validación personalizada:

  * Nombre mínimo 3 caracteres
  * Correo válido
  * Mensaje entre 20 y 50 caracteres
* Mensajes de error dinámicos.

---

### 🎨 Diseño y experiencia de usuario

* Uso de Bootstrap 5.
* Tipografía personalizada con Google Fonts (Poppins).
* Diseño moderno con efectos hover y sombras.
* Animaciones al mostrar películas.
* Estrellas visuales para reseñas.

---

### 🧠 Funcionalidades adicionales

* Mensaje de bienvenida (solo una vez) usando `localStorage`.
* Navbar presente en todas las páginas.
* Resaltado automático de la página activa.
* Footer fijo en la parte inferior del navegador.

---

## 🛠️ Tecnologías utilizadas

* HTML5
* CSS3
* JavaScript (jQuery)
* AJAX
* Bootstrap 5
* Bootstrap Icons

---

## 📂 Estructura del proyecto

```
/codigo-1_44
│── index.html
│
├── css/
│   └── style.css
│
├── data/
│   ├── peliculas.json
│   └── resenas.json
│
├── img/
│   └── (imágenes de películas)
│
├── js/
│   └── app.js
│
└── pages/
    ├── detalle.html
    ├── contacto.html
    └── renta.html
```

---

## ▶️ Instrucciones de uso

1. Abrir el proyecto con **Live Server** en Visual Studio Code.
2. Navegar a `index.html`.
3. Explorar las películas disponibles.
4. Hacer clic en:

   * **Ver más** → ver detalles
   * **Ver tráiler** → abrir video
   * **Rentar** → alquilar película
5. Completar el formulario de renta para ver el resumen.
6. Probar el formulario de contacto con validaciones.

---

## ⚠️ Notas

* Es necesario ejecutar el proyecto con un servidor local (Live Server) para que AJAX funcione correctamente.
* Verificar que las imágenes estén en la carpeta `/img`.
* Mantener la estructura de los archivos JSON para evitar errores.

---


