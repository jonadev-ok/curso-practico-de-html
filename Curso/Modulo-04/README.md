<img width="1280" height="250" alt="portadas (2)" src="https://github.com/user-attachments/assets/303e8005-bbb1-4c93-a69e-c7ed5efc7c54" />

<h2>Introducción al SEO (Search Engine Optimization)</h2>

<p>
  El objetivo principal del SEO es, hacer que una web sea facilmente entendible tanto para los motores de busqueda como para los 
  usuarios. Esto permite mejorar su posicionamiento en los resultados de búsqueda. Un SEO bien implementado favorece la llegada de 
  tráfico orgánico al sitio, es decir, sin necesidad de recurrir a anuncios pagados.<br> El SEO se divide en 3 categorias. 
  Veremos cada una a continuación.
</p>

<ol>
  <li>
    <h3>SEO On-Page</h3>
    <p>Optimización dentro del contenido y el código HTML de la página.</p>
  </li>
  <li>
    <h3>SEO Off-Page</h3>
    <p>Factores externos como enlaces entrantes o backlinks.</p>
  </li>
  <li>
    <h3>SEO Técnico</h3>
    <p>Relacionado con la arquitectura del sitio y la indexabilidad.</p>
  </li>
</ol>

<h3>Elementos de HTML que afectan el SEO</h3>

<ol>
  <li>
    <h3> Etiquetas de título.</h3>
    <p>
      La etiqueta title es uno de los factores más importantes para el SEO. Es el título de la página 
      que aparece en la pestaña del navegador y es también el primer texto que los motores de búsqueda ven.
    </p>
    <ul>
      <li>
        <p>
          Longitud recomendada: Entre 50 y 60 caracteres.
        </p>
      </li>
      <li>
        <p>
          Incluye palabras clave relevantes: Asegúrate de que el título 
          contenga las palabras clave principales, pero de manera natural.
        </p>
      </li>
    </ul>
      
```html
    <title>Guía completa de SEO en HTML | Curso de HTML</title>
```
      
  </li>
  <li>
    <h3> Meta descripción.</h3>
    <p>
      La meta descripción es un breve resumen de la página que aparece debajo del título en los resultados de búsqueda. 
      Aunque no afecta directamente al ranking, una buena descripción puede mejorar la tasa de clics (CTR).
    </p>
    <ul>
      <li>
        <p>
          Longitud recomendada: Entre 150 y 160 caracteres.
        </p>
      </li>
      <li>
        <p>
          Debe ser descriptiva y contener palabras clave.
        </p>
      </li>
    </ul>
      
```html
    <meta name="description" content="Aprende SEO para mejorar el ranking de tu sitio web en los motores de búsqueda con esta guía completa de HTML.">

```
      
  </li>
  <li>
    <h3>Encabezados.</h3>
    <p>
      Los encabezados estructuran el contenido de la página, facilitando tanto la lectura para los usuarios como la 
      comprensión para los motores de búsqueda. Los encabezados deben seguir una jerarquía lógica.
    </p>
    <ul>
      <li>
        <p>
          h1: Debe contener el título principal de la página, y solo debe haber uno por página.
        </p>
      </li>
      <li>
        <p>
         h2, h3: Se usan para subtítulos y organizar el contenido.
        </p>
      </li>
    </ul>
      
```html
    <h1>Guía de SEO para HTML</h1>
    <h2>¿Qué es SEO?</h2>
    <h3>Importancia de SEO On-Page</h3>


```
      
  </li>
  <li>
    <h3>URLs amigables (SEO-friendly URLs).</h3>
    <p>
      Las URLs deben ser claras, descriptivas y contener palabras clave relevantes. 
      Evita las URLs largas y con parámetros complicados.
    </p>
    <ul>
      <li>
        <p>
          Usa guiones (-) para separar palabras.
        </p>
      </li>
      <li>
        <p>
         Mantén las URLs cortas y descriptivas.
        </p>
      </li>
    </ul>
      
```html
    https://www.ejemplo.com/curso-seo-html-basico

```
      
  </li>
  <li>
    <h3>Atributo alt en imágenes.</h3>
    <p>
      El atributo alt proporciona una descripción de las imágenes, 
      lo que es útil para los motores de búsqueda y también para la accesibilidad. 
      Al incluir palabras clave relevantes en el alt, puedes mejorar el SEO de la página.
    </p>
      
