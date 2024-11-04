# Selectores 

1. Vincular hojas de estilo HTML con CSS usando el atributo: link rel="stylesheet" href="estilo.css" type="text/css" media="screen, print"

2. Selectores
    Etiquetas (Ejemplo: h1 {color:blue})
    Clases (Ejemplo: < h1 class="roja")
    Identificadores (Ejemplo: < p id="rojo")

3. Agrupamiento
    h1, p, h3 {font-family:arial}
    
    Identificadores y clases sería: 
    #cabecera, #piepagina {color:#00FF00} .cabecera, h2, #micolor {color:#FF0000}

4. Anidamiento selector anidado común
    h1 span a {color:red; font-weight: bold}

    Anidamiento de selectores hijos
    h1>a {color:red}

5. Selectores adyacentes
    h5 + p {font-weight: bold}

6.  SELECTORES CON PSEUDOCLASES 
    a:link, span:hover
    SELECTORES CON PSEUDO-ELEMENTOS
    p.clase::first-line

7. Variables 
    :root {--main-bg-color: coral;--main-padding: 15px; } 

# Buena práctica al escribir CSS

/* hay que poner comentarios con esta sintaxis (son multilínea) */ 

Los selectores se nombran en minúsculas, nunca empezando por caracteres especiales o numéricos. 

El nombre de los selectores debe ser específico y claro, para que tenga una mayor capacidad expresiva. 

El nombre de los identificadores no debe describir una característica visual, como color, tamaño o posición. 

Los nombres deben seguir más una visión semántica que estructural. Para facilitar los cambios. 

Separa las palabras mediante guiones (_ o-) o mayúsculas. Lo más común hoy en día es emplear guiones (-) y minúsculas. Por ejemplo, las clases con nombre “letra-negrita”, “seccionprincipal”, etc. 

No hacer uso excesivo de clases. En muchas ocasiones se puede organizar el código de forma más eficiente con agrupamientos o adyacencia.

# Unidades de medida

Absolutas: 


Pulgadas (In). Una Pulgada = 2,54 Cm.

Centímetros (Cm). Milímetros (Mm). 

Puntos (Pt). Un Punto = 1/72 De Pulgada. 

Picas (pc). Una pica = 12 puntos. 

Píxeles (px) 


Relativas:


em(relativo al font-size del elemento en el que se usa) 

rem (relativo al font-size del elemento raíz de la página, es decir < html >) 

% es relativo al tamaño del elemento raíz donde está situada la etiqueta. 

vw y vh. Respectivamente, el ancho y alto del viewport (área de visualización) 

vmin y vmax. El ancho máximo o mínimo del área de visualización dependiendo de la orientación (se verá con más detalle adelante).

# Atributos de Fuentes

Formato RGB
Formato RGBA
Formato hexadecimal

font-size: unidades \ xx-small \ x-small \ small \ médium \ large \ x-large \ xx-large. Sirve para determinar el tamaño de una fuente. Ejemplo: span.clase {font-size: 16px} 

font-weight: normal \ bold \ bolder \ lighter \ 100 \ 200 \ 300 \ 400 \ 500 \ 600 \ 700 \ 800 \ 900. Sirve para definir la anchura de los caracteres, es decir, efecto de negrita. Normal y 400 son el mismo valor, así como bold y 700. 

font-style: normal \ italic \ oblique. Es el estilo de la fuente. El estilo obligue es similar al italic (ambos cursiva).

font-family: serif \ sans-serif \ cursive \ fantasy \ monospace.

@ font-face

text-decoration: none \ underline \ overline \ line-through. 

text-align: left \ right \ center \justify. Sirve para indicar la alineación del texto. 

text-shadow: Efecto de sombra. Los parámetros son: sombra horizontal, sombra vertical, borrosidad, color.

text-indent: Unidades. 

line-height

# Atributos de Fondo

Background-color: RGB, RGBA o nombre de color. 

background-image:url('smiley.gif’)

background-repeat

background-position

background-origin

background-clip

background-size

background-blend-mode

background-attachment

# Atributos de Tablas

caption-side: valores top \ bottom.

table-layout: auto \ fixed

border-collapse: collapse \ separate

border-spacing: horizontal vertical.

empty-cells: show \ hide.

vertical-align: top \ bottom \ middle

# Atributos de Visibilidad

Overflow: visible \ hidden \ scroll \ auto

Display: inline \ block \ contents \ flex \ grid \ inline-block \ inline-flex \ inline-grid \ inline-table \ list-item \ run-in \ table \ table-caption \ table-column-group \ table-header-group \ table-footer-group \ tablerow-group \ table-cell \ table-column \ table-row

Visibility: visible \ hidden

# Atributos de Listas

list-style-type: disc \ circle \ square \ decimal \ decimal-leadingzero \ lower-roman \ upper-roman \ lower-greek \ lower-latin \ upperlatin \ armenian \ georgian \ lower-alpha \ upper-alpha \ none

list-style-image: url("../jpg") \ none

list-style-position: inside \ outside

# Atributos de Modelo de Cajas

margin-left , margin-right , margin-top , maring-bottom

border-left , border-right , border-top , border-bottom

padding-left , padding-right , padding-top , padding-bottom

# Atributos Border

Border-width: thick (ancho), medium(medio), thin(estrecho)

Border-style: none, dotted (punteado), dashed (discontinua), solid (línea sólida), doublé (doble linea), groove (ranura), ridge (cresta), inset (recuadro) y outset. 

Border-color: Cualquier color válido en RGB, hexadecimal o con palabras reservadas.

border-radius

border-image

box-shadow

# ATRIBUTOS DEL CONTENIDO Y DIMENSIONES

width, height, max-width, max-height, min-width y min-height

max-content, min-content, fit-content

calc

# Maquetación con Capas 

Capa 1: Es la capa principal y contenedora 

Capa 2: Capa dentro de la capa contenedora 1 y alineada a la izquierda (float: left;) 

Capa 3: Igual que la capa 2, pero a la derecha y con un margen (float: right; margin: 10px).

# Atributos de Posicion

position: static

position: absolute

position: relative

position: fixed

position: sticky

    top 
    bottom 
    left 
    right

Ejemplo: a.caja { 
            position:absolute; 
            top:50px; 
            left:50px; 
            background-color:red; 
            }

# FLOTAR Y POSICIONAR

Float: none, left, right

Clear: left, right, both, none

# Centrar Elementos

La solución correcta para centrar verticalmente una página web se basa en el posicionamiento absoluto e implica realizar un cálculo matemático sencillo. A continuación se muestra el esquema gráfico de los cuatro pasos necesarios para centrar una página web en la ventana del navegador: 
#contenedor { 
    width: 500px; 
    height: 500px; 
    position: absolute; 
    top: 50%; 
    left: 50%; 
    margin-top: -250px; /* height/2 = 500px / 2 */ 
    margin-left: -250px; /* width/2 = 500px / 2 */ 
    }

# PRECEDENCIA DE ESTILOS

< style> 
    p{background: crimson;} /* Especificidad de 1 puntos */ 
    .parrafo{background: pink;} /*Especificidad de 10 puntos*/ 
    p.parrafo{background: brown;} /*Especificidad de 11 puntos*/ 
    #id-parrafo{background: orange;}/*Especificidad de 100 puntos*/ 
    p#id-parrafo{background: red;}/*Especificidad de 101 puntos*/ 
    p.parrafo#id-parrafo{background:green;}/*Especificidad de 111 puntos*/ 
    < /style> 

!important (Por ejemplo: p{color: blue !important})