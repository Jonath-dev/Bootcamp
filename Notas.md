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
```
<p>: Representa un parrafo.
<i>: Letra cursiva.
<b>: letra negrita.
<h1>- <h6>: Encabezados se rigen por jerarquia del 1 al 6. 
```

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
