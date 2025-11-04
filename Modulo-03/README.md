<img width="1280" height="250" alt="portadas" src="https://github.com/user-attachments/assets/76e6fbc3-02f2-44e0-8261-451ebe5b4666" />

<h2>Accesibilidad en HTML</h2>

<p>
  La accesibilidad web consiste en garantizar que las personas con discapacidades visuales, auditivas, físicas, del habla, cognitivas 
  o neurológicas puedan utilizar la web de manera efectiva. Incluir accesibilidad en el desarrollo web también mejora la experiencia 
  para todos los usuarios, haciendo los sitios más intuitivos y fáciles de usar.
</p>

<h3>Importancia de la accesibilidad web</h3>
<ul>
  <li>
    <h3>Inclusión</h3>
    <p>
      Permite que cualquier persona pueda navegar y usar tu sitio.
    </p>
  </li>
  <li>
    <h3>SEO</h3>
    <p>
      Muchos de los principios de accesibilidad mejoran también el posicionamiento en motores de búsqueda.
    </p>
  </li>
  <li>
    <h3>Legal</h3>
    <p>
      En algunos países, la accesibilidad es un requisito legal (ej. ADA en Estados Unidos).
    </p>
  </li>
</ul>

<h3>Elementos fundamentales de la accesibilidad en HTML</h3>

<ol>
  <li>
    <h3>Uso de etiquetas semanticas.</h3>
    <p>
      Como vimos anteriormente, las etiquetas semanticas describen claramente el contenido de un sitio web, lo que ayuda a 
      los navegadores, lectores de pantalla y motores de búsqueda a comprender mejor la estructura de una página.
    </p>

```html

    <header>
      <h1>Título principal del sitio</h1>
      <nav>
        <ul>
          <li><a href="#">Inicio</a></li>
          <li><a href="#">Acerca de</a></li>
        </ul>
      </nav>
    </header>
    
    <main>
      <section>
        <h2>Sección importante</h2>
        <p>Este es el contenido principal.</p>
      </section>
    </main>
    <footer>
      <p>&copy; 2024 Mi Sitio Web</p>
    </footer>
```

  </li>
  <li>
    <h3>Texto alternativo en imagenes (alt)</h3>
    <p>
      Las imágenes deben tener texto alternativo que describa su contenido o función. Esto es esencial para los lectores de 
      pantalla utilizados por personas con discapacidad visual.
    </p>

```html

    <img src="imagen.jpg" alt="Descripción de la imagen">

```

  </li>
  <li>
    <h3>Enlaces descriptivos</h3>
    <p>
      Los textos de los enlaces deben ser claros y describir a dónde llevan. Evita textos como "Haz clic aquí" o "Más información".
    </p>

```html

    <a href="contacto.html">Contáctanos</a>

```
    
  </li>
  <li>
    <h3>Uso correcto de los encabezados (respetar su jerarquia)</h3>
    <p>
      La jerarquía de encabezados (h1, h2, h3, etc.) ayuda a estructurar el contenido y permite a los usuarios de lectores de 
      pantalla navegar fácilmente por la página. No olvides que se permite solo un encabezado H1 por pagina.
    </p>

```html

    <h1>Título principal</h1>
    <h2>Subtítulo o tema relacionado</h2>

```

  </li>
  <li>
    <h3>Formularios accesibles</h3>
    <p>
      Asegúrate de que los formularios estén correctamente etiquetados, utilizando la etiqueta label asociada a cada campo de formulario.
    </p>

```html

    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre">

```

  </li>
   <li>
    <h3>Vídeos y subtítulos</h3>
    <p>
      Los vídeos deben incluir subtítulos y, si es posible, transcripciones para que sean accesibles para personas 
      con discapacidad auditiva.
    </p>

```html

    <video controls>
      <source src="video.mp4" type="video/mp4">
      <track kind="subtitles" src="subtitulos.vtt" srclang="es" label="Español">
    </video>


```

  </li>
  <li>
    <h3>Contraste de color</h3>
    <p>
      Asegúrate de que haya suficiente contraste entre el texto y el fondo para que sea legible por personas con baja visión. 
      Vamos a profundizar mas este tema en el curso de CSS.
    </p>
  </li>
  <li>
    <h3>Uso del atributo ARIA (Accessible Rich Internet Applications)</h3>
    <p>
      mejora la accesibilidad de componentes interactivos. Existen varios roles y atributos ARIA que proporcionan más 
      información a los lectores de pantalla. A continuación vamos a verlos...
    </p>
  </li>
</ol>
