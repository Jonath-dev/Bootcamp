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

### Tables
* Table: Sintaxis para iniciar una tabla.
* th (Table head): Ingresa los titulos de nuestra tabla.
* tr (Table row): Indica una fila en la tabla.
* td (Table data): Celda de la tabla, dentro ingresa el contenido a mostrar.
* thead: Indica los headers de la tabla.
* tbody: Indica el contenido de la tabla.
* tfoot: Indica el footer de la tabla.

```
<Table>
        <thead>
            <tr>
                <th>Name</th>
                <th>Flighted </th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Ostrich</td>
                <td>No</td>
            </tr>
            <tr>
                <td>Somali ostrich</td>
                <td>No</td>
            </tr>
        </tbody>
    </Table>
```
#### Atributos
* colspan: Modifica el espacio que ocupa esta columna.
    * colspan=2: Signidica que utilizara dos cuadros de nuestra tabla en esa columna
* rowspan: Modifica el espacio que ocupa esta fila.
    * rowspan=2: Signidica que utilizara dos cuadros de nuestra tabla en esa fila

### Forms
Form: Contenedor con controles interactivos para enviar info.  
* Action: Especifica a donde sera enviada nuestra info.
* Method: Especifica que metodo HTTP sera usado.

Input:
* TYPES: Cada tipo es para un proposito en especifico.
* button: Boton sin comportamiento predeterminado.
* checkbox: Un check box que permite un solo valor a seleccionar
* color: Abre un selector de color.
* date: Control para ingresar año, mes y dia.
* email: Valida que el texto ingresado sea un email.
* file: Abre el selector de archivos.
* hidden
* image: Un boton de submit que muestra una img.
* month: Selecciona un mes.
* number: Ingresa solo valores.
* password: Caracteres ocultos. 
* radio: Permite una sola eleccion de los diferentes radios con el mismo nombre.
* range: Ingresa un valor entre un parametro.
* reset: Limpia el form.
* search: Ingresa una busqueda.
* tel: Valida que se un numero de telefono.
* url: Valida que sea un url.
* submit: Envia los datos del form.

Placeholder: Atributo que indica el contenido predeterminado.

Labels: Etiquetas, pueden ser vinculadas con un imput ingresando en el atributo "for", el id del input.
```
<form action="">
    <label for="username">Ingresa un nombre de usuario</label>
    <input id="username" type="text" placeholder="Nombre de usuario">
</form>
```
### Name attribute
Puede ser utilizado para referencias un elemento en javascript.

### Radiobuttons, checkboxs and select

Checksboxs: Se utilizan para permitir al usuario seleccionar una o más opciones de un número limitado de opciones.

Radiobuttons: Se utilizan para permitir al usuario seleccionar solo una opcion de un número limitado.

Select: Se utiliza para crear una lista desplegable.

NOTAS:
Para agregar las diferentes opciones todas deben contener el mismo valor en el atributo name.
Id: Se utiliza para vincular una etiqueta con las etiquetas.
Value: Es la informacion que sera enviada al enviar el formulario.

```
<form action="">
    <p>
        Selecciona tu color preferido:
        <input type="radio" name="fcol" id="fred" value="red">
        <label for="fred">Red</label>
        <input type="radio" name="fcol" id="fblue" value="blue">       
        <label for="fblue">Blue</label>
        <input type="radio" name="fcol" id="fgreen" value="green">
        <label for="fgreen">Green</label>
    </p>
    <p>
        <label for="fmasc">Selecciona tu mascota preferida</label>
            <select name="fmasc" id="mascota">
                <option value="Gatos">Gatos</option>
                <option value="Perros">Perros</option>
                <option value="Aves">Aves</option>
                <option value="Otro">Otro</option>
            </select>
    </p>
    <p>
        <input type="checkbox" id="terms" name="agree">
        <label for="terms">I am agree</label>
    </p>
</form>
```
### Range and Text area
Range: Define un control para introducir un número entre dos valores.

Text area: Define un control de entrada de texto multilínea.

```
    <p> 
        <label for="brillo">Selecciona el nivel de brillo</label>
        <input type="range" id="brillo" name="brightness_lvl" min="0" max="100" step="10">
    </p>        
    <p>
        <label for="comments"> Desea agregar un comentarios </label>
        <br> 
        <textarea name="comments" id="comments" cols="30" rows="10" placeholder="Comments"></textarea>
    </p>
```

### Validation

Atributo required: Los inputs con este atributo son nesesarios para poder enviar el form.

(min-max)lenght: Este atributo indica el minimo o maximo numero de caracteres de una entrada.
