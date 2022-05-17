# Introducción a HTML

1. [Estructura base de HTML](#Estructura-base-de-HTML)
2. [Atributos](#Atributos)
3. [Encabezados](#Encabezados)
4. [Tipos de Texto](#Tipos-de-Texto)
5. [Listas](#Listas)
6. [Tablas](#Tablas)
7. [Enlaces](#Enlaces)


---
## Estructura base de HTML 

- `<!DOCTYPE html>` define que este documento es un documento HTML5
- `<html>`elemento raíz de una página HTML.
- `<head>` contiene metainformación sobre la página HTML.
- `<title>` especifica un título para la página HTML
- `<body>` define el cuerpo del documento 
- `<h1>` define un encabezado grande
- `<p>` define un párrafo.

~~~html
<!DOCTYPE html>
<html>
    <head>
        <title>Mi sitio web</title>
    </head>
    <body>

        <h1>Hola Mundo</h1>
        <p>Mi primer párrafo</p>

    </body>
</html>
~~~

---
## Atributos
Los elementos de HTML  pueden tener atributos que nos permite describir información sobre los elementos. 
- Los atributos deben estar escritos en la etiqueta de apertura. 
- Los atributos tienen nombre y valor.
- El valor de un atributo va después de signo `=` entre comillas. 

~~~html
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8">
        <title>Mi sitio web</title>
    </head>
    <body>
        <h1>Hola Mundo</h1>
        <p>Mi primer párrafo</p>
    
</html>
~~~

---

## Encabezados 
Los elementos de encabezado implementan seis niveles de encabezado del documento, `<h1>` es el más importante, y `<h6>`, el menos importante. 

~~~html

<!-- Eeste es un comentario -->
<!-- Encabezados en HTML -->

<h1>Hola Mundo</h1>
<p>Mi primer párrafo</p>

<h2>Encabezado level 2</h2>
<h3>Encabezado level 3</h3>
<h4>Encabezado level 4</h4>
<h5>Encabezado level 5</h5>
<h6>Encabezado level 6</h6>

~~~

---

## Tipos de Texto

- `<p></p>` Contenedor de párrafo 
- `<hr>` Genera una linea horizontal 
- `<br>` Genera un sato a la siguiente linea 
- `<pre></pre>` Contenedor de texto preformateado
- `<b></b>` Texto en negrita 
- `<strong></strong>` Texto en negrita importante 
- `<i></i>` Texto en cursiva 
- `<em></em>` Texto en cursiva importante
- `<u></u>` Texto subrayado 
- `<small></small>` Texto pequeño
- `<code></code>` Para código

~~~html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <title>Mi sitio web</title>
</head>

<body>
    
    <h1>Hola Mundo</h1>
    <p>
        Lorem ..., <br> conse...adip<br>Ma... <br>
        impedit...odio.
    </p>
    <hr>

    <h2>Texto preformateado</h2>
    <pre>
        Lorem ... odio.
    </pre>

    <hr>
    <h2>Tipos de Texto</h2>
    <p>
        Texto en <b>negrita</b> <br>
        Texto en <strong>negrita importante</strong> <br>
        Texto en <i>cursiva</i> <br>
        Texto en <em>cursiva importante</em> <br>
        Texto <u>subrayado</u> <br>
        Texto <small>pequeño</small> <br>
        Texto en <code>código</code>
    </p>

</body>

</html>
~~~

---
## Listas 
### Listas Desordenadas  

La etiqueta `<ul></ul>` crea un lista no ordenada. Esta definido como elemento para listas. 
- Puede contener uno o mas elementos `<li></li>`. 

~~~html
<h2>Lista de Tipos de Texto</h2>
<h3>Listas Desordenadas</h3>
    <ul>
        <li>Textos en gritas</li>
        <ul>
            <li>Texto en <b>negrita</b></li>
            <li>Texto en <strong>negrita importante</strong></li>
        </ul>
        <li>Textos en cursivas</li>
        <ul>
            <li>Texto en <i>cursiva</i></li>
            <li>Texto en <em>cursiva importante</em></li>
        </ul>
        <li>Otros</li>
        <ul>
            <li>Texto <u>subrayado</u></li>
            <li>Texto <small>pequeño</small></li>
            <li>Texto en <code>código</code></li>
        </ul>      
    </ul>

~~~
### Listas Ordenadas
La etiqueta `<ul></ul>` crea un lista no ordenada. Esta definido como elemento para listas. 
- Puede contener uno o mas elementos `<li></li>`.
- `type`: Este atributo puede contener el tipo de valor que va enumerar. 
- `start`: Este atributo pude contener desde que valor inicia la enumeración. 
~~~html
<h3>Listas Ordenadas</h3>
    <ol>
        <li>Textos en gritas
            <ol type="I">
                <li>Texto en <b>negrita</b></li>
                <li>Texto en <strong>negrita importante</strong></li>
            </ol>
        </li>
        
        <li>Textos en cursivas
            <ol type="A">
                <li>Texto en <i>cursiva</i></li>
                <li>Texto en <em>cursiva importante</em></li>
            </ol>
        </li>
        
        <li>Otros
            <ol type="1" start="100">
                <li>Texto <u>subrayado</u></li>
                <li>Texto <small>pequeño</small></li>
                <li>Texto en <code>código</code></li>
            </ol>
        </li>    
    </ol>    
    
~~~

### Listas de descripción
- `<dl>` para definir una lista de descripción
- `<dt>` para definir el término de descripción
- `<dd>` para describir el término en una lista de descripción

~~~html
    <h3>Listas de descripción</h3>
    <dl>
        <dt>Café</dt>
        <dd>El café esta caliente</dd>
        <dt>Leche</dt>
        <dd>La leche esta tibia</dd>
    </dl>
~~~
---
## Tablas 
Las tablas HTML permiten a los desarrolladores web organizar los datos en filas y columnas.
- `table`: Para definir una tabla. 
- `colspan`: Para hacer que una celda abarque varias columnas.
- `rowspan`: Para hacer que una celda abarque varias filas.
~~~html
<h2>Tabla de Usuarios</h2>

    <table border="1">
        <tr>
            <th>N#</th>
            <th>Nombres</th>
            <th>Correo</th>
            <th>Telefono</th>
        </tr>
        <tr>
            <td>1</td>
            <td>Alex</td>
            <td>alex@gmail.com</td>
            <td>910456123</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Roel</td>
            <td>roel@gmail.com</td>
            <td>950456789</td>
        </tr>
    </table>
~~~
---
## Enlaces
El elemento `<a></a>` es un enlace. Una ancla puede convertir el texto que encierra en un hipervínculo. Las anclas pueden tener varios atributos, pero varios son como sigue:

- `href`: El valor de este atributo indica la dirección web a la que se quiere que apunte el enlace.
- `target`:  El atributo target especifica el contexto de navegación que va a usar para mostrar el enlace. 
    - `_self` Defecto. Abre el documento en la misma ventana.
    - `_blank` Abre el documento en una nueva ventana o pestaña
    - `_parent` Abre el documento en el marco principal
    - `_top` Abre el documento en el cuerpo completo de la ventana.
- `title`: Añade información adicional sobre el enlace, como puede ser el título de la página que vinculas. 


~~~html
<a href="https://www.google.com/" title="Buscador Google" target="_blank">Ir a Google</a>
<a href="https://www.roelcode.com/" title="Curso de Programación" >Ir a ROELCODE</a>
<a href="other.html" >Otra Página</a>
~~~
