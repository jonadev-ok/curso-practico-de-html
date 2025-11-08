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
