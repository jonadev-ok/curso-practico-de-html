<img width="1280" height="250" alt="portadas (3)" src="https://github.com/user-attachments/assets/259e34b6-8c15-4862-9108-f8f949779826" />

<h1>Optimización, Rendimiento y Buenas Prácticas en HTML</h1>

<p>
  En esta sección vamos a repasar, reforzar y profundizar conceptos ya vistos a lo largo del curso, y ver algunos otros que, van a dar 
  mayor rendimiento al desarrollo de sus proyectos en HTML.
</p>

<h2>Estructura y Semántica Correcta</h2>

<p>
  Objetivo: mejorar la accesibilidad, el SEO y la mantenibilidad.
</p>

<ul>
  <li>
    Usa etiquetas semánticas: 
    <a href="https://github.com/jonadev-ok/curso-practico-de-html/blob/main/Curso/Modulo-02/README.md">
      consultar aqui
    </a>
  </li>
  <li>
    Evita usar divs innecesarios.
  </li>
  <li>
    Usa encabezados jerarquicos de forma logica.
  </li>
</ul>

<h2>Optimización de carga</h2>
<p>
  Objetivo: mejorar la velocidad percibida y real de carga de la página.
</p>
<ul>
  <li>
    Minimiza el HTML (usa herramientas como HTMLMinifier o el proceso de build del framework).
  </li>
  <li>
    Evita comentarios innecesarios en producción.
  </li>
  <li>
    Usa lazy loading para imágenes y recursos:

    
```    
    <img src="imagen.jpg" loading="lazy" alt="Descripción" />
```

    
  </li>
  <li>
    Coloca los scripts al final del body o usa defer:


 ```
    <script src="app.js" defer></script>
```   
  </li>
</ul>

<h2>Optimización de Imágenes</h2>

<p>
  Objetivo: reducir el peso sin perder calidad.
</p>

<ul>
  <li>
    Usa formatos modernos (.webp, .avif).
  </li>
  <li>
    Adapta el tamaño según el dispositivo (srcset y sizes):
    
```
    <img src="img.jpg"
     srcset="img-400.jpg 400w, img-800.jpg 800w"
     sizes="(max-width: 600px) 400px, 800px"
     alt="Ejemplo optimizado">
```

  </li>
  <li>
    Comprime las imágenes.
  </li>
  <li>
    Elimina metadatos EXIF innecesarios.
  </li>
</ul>

<h2>Accesibilidad Web (a11y)</h2>

<p>
  Objetivo: permitir que todas las personas puedan navegar correctamente.
</p>

<ul>
  <li>
    Siempre usar alt en imágenes.
  </li>
  <li>
    Usa roles y atributos ARIA solo cuando sea necesario.
  </li>
  <li>
    Asegura contraste de color suficiente.
  </li>
  <li>
    Permite navegación con teclado.
  </li>
  <li>
    Asocia etiquetas <label> a los inputs.
  </li>
</ul>

<h2>SEO Técnico</h2>

<p>
  Objetivo: mejorar la visibilidad en buscadores.
</p>

<ul>
  <li>
    Usa metadatos completos:

```
        <meta name="description" content="Curso completo de desarrollo web con prácticas modernas.">
```
  </li>
</ul>
