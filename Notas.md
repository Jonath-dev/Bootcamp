# The Web Developer Bootcamp 2022

## HTML

### Skeleton
```
<!DOCTYPE html>     
<html lang="en">
<head>: Contiene todos los metadatos de nuestra pagina.      
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>: Define el titulo de nuestro documento.
</head>
<body>: Representa todo el contenido del documento.
    <b></b>
</body>
</html>
```

### Elementos
* p: Representa un parrafo.
* i: Letra cursiva.
* b: letra negrita.
* h1-h6: Encabezados se rigen por jerarquia del 1 al 6. 
* hr: Representa un cambio de tema.
* br: Produce un salto de línea en el texto.
* sup: Agrega un super indice.
* sub: Agrega un sub indice.

### Elementos semanticos
* main: Representa el contenido principal del documento.
* nav: Se usa para brindar navegacion en el documento.
* section: Representa una seccion independiente.
* article: Representa una composición auto-contenida en un documento
* aside: parte del documento que se relaciona solo indirectamente con resto. 
* Header: Encabezados, contenido introductorio. 
* Footer: Pie de página para el contenido de sección
* figure: Contenido independiente, a menudo con un título.
```
<main>
    <section>
        <h3>Ofertas especiales</h3>
    </section>
    <article>
        <H2>Mejores productos 2022</H2>
    </article>
    <aside>
        <nav>
            <ul>
                <li>Atributos</li>
                <li>Ejemplos</li>
            </ul>
        </nav>
    </aside>
</main>
```

#### Inline
Los elementos inline utilizan solo es espacio necesario por lo cual comparten es espacio con los demas elementos inline hasta agotarse. 
* Span
#### Block
Los elementos de bloque utilizan todo el bloque incluso si el espacio esta vacio.
* Div

### Listas
La sintaxis para las listas es la misma:
* ul: Listas desordenadas.
* ol: Listas ordenadas.  
```
<ul>
    <li>Rojo</li>
    <ul>
        <li>Carmesi</li>
        <li>Cherry</li>
    </ul>
    <li>Azul</li>
    <li>Verde</li>
</ul>

```
Las listas pueden anidar otras listas.

### Ancla (link)

```
<a href="https://www.google.com/">Google</a>
<a href="Us.html">Sobre nosotros</a>
```
#### Atributos
href: Directorio, archivo o direccion al que envia el ancla.

### Imagenes
```
<img src="https://www.rd.com/wp-content/uploads/2021/01/GettyImages-1175550351.jpg" alt="Gato negro">
<img src="img/blackcat.jpg" alt="Gato negro">
```
#### Atributos
* src: Directorio o link de la imagen.
* alt: Texto alternativo en caso de no poder acceder a la imagen.

### Comentarios
```
    <!--  -->
```
ctrl+/: Crea automaticamente una linea de comentario.
shift+alt+a: Crea un bloque de comentarios.

### Divs & Span
#### Divs
Sirve para crear secciones o agrupar contenidos.Es un elemento de bloque.

#### Span
Sirve para aplicar estilo al texto o agrupar elementos en línea.

```
<div style="color: blue;">
 <h2> Ejemplo de div y span </h2>
  <p>
    Esto es un párrafo dentro de un div,
    <span style="color: red;"> y esto un span dentro de un párrafo.</span>
  </p>
</div>

```

### Entities

Son codigos especiales que se usan para caracteres reservados en html. Todos espiezan con & y terminan con un punto y coma.
```
&lt; = <
```