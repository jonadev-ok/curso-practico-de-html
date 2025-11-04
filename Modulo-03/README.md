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

<h2>Etiquetas de contenido multimedia</h2>

<ol>
  <li>
    <h3>Etiqueta de imagen</h3>
    <p>
      Es una etiqueta simple y se utiliza para mostrar imágenes que complementan el contenido textual. Mejora la experiencia visual 
      y puede ser parte clave del contenido. Se utiliza el atributo src para especificar la URL de la imagen.
    </p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <img src="logo.png" alt="Logo de JonaDev" width="200" height="100">
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de video</h3>
    <p>
      Esta etiqueta se utiliza para incrustar archivos de video que se pueden reproducir directamente en el navegador, con controles 
      de reproducción como pausa y volumen.  Se utiliza el atributo src para especificar la URL del video, el atributo controls 
      para mostrar controles de reproducción, como el botón de play, barra de progreso, etc, el atributo poster para mostrar una 
      imagen antes de que comience la reproducción y otros atributos que veremos mas adelante.
    </p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <video src="video.mp4" controls width="600" poster="imagen-inicial.png">
      Tu navegador no soporta el elemento de video.
    </video>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiquetas de audio</h3>
    <p>
      Similar a la anterior. Se utiliza para agregar clips de audio, como música o efectos de sonido, con controles de reproducción. 
      Los atributos son casi los mismos que los de la etiqueta de video.
    </p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <audio src="audio.mp3" controls>
      Tu navegador no soporta el elemento de audio.
    </audio>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiquetas de subtítulos y pistas de texto en videos</h3>
    <p>
      La etiqueta track añade una pista de texto (subtítulos, transcripciones o descripciones) a los videos. Se usa dentro de 
      la etiqueta video para proporcionar subtítulos o descripciones alternativas. Se utilizan los atributos kind, para definir el 
      tipo de pista (por ejemplo, subtitles, captions, descriptions), el src para especificar la URL de la pista de subtítulos y 
      srclang para especificar el idioma de la pista de texto.
    </p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <video controls>
      <source src="video.mp4" type="video/mp4">
      <track src="subtitulos.vtt" kind="subtitles" srclang="es" label="Español">
    </video>
  </body>
</html>
```

  </li>
</ol>

