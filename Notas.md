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

<img src="https://www.rd.com/wp-content/uploads/2021/01/GettyImages-1175550351.jpg" alt="Gato negro">

```
<img src="https://www.rd.com/wp-content/uploads/2021/01/GettyImages-1175550351.jpg" alt="Gato negro">
<img src="img/border-box.png" alt="Gato negro">
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

## CSS

### Color and background-color
El atributo color puede ser ingresado con diferentes sistemas como son: 
* RGB (0,0,0);
* Hex #000;
* Name black;

### Text properties

1. Text-aling: Establece la posicion del texto.
```
p{
    text-aling: (Left/start, Right/end, Center, Justify);
}
```

2. Font-weight: Especifica el peso o grueso de la letra.

* Normal/bold: Letra normal o en negritas. (400)/700)
* Lighter/bolder: Mas delgada o gruesa con respecto al padre.
* 100-900: Depende del valor numerico que se le de.

```
/* Poner texto del párrafo en negrita. */
p {
  font-weight: (Normal/bold, Lighter/bolder, 100-900);
}
```

3. Text decoration: Se usa para establecer el formato de texto a subrayado (underline) y suprarrayado (overline), tachado (line-through) o parpadeo (blink).
```
/* Valores clave */
text-decoration: none;                 /* Sin decoración */
text-decoration: underline red;        /* Subrayado rojo */
text-decoration: underline wavy red;   /* Subrayado rojo linea ondulada */
```
4. Line-height: Establece la altura de una caja de línea. Se utiliza comúnmente para establecer la distancia entre líneas de texto.
```
p{
    line-height: (normal,3.5, 3em,34%);
}
```

5. Letter-spacing: Establece el espaciado horizontal entre caracteres de texto.
```
h1{
    letter-spacing: (normal,3.5, 3em,34%);
}
```

6. Font-size: Propiedad que establece el tamaño de la fuente.
```
a{
    Font-size: (small,medium,large,x-large,12px, 3em,34%);
}
```
7. Font-family: Establece la fuente de nuestro texto. Puedes agregar fuentes de respaldo en caso de no ser posible desplegar la determinada, esto se hace agregando la fuente de respaldo despues de la principal separandolas con una coma.

```
p{
    font-famuly: Arial narrow, Serif;
}
```

### Selectors

1. Universal selector: Selecciona todo en el documente, puede ser poco eficiente.
```
*{
    color:pink;
}
```

2. Element selector: Selecciona un todos los elementos de un tipo. Podemos anidar elementos con una coma.

```
    button{
        font-size: 20pc;
    }
    h1,h2{
        color:pink;
    }
```

3. Id selector: Selecciona un elemento por su Id unico. la sintaxis para esto es un # seguido del Id.

```
#login-b{
    text-decoration:none;
}
```

4. Class selector: Selecciona todos los elementos de una clase, sin importar el tipo.

```
HTML 
    <input type="text" name="name" id="name" class="tag">
CSS
    .tag{
        Color:pink;
    }

```

5. Descendant selectors: Selecciona elementos que se encuentren anidados en ciertos elementos.
```
HTML
    <div>
        <p>
            <img>
        </p>
    </div>
CSS
    div a img{
        width:250px;
    }
```
En este ejemplo el selecctor busca las imagenes que se encuentren dentro de un enlace dentro de un div y le dara es estilo definido. 

6. Adjacent selector: Este selector es utilizado para modificar elementos que esten justo despues de otro elemento.
```
HTML
    <label for="name">Ingrese nu nombre:</label>
    <input type="text" name="name" id="name">
CSS
    label + input{
        background-color:pink;
    }
```
En este ejemplo se selecciona el input ya que esta inmediatamente despues del label como especificamos.

7. Direct Descendant: Selecciona todos los elementos un nivel inferios al nivel especificado.
```
HTML
    <form action="">
        <div>
            <label for="name">Ingrese nu nombre:</label>
            <input type="text" name="name" id="name" required>
            <button>Comprobar</button>
        </div>
        <button>Register now</button> 
    </form>        
CSS
    form > button{
        Background-color:pink;
    }
