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
