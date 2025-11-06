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

<h2>Formularios avanzados.</h2>

<p>
  Los formularios son una de las interacciones más comunes en la web. En este punto, vamos a ver cómo crear formularios más 
  completos y accesibles.
</p>

<h3>Etiquetas y Atributos Avanzados para formularios.</h3>

<ol>
  <li>
    <h3>input (tipos avanzados)</h3>
    <p>Introducción a tipos avanzados de input</p>
    <ul>
      <li>type="email": Valida automáticamente que el usuario ingrese un formato de email válido.</li>
      <li>type="password": proporcionan una forma para que el usuario ingrese una contraseña de forma segura.</li>
      <li>type="url": Asegura que la entrada sea una URL.</li>
      <li>
        type="number": Solo permite ingresar números y puede tener atributos como min, max y step para especificar rangos y 
        valores aceptables.
      </li>
      <li>type="date" y type="datetime-local": Permiten seleccionar fechas y tiempos con un selector gráfico.</li>
      <li>type="range": Crea un control de rango deslizante, ideal para selecciones numéricas rápidas.</li>
    </ul>
    <br><br>
    
```html

    <label for="email">Correo Electrónico:</label>
    <input type="email" id="email" name="email" >
    
    <label for="date">Fecha de nacimiento:</label>
    <input type="date" id="date" name="date">

    <label for="range">Ingrese una contraseña:</label>
    <input type="password">

    <input type="submit" value="Enviar">

```
    
  <li>
    <h3>Nuevos Controles de Formularios</h3>
    <ul>
      <li>datalist: Crea una lista de sugerencias predefinidas para un campo de texto, útil para autocompletar.</li>
      <li>output: Usado para mostrar el resultado de un cálculo o una operación dinámica en un formulario.</li>
    </ul>
    
```html

    <label for="ciudad">Ciudad:</label>
    <input list="ciudades" id="ciudad" name="ciudad">
    <datalist id="ciudades">
      <option value="Buenos Aires">
      <option value="Córdoba">
      <option value="Rosario">
    </datalist>

    <form oninput="resultado.value=parseInt(a.value)+parseInt(b.value)">
      <input type="number" id="a" name="a">
        +
      <input type="number" id="b" name="b">
        =
      <output name="resultado" for="a b">0</output>
    </form>


```

  </li> 
  <li>
    <h3>Atributos de validación y constricciones.</h3>
    <ul>
      <li>required: Hace que un campo sea obligatorio.</li>
      <li>pattern: Permite definir un patrón de expresión regular para validar el campo.</li>
    </ul>

```html

    <input type="text" id="username" name="username" pattern="[a-zA-Z0-9]+" required>

```

  </li>
</ol>

<p>
  Utilizando atributos como required, minlength, maxlength, pattern, entre otros. Estos permiten verificar los datos del formulario 
  antes de ser enviados al servidor, mejorando la experiencia de usuario.
</p>

<h3>Roles ARIA (roles de accesibilidad).</h3>
<p>
  Los roles ARIA definen el propósito o comportamiento de un elemento 
  HTML para los usuarios que dependen de tecnologías de asistencia.
</p>

<h3>Roles de estructura de documento</h3>
<ol>
  <li>
    <h4>role="banner":</h4>
    <p>
      Se usa para identificar la cabecera principal de un documento o aplicación.
      Normalmente se asigna a header.
    </p>
  </li>
  <li>
    <h4>role="navigation":</h4>
    <p>
      Define una barra de navegación, ayudando a los usuarios a identificar secciones de navegación.
      Usualmente asignado a nav.
    </p>
  </li>
  <li>
    <h4>role="main":</h4>
    <p>
      Indica el contenido principal de la página, excluyendo elementos repetitivos como la barra lateral o el encabezado.
      Se usa en main.
    </p>
  </li>
  <li>
    <h4>role="complementary":</h4>
    <p>
      Define contenido complementario, como barras laterales, que respalda el contenido principal.
      Se suele asignar a aside.
    </p>
  </li>
  <li>
    <h4>role="contentinfo":</h4>
    <p>
      Define el pie de página de un documento o aplicación, que generalmente contiene información sobre el autor, derechos de autor, etc.
      Se asigna al footer.
    </p>
  </li>
  <li>
    <h4>role="article":</h4>
    <p>
      Define contenido que es autónomo y puede ser distribuido de forma independiente.
      Se usa en article.
    </p>
  </li>
  <li>
    <h4>role="region":</h4>
    <p>
      Se usa para definir una sección importante del contenido de la página, que normalmente lleva un encabezado visible.
      Se puede usar en section.
    </p>
  </li>
</ol>

