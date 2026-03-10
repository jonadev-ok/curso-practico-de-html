<img width="1280" height="250" alt="portadas (3)" src="https://github.com/user-attachments/assets/259e34b6-8c15-4862-9108-f8f949779826" />

# Optimización, Rendimiento y Buenas Prácticas en HTML

En esta sección vamos a repasar, reforzar y profundizar conceptos ya vistos a lo largo del curso, y ver algunos otros que, van a dar  
mayor rendimiento al desarrollo de sus proyectos en HTML.

## Estructura y Semántica Correcta

Objetivo: mejorar la accesibilidad, el SEO y la mantenibilidad.

  - Usa etiquetas semánticas: 
    <a href="https://github.com/jonadev-ok/curso-practico-de-html/blob/main/Curso/Modulo-02/README.md">
      consultar aqui
    </a>
  - Evita usar divs innecesarios.
  - Usa encabezados jerarquicos de forma logica.

## Optimización de carga

Objetivo: mejorar la velocidad percibida y real de carga de la página.

  - Minimiza el HTML (usa herramientas como HTMLMinifier o el proceso de build del framework).
  - Evita comentarios innecesarios en producción.
  - Usa lazy loading para imágenes y recursos:

    
```html
<img src="imagen.jpg" loading="lazy" alt="Descripción" />

```

    
  - Coloca los scripts al final del body o usa defer:


 ```html
 <script src="app.js" defer></script>

```   

## Optimización de Imágenes</h2>

Objetivo: reducir el peso sin perder calidad.
  - Usa formatos modernos (.webp, .avif).
  - Adapta el tamaño según el dispositivo (srcset y sizes):
    
```html

<img src="img.jpg"
srcset="img-400.jpg 400w, img-800.jpg 800w"
sizes="(max-width: 600px) 400px, 800px"
alt="Ejemplo optimizado">

```

  - Comprime las imágenes.
  - Elimina metadatos EXIF innecesarios.

## Accesibilidad Web (a11y)

Objetivo: permitir que todas las personas puedan navegar correctamente.

  - Siempre usar alt en imágenes.
  - Usa roles y atributos ARIA solo cuando sea necesario.
  - Asegura contraste de color suficiente.
  - Permite navegación con teclado.
  - Asocia etiquetas <label> a los inputs.

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
  <li>
    Usa un <title> descriptivo por página.
  </li>
  <li>
    URLs limpias y semánticas
  </li>
  <li>
    Añade datos estructurados (schema.org) si es necesario.
  </li>
</ul>

<h2>Código Limpio y Mantenible</h2>

<p>
  Objetivo: facilitar lectura, colaboración y escalabilidad.
</p>

<ul>
  <li>
    Mantén indentación consistente (2 o 4 espacios).
  </li>
  <li>
    Usa comentarios claros donde agreguen valor.
  </li>
  <li>
    Evita style="" y onclick="" en línea.
  </li>
  <li>
    Nombra las clases de forma coherente (usa BEM si podés).
  </li>
</ul>

<h2>Compatibilidad y Buen Rendimiento</h2>

<p>
  Objetivo: garantizar compatibilidad entre navegadores.
</p>

<ul>
  <li>
    Usa el DOCTYPE correcto:
    
```
<!DOCTYPE html>
```
  </li>
  <li>
    Define el charset:
    
```
<meta charset="UTF-8">
```
  </li>
  <li>
    Viewport responsivo:
    
```
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
  </li>
  <li>
    Prueba el sitio con Lighthouse o PageSpeed Insights.
  </li>
</ul>

<h2>Microoptimizaciones Avanzadas</h2>

<p>
  Para proyectos grandes o de alta performance
</p>

<ul>
  <li>
    Viewport responsivo:
    
```
<link rel="preload" href="styles.css" as="style">
<link rel="prefetch" href="next-page.html">
```
  </li>
  <li>
    Ordena y agrupa los recursos CSS/JS según prioridad.
  </li>
  <li>
    Implementa Service Workers para cachear contenido estático.
  </li>
</ul>
