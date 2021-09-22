# estructura

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
</head>
<body>
</body>
</html>
```

`<!DOCTYPE html>` para que el navegador interprete el codigo como html5.
`<html>` etiqueta raiz de todo elemento html.
`<head>` aqui se agregan caracteristicas que no neceseriamente va a ser visibles para el usuario.
`<title>` indica cual sera el titulo de la pagina web.
`<body>` aqui se encontrara el contenido de la pagina web.

# etiquetas

```html
<body>
    <h1>Mi primer heading</h1>
    <p>parrafo</p>
    <hr>
    <!-- comentario -->
    <p>
        Este texto es <span>mucho mas largo</span> y es para <br>
        la etiqueta span!
    </p>
    <a href="https://www.google.com">Ir a google</a>
    <a target="_blank" href="https://www.google.com">Ir a google</a>
    <img src="https://www.rutaalaimagen.com/img.png" />
    <img src="coffe.png" />
    <img src="img/coffe.png" width="400" height="600" />
</body>
```

`<h1></h1>`-`<h6></h6>` titulos.
`<p></p>` parrafos.
`<hr>` separacion.
`<!-- -->` comentarios.
`<span></span>` para identificar un texto o una etiqueta dentro de otra y asi
poder referenciarlas o agregarles estilo
`<br>` salto de linea.
`<a href="https://www.google.com"></a>` link.
`<a target="_blank" href="https://www.google.com">Ir a google</a>` abre el link en otra pestanna.
`<img src="https://www.rutaalaimagen.com/img.png" />` agregar una imagen desde la web.
`<img src="coffe.png" />` agregra una imagen local.
`<img src="img/coffe.png" width="400" height="600" />` modifica dimensiones

# formularios

```html
<body>
    <form action="/formulario" method="POST">
        <label for="nombre">Nombre</label>
        <input value="chanchito" type="text" id="nombre" name="nombre" placeholder="Nombre" />
        <label for="comentario">Comentario</label>
        <textarea rows="10" cols="50" id="comentario" placeholder="ingrese comentario" name="comentario">este es un valor por defecto</textarea>
        <input type="submit" />
    </form>
</body>
```

`<form action="/formulario" method="POST">` formulario.
`action="/formulario"` ruta a la que se envian los datos.
`method="GET"`
`method="POST"` metodo con el que se envian los datos.
GET envia los datos en la url.
POST no envia los datos en la url.
(POST no es mas seguro)
(lo seguro seria utilizar certificados que se encarguen de encriptar todas nuestras conexiones)
`<label for="nombre">Nombre</label>` etiqueta.
`for="nombre"` para identificar a que input pertenece y que al hacer click se
habilite el mismo.
`<input value="makz" type="text" id="nombre" name="nombre" placeholder="Nombre" />` campo de texto.
`value="makz"` valor por defecto de un input text.
`id="nombre"` identificador del campo de texto.
`name="nombre"` key: nombre value: texto en el input
`placeholder="Nombre"` para indicar al usuario que va en el campo de texto.
`type="text"` para indicarle al navegador el comportamiento del input.
`type="text"` texto.
`type="submit"` boton.
`type="email"` email.
`type="password"` contrasenna.
`type="radio"` radio.
`type="checkbox"` checkbox.
`type="file"` archivos.
`<textarea rows="10" cols="50" id="comentario" placeholder="ingrese comentario" name="comentario""></textarea>`
`rows="10"` indica la cantidad de filas del textarea.
`cols="50"` indica la cantidad de columnas del textarea.
`<input type="submit" />` en cuando se presione tomara todos los valores y los enviara al servidor.

# botones

```html
<body>
    <button type="button">Enviar</button>
</body>
```

`<button type="button"></button>` boton se configura su comportamiento con js.
`<button type="reset"></button>` al presionarlo se resetean los valores del form.
`<button type="submit"></button>` envia el formulario.
(los botones pueden contener otras etiquetas)

# listas

