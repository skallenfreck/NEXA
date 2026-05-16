# NEXA — Guía de Organización de Archivos
Proyecto de Alfabetización Digital para Adultos Mayores
Fundación Universitaria Konrad Lorenz · 2026

## Estructura de Carpetas

Organice su carpeta local exactamente así:

```
NEXA/                         ← Carpeta principal del proyecto
│
├── index.html                ← Menú principal (página de inicio)
├── salud.html                ← Sección de Salud
├── ocio.html                 ← Sección de Ocio
├── servicios.html            ← Sección de Servicios Públicos
├── styles.css                ← Estilos visuales (NO modificar sin conocimiento)
│
└── imagenes/                 ← Carpeta para sus fotos e infografías
    ├── infografia-salud.png
    ├── infografia-ocio.png
    └── infografia-servicios.png
```

## Cómo Agregar sus Propias Imágenes

1. Cree una carpeta llamada **imagenes** dentro de la carpeta NEXA.
2. Guarde sus imágenes ahí con los nombres indicados arriba.
3. En cada archivo HTML, reemplace el bloque `<div class="imagen-placeholder">...</div>`
   por la etiqueta de imagen correspondiente:

   ```html
   <img src="imagenes/infografia-salud.png" alt="Descripción de la imagen" />
   ```

## Cómo Cambiar los Videos de YouTube

En cada archivo HTML encontrará un `<iframe>` con el atributo `src`.
Para cambiar el video:

1. Vaya a YouTube y abra el video que desea usar.
2. Copie el código del video de la URL. Por ejemplo:
   - URL: `https://www.youtube.com/watch?v=ABC123XYZ`
   - Código: `ABC123XYZ`
3. En el archivo HTML, reemplace el src así:
   ```html
   src="https://www.youtube.com/embed/ABC123XYZ"
   ```

## Cómo Abrir la Plataforma Localmente

1. Abra la carpeta NEXA en su computador.
2. Haga doble clic sobre el archivo **index.html**.
3. Se abrirá automáticamente en su navegador (Chrome, Firefox, Edge, etc.)
4. ¡Listo! La plataforma funciona sin necesidad de internet para navegar entre páginas.
   (Solo necesita internet para que se carguen los videos de YouTube.)

## Agregar Nuevas Secciones

Para agregar una nueva sección (por ejemplo, "Banca en Línea"):

1. Copie el archivo `salud.html` y renómbrelo, por ejemplo: `banca.html`
2. Cambie el título, contenido y colores según corresponda.
3. En `index.html`, agregue una nueva `<a>` dentro del `<div class="grid-secciones">`:

   ```html
   <a href="banca.html" class="tarjeta-seccion" style="background-color: #1A5276;">
     <span class="icono">🏦</span>
     <span class="titulo-seccion">BANCA EN LÍNEA</span>
     <span class="desc-seccion">Consultas y pagos desde su banco</span>
   </a>
   ```

## Personalización de Colores

Todos los colores se controlan desde `styles.css` en la sección `:root`.
Cambie los valores hexadecimales según la identidad visual que desee.

---
Documento técnico — Equipo NEXA 2026
Alexander Chacon, Cristian Amado, Javier Barreto, Salim Ferez, Lizeth Pastran, Mauricio Moreno.