```html
    <img src="seo.jpg" alt="Guía completa de SEO en HTML">

```
      
  </li>
  <li>
    <h3>Enlaces internos.</h3>
    <p>
      Conectan páginas dentro del mismo sitio web. 
      Ayudan a los motores de búsqueda a descubrir más contenido en tu sitio.
    </p>
      
```html
    <a href="/guia-seo">Guía completa de SEO</a>

```

  </li>
  <li>
    <h3>Enlaces externos.</h3>
    <p>
      Enlaces a sitios web externos relevantes y de alta calidad. Estos enlaces pueden mejorar tu autoridad si son confiables.
    </p>
      
```html
    <a href="https://www.google.com/webmasters/">Google Search Central</a>

```

  </li>
  <li>
    <h3>Atributo rel en enlaces (rel="nofollow", rel="noopener").</h3>
    <p>
      El atributo rel le dice a los motores de búsqueda cómo tratar los enlaces. 
      Por ejemplo, rel="nofollow" indica que no se debe transferir "autoridad" (link juice) al sitio vinculado.
    </p>
    <ul>
      <li>
        <p>
          rel="nofollow": Úsalo para enlaces pagados o patrocinados.
        </p>
      </li>
    </ul>
    
```html
    <a href="https://www.sitio.com" rel="nofollow">Enlace patrocinado</a>

```

  <ul>
    <li>
      <p>
        rel="noopener" y rel="noreferrer": Son buenas prácticas de seguridad cuando se usan 
        enlaces que abren en nuevas pestañas (target="_blank").
      </p>
    </li>
  </ul>

```html
    <a href="https://www.sitio-seguro.com" target="_blank" rel="noopener noreferrer">Abrir en nueva pestaña</a>

```
                
  </li>  
  <li>
    <h3>Sitemap.</h3>
    <p>
      Un sitemap es un archivo XML que enumera todas las páginas de tu sitio y ayuda a los motores de búsqueda a indexarlas. 
      Aunque no es directamente parte del HTML, es fundamental para el SEO técnico.
    </p>
      
```xml
    <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
      <loc>https://www.ejemplo.com/</loc>
      <lastmod>2024-10-05</lastmod>
      <priority>1.00</priority>
   </url>
   <url>
      <loc>https://www.ejemplo.com/curso-seo</loc>
      <lastmod>2024-10-01</lastmod>
      <priority>0.80</priority>
   </url>
</urlset>

```
      
  </li>
  <li>
    <h3>Robots.txt</h3>
    <p>
      El archivo robots.txt le indica a los motores de búsqueda qué páginas de tu sitio pueden o no pueden ser indexadas.
    </p>
      
```txt
    User-agent: *
    Disallow: /admin/
    Allow: /


```
      
  </li>
  <li>
    <h3>Rich Snippets (Microdatos y Schema.org)</h3>
    <p>
      Los Rich Snippets son fragmentos enriquecidos que se muestran en los resultados de búsqueda, 
      proporcionando información adicional (como valoraciones, recetas, eventos, etc.).
      El marcado de Schema.org es el más común y proporciona una manera de estructurar 
      los datos de tu página para que los motores de búsqueda puedan mostrar información adicional.
    </p>
      
```html
    <div itemscope itemtype="http://schema.org/Product">
      <span itemprop="name">Camiseta SEO</span>
      <span itemprop="priceCurrency" content="USD">$</span><span itemprop="price">19.99</span>
      <img src="camiseta.jpg" alt="Camiseta SEO" itemprop="image">
      <meta itemprop="productID" content="12345">
    </div>

```
      
  </li>
  <li>
    <h3>Buenas prácticas adicionales de SEO</h3>
    <ul>
      <li>Palabras clave (Keyword Research): Investiga qué palabras clave son relevantes 
        para tu contenido y utilízalas de manera natural en los títulos, meta descripciones, y contenido.
      </li>
      <li>
        Contenido original y de calidad: El contenido debe ser único, relevante y proporcionar valor. Evita el contenido duplicado.
      </li>
      <li>
        Indexabilidad: Asegúrate de que todas las páginas importantes de tu sitio sean indexables 
        por los motores de búsqueda. Utiliza robots.txt y meta noindex para evitar la indexación de páginas irrelevantes.
      </li>
      <li>
        Mobile First: Asegúrate de que tu sitio sea responsive. Los motores de búsqueda como Google 
        priorizan sitios optimizados para dispositivos móviles.
      </li>
    </ul>
      
  </li>
</ol>