<h3>Roles de widgets y componentes interactivos</h3>
<ol>
  <li>
    <h4>role="button":</h4>
    <p>
      Indica que un elemento tiene un comportamiento similar a un botón.
      Se usa en cualquier elemento que actúe como un botón, como un div o span, si no se usa el elemento button.
    </p>
  </li>
  <li>
    <h4>role="checkbox":</h4>
    <p>
      Define un campo de verificación que puede estar marcado o no.
      Usado en inputs o en otros elementos personalizados que simulan un checkbox.
    </p>
  </li>
  <li>
    <h4>role="dialog":</h4>
    <p>
      Define una ventana emergente (popup) que captura el foco del usuario.
      Se usa en modales.
    </p>
  </li>
  <li>
    <h4>role="alertdialog":</h4>
    <p>
      Similar a dialog, pero implica un mensaje urgente que requiere la atención inmediata del usuario.
    </p>
  </li>
  <li>
    <h4>role="progressbar":</h4>
    <p>
      Representa una barra de progreso que indica el estado de una operación en curso.
      Se usa en elementos como progress.
    </p>
  </li>
  <li>
    <h4>role="slider":</h4>
    <p>
      Define un control que permite seleccionar un valor dentro de un rango.
      Se usa en elementos como barras de rango o sliders personalizados.
    </p>
  </li>
  <li>
    <h4>role="menu":</h4>
    <p>
      Define un menú de navegación o contexto, como el menú de opciones de un botón derecho.
      Usado en menús desplegables.
    </p>
  </li>
  <li>
    <h4>role="menuitem":</h4>
    <p>
      Define un ítem dentro de un menú, como una opción de lista.
      Se usa dentro de roles de menú.
    </p>
  </li>
  <li>
    <h4>role="tab":</h4>
    <p>
      Define una pestaña dentro de un componente de pestañas (tab panel).
      Usado en interfaces de tabulación.
    </p>
  </li>
  <li>
    <h4>role="tabpanel":</h4>
    <p>
      Define el contenido asociado a una pestaña (tab).
      Usado en interfaces de pestañas.
    </p>
  </li>
  <li>
    <h4>role="textbox":</h4>
    <p>
      Define un campo de entrada de texto.
      Usado en elementos personalizados que no son un input o textarea pero se comportan como uno.
    </p>
  </li>
</ol>

<h3>Roles de estado y propiedades</h3>
<ol>
  <li>
    <h4>role="alert":</h4>
    <p>
      Se usa para anunciar mensajes importantes que no requieren interacción.
      Estos mensajes deben ser leídos automáticamente por el lector de pantalla.
    </p>
  </li>
  <li>
    <h4>role="status":</h4>
    <p>
      Define un área que proporciona actualizaciones de estado dinámicas sobre la página.
      Diferente a alert, ya que no interrumpe al usuario.
    </p>
  </li>
  <li>
    <h4>role="tooltip":</h4>
    <p>
      Indica una caja de información flotante que aparece cuando el usuario pasa el ratón sobre un elemento.
    </p>
  </li>
</ol>

<h3>Atributos ARIA.</h3>
<p>
  Los atributos ARIA complementan los roles, proporcionando más detalles sobre el estado, propiedades y relaciones de los elementos.
</p>

<h3>Atributos de estado y propiedades</h3>

<ol>
  <li>
    <h4>aria-hidden="true":</h4>
    <p>
      Indica que un elemento debe ser ignorado por las tecnologías de asistencia. Se usa cuando el contenido es 
      irrelevante para los lectores de pantalla.
    </p>
  </li>
  <li>
    <h4>aria-disabled="true":</h4>
    <p>
      Indica que un elemento está deshabilitado y no puede ser interactuado.
    </p>
  </li>
  <li>
    <h4>aria-expanded="true/false":</h4>
    <p>
      Indica si un elemento desplegable (como un menú o acordeón) está expandido (true) o colapsado (false).
    </p>
  </li>
  <li>
    <h4>aria-checked="true/false/mixed":</h4>
    <p>
      Indica el estado de un control de selección, como un checkbox (true para marcado, false para no marcado, 
      y mixed para un estado indeterminado).
    </p>
  </li>
  <li>
    <h4>aria-selected="true/false":</h4>
    <p>
      Indica si un elemento, como una opción de lista, está seleccionado.
    </p>
  </li>
  <li>
    <h4>aria-label="Texto":</h4>
    <p>
      Define una etiqueta personalizada para un elemento que puede no tener texto visible, 
      útil para botones de íconos o elementos gráficos.
    </p>
  </li>
  <li>
    <h4>aria-labelledby="ID":</h4>
    <p>
      Asocia el elemento con un ID de otro elemento que actúa como su etiqueta. Similar a label en formularios, 
      pero permite etiquetas más complejas.
    </p>
  </li>
  <li>
    <h4>aria-describedby="ID":</h4>
    <p>
      Asocia un elemento con un ID de otro elemento que proporciona una descripción adicional, útil para proporcionar 
      más contexto sobre el uso o estado de un control.
    </p>
  </li>
  <li>
    <h4>aria-controls="ID":</h4>
    <p>
      Indica que el elemento controla otro elemento (por ejemplo, un botón que controla la visibilidad de un panel desplegable).
    </p>
  </li>
  <li>
    <h4>aria-live="polite/assertive":</h4>
    <p>
      Define el nivel de prioridad para que los lectores de pantalla anuncien cambios en el contenido dinámico.
      <br>polite: No interrumpir al usuario, esperar hasta que termine su acción.
      <br>assertive: Interrumpir inmediatamente para anunciar el cambio.
    </p>
  </li>
  <li>
    <h4>aria-role="tablist":</h4>
    <p>
      Indica un contenedor de pestañas (tab) que gestiona la interacción entre pestañas y paneles de contenido.
    </p>
  </li>
  <li>
    <h4>aria-busy="true/false":</h4>
    <p>
      Indica que el elemento está cargando o está ocupado. Cuando true, las tecnologías de asistencia 
      informarán al usuario que el elemento aún está ocupado y no debe interactuar con él.
    </p>
  </li>
</ol>