```html
<body>
    <ul>
        <li>Elemento 1</li>
        <li>Elemento 2</li>
        <li>Elemento 3</li>
        <li>Elemento 4</li>
    </ul>
    <ol>
        <li>Elemento 1</li>
        <li>Elemento 2</li>
        <li>Elemento 3</li>
        <li>Elemento 4</li>
    </ol>
    <ol value="50">
        <li>Elemento 50</li>
        <li>Elemento 51</li>
        <li>Elemento 52</li>
        <li>Elemento 53</li>
    </ol>
    <ol>
        <li>Elemento 1</li>
        <li>Elemento 2</li>
        <li>Elemento 3</li>
        <li>
            <ol>
                <li>sub elemento 1</li>
                <li>sub elemento 2</li>
                <li>sub elemento 3</li>
            </ol>
        </li>
    </ol>
</body>
```

`<ul></ul>` lista no ordenada.
`<li></li>` item de la lista.
`<ul></ul>` lista ordenada.
`<ol value="50">` para que empiece a contar desde 50.

# tablas

```html
<body>
    <table>
        <thead>
            <tr>
                <th>Producto</th>
                <th>Precio</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Hola beats</td>
                <td>Gratis</td>
            </tr>
            <tr>
                <td>chanchito feliz</td>
                <td>19,90$</td>
            </tr>
            <tr>
                <td>chanchito feliz muy feliz</td>
                <td>29,90$</td>
            </tr>
        </tbody>
        <tfoot>
            <td>total</td>
            <td>49.80$</td>
        </tfoot>
    </table>
</body>
```

`<table></table>` tabla.
`<tr></tr>` fila.
`<th></th>` header.
`<td></td>` data.
`<thead></thead>` para agrupar headers.
`<tbody></tbody>` para agrupar filas que no contengan headers.
`<tfoot></tfoot>` para el footer.

# mas etiquetas

```html
<body>
    <!-- header: se usa para agrupar links, alguna imagen o logo de la pagina
    y se pueden crear tantas como queramos.
    excepciones:
    - no se puede crear una etiqueta header dentro de otra etiqueta header
    - no se puede crear una etiqueta header dentro de un footer -->
    <header>
        <h1>Blog de chanchito feliz</h1>
    </header>
     <!-- sirve para definir secciones dentro de la aplicacion. -->
     <section>
         <!-- article: para definir contenido independiente. en este caso los
         post del blog -->
         <article>
             <h2>Titulo de mi post</h2>
             <p>Descripcion de mi post</p>
             <img src="img/coffee.png" width="400" />
             <p>Texto del articulo que hay aca y es texto de prueba
             chanchito feliz</p>
         </article>
         <article>
             <h2>Titulo de mi post 2</h2>
             <p>Descripcion de mi post 2</p>
             <img src="img/monster.png" width="400" />                                             p
             <p>Texto del articulo que hay aca y es texto de prueba
             chanchito feliz</p>
         </article>
         <article>
             <h2>Titulo de mi post 3</h2>
             <p>Descripcion de mi post 3</p>
             <img src="img/guitarra.png" width="400" />
             <p>Texto del articulo que hay aca y es texto de prueba
             chanchito feliz</p>
         </article>
     </section>
     <!-- footer: se usa para indicar el pie de pagina. esta puede contener
     el copyright, info de contacto, links, autor -->
     <footer>
         <a href="mailto:micorreo@gmail.com">micorreo@gmail.com</a>
         <p>Copyright 2021</p>
     </footer>
 </body>
```

`href="mailto:micorreo@gmail.com"></a>` abre el cliente de correo en la seccion
de redactar correo con el correo de destino listo.

# divs

```html
<body>
    <div>
        <p>esto es un parrafo dentro de un div</p>
    </div>
</body>
```

`<div></div>` cumple la misma funcion de section. se usa para dividir el contenido
y para agrupar secciones.

# atributos id y class

identificador unico o generico para interactuar con las etiquetas mediante js o
para asignarle un estilo de css.

```html
    <h1 id="titulo"></h1>
    <article class="post"></article>
```

`id="titulo"` identificador unico.
`class="post"` identificador generico.

# links ++

```html
<body>
    <a href="#titulo">Ir al comienzo</a>
</body>
```
`<a href="#titulo">Ir al comienzo</a>` hace scroll hasta donde esta definida
una etiqueta con el id titulo.