```
En este ejemplo el boton dentro del div no toma es estilo deseado por que se encuentra dos niveles abajo del form(Form > Div > button),pero el boton que se encuentra despues del div si, ya que esta solo un nivel abajo (Form > button).

8. Attribute selector: Empareja elementos en función de la presencia o el valor de un atributo determinado.
```
input[type="password"]{
    color: pink;
} 
```
Selecciona todos los input de tipo contraseña.

### Pseudo classes 

Una Pseudoclase es una palabra clave añadida a un selector que especifica un estado especial del elemento o elementos seleccionados. 

1. :hover: Coincide cuando el usuario interactúa con un elemento con el mouse.
```
    .login button:hover{
        background-color: burlywood;
        color: darkgreen;
    }
```
2. :active - Coincide con el momento en que el usuario activa un elemento. Por ejemplo, cuando se hace clic en el.
3. :check - Representa cualquier elemento de radio, casilla de verificación u opción que esté marcado o activado.
4. :focus -  representa un elemento que ha recibido foco.
5. nth-of-type(3n): empareja elementos basándose en su posición entre hermanos del mismo tipo.
Suponiendo que haya 10 elementos del mismo tipo, esta funcion seleccionaria a los elementos 3,6 y 9. 
Nota: si no se le agrega la "n", solo seleccionaria al tercer elemento.


### Pseudo elementos
Es una palabra clave que permite aplicar estilo a una parte específica del elemento seleccionado

1. ::first-letter
2. ::first-line
3. ::selection

4. ::after - Suele utilizarse para añadir contenido cosmético al final de un elemento con la propiedad content.
```
    .dead-link::after {
        content: url('../../media/warning.svg');
        display: inline-block;
        width: 12px;
        height: 12px;
    }
```
El codigo anterior coloca un icono al final del link caido.

5. ::before - Suele utilizarse para añadir contenido cosmético al principio de un elemento con la propiedad content. Su sintaxis es igual a la de after.

### Box model

#### Width and Height
Establece el ancho y la altura respectivamente del contenido principal.
```
    p{
        width: 200px;
        height: 200px;
    }
```
El codigo anterior restringe las dimenciones de nuestro contenido para formar un cuadrado de 200px.

#### Border properties 

1. Width: Controla el espesor del borde.
2. Color: Cambia el color del borde.
3. Style: Cambia el estilo (solid, wavy, dashed,).
4. Box-sizing: border-box; - Si el elemento tiene algun borde, este es entonces añadido al ancho y alto, entonces se ajusta al tamaño establecido. 
![border-box](/img/border-box.png)

5. border-left-():Esta funcion especifica el borde al que quieres cambiarle el estilo.
6. border-radius: Redondea las esquinas de nuestros bordes, puede ser usado en diferentes elementos, como las imagenes por ejemplo. Tambien podemos especificar el borde y la medida del redondeo.
![padding](/img/padding.png)

#### Pading and Margin
Padding : Este elemento establece la distancia entre el contenido principal y el borde. Hay diferentes formas de configurarse.

Margin: Establece el área de margen en los cuatro lados de un elemento.
Comparte sintaxis con el padding.
![padding](/img/padding.png)

### Display 

1. Inline: Se ignora el ancho y el largo, los elementos son empujados de manera horizontal
2. Block: Se respeta el ancho, largo, margen y padding, ocupa todo el espacio horizontal de su elemento.
3. Inline-block: Se comporta como un elemento de linea pero su margen, padding, ancho y largo se respetan.

### Unidades relativas

% : Dependiendo del elemento en el que se use varia su resultado, algunos elementos como el section, calculan este valor compadado con el de su padre.
EMs: Tamaño de fuente del padre, en el caso de propiedades tipográficas como font-size, y tamaño de fuente del propio elemento, en el caso de otras propiedades como anchura.
Varia dependiendo del padre.
```
HTML
    <section>
        <button>
            Register
        </button>
    </section>
CSS
    section {
        font-size: 30px;
    }
    button{
        background-color: blanchedalmond;
        color: darkblue;
        border-radius: .5 em;
    }
```
En este caso el radio del borde sera de 15px, ya que el padre usa una fuente de 30px.

Rems:Tamaño de fuente del elemento raíz y este valor no cambiara, es mas facil de usar a comparacion de los ems.