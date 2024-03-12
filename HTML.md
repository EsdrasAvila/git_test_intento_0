# HTML
## ELEMENTOS Y ETIQUETAS
Elemento: Contenido dentro de las etiquetas
Etiquetas: Contienen el elemento: Hay dos tipos de apertura y cierre que le dicen al navegador que contenido contiene el elemnto.

\ <p></p>: PARRAFOS DE APERTURA Y CIERRE

### Lista de etiquetas predefinidas
https://developer.mozilla.org/en-US/docs/Web/HTML/Element

### ELEMENTOS VACIOS
Son aquellos que no tienen una etiqueta de cierre:
Ej: \ <br> o <img>
Se les dice asi porque no tienen un contenido provisto en ellos. No se ajusta al contenido como las otras etiquetas.

Tambbien hay etiquetas de cierre automatico
Ej: \ <br/> o <img/> 
Es probable que vea etiquetas de cierre automático que se utilizan con frecuencia por motivos históricos. Los navegadores podrán mostrarlos perfectamente, pero la última versión de la especificación HTML desaconseja su uso y los considera inválidos.

**¿Qué es una etiqueta HTML?**
Es una especie de contenedor, en donde esta el elemento

**¿Cuáles son las tres partes de un elemento HTML?**
Esta compuesto por 3 partes, Apertura, contenido y cierre

## TEXTO REPETITIVO

### Tipo de archivo
**¡Importante:!** _Siempre debemos nombrar el archivo HTML que contendrá la página de inicio de nuestros sitios web index.html. Esto se debe a que los servidores web buscarán de forma predeterminada una index.htmlpágina cuando los usuarios accedan a nuestros sitios web, y no tener una causará grandes problemas._

### Tipo de documento
html tiene diferentes versiones, con la cual le podemos indicar al navegador la version de html que debe usar para representar el documento.
La ultima version de html, es HTML5 y su tipo de documento es DOCTYPE
Y se declara asi: " / <!DOCTYPE html> "
La version anterior es HTML4 y delcara así: / <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">

### elemento html
el elemento hmtl, se declara de la siguiente manera: <html>
y este indica la raiz del documento, es el inicio del documento, lo que significa que todos los demas elelemtos sera decendentes a el.

Dentro de este apartado, tambien se puede apreciar un **"atributo"**, el atributo la, que se encuentra de la siguiente manera: 
`<!DOCTYPE html>`
`<html lang="en"> https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/lang`
 `</html>`

Este atributo indica que tipo de idioma, se esta utilizando en el contenido de la pagina, esto ayuda a mejorar:
 - La accesibilidad a la pagina
 - Permite tegnologias de asistencia

### Elemento principal

<header>, es el lugar en donde se pone la metainformacion (información sobre la información o los datos sobre los datos Normalmente la meta información se utiliza para proporcionar referencias o contextos acerca de los datos) importante y todo lo necesario para que nuestras paginas web se muestre correctamente en el navegador. no debemos utilisar ningun elemnto que muestre contenido en nuestra pagina.

### Metaelemento
El meta elemento es importante ya que con el podremos ver/mostrar los caracteres especiales de los diferentes idiomas en la pagina web.
Este elemento se declara asi: <meta> y va adentro de <header>
Para que pueda agarrar dichos caracteres especiales de todos los idiomas se escribe así: <meta charset="utf-8">  

### Elemento de titulo
EL elemento titulo, es uno de los mas importantes en el documento.
Se declara de la siguiente manera: <title>
ej: <title>My First WebPage</title>

Si no se incluye el elemento en el documento, se quedaria predeterminadamente el nombre del archivo que en este caso es index.html, y eso no tiene mucho significado, para el usuario; esto haría muy difícil encontrar nuestra página web si el usuario tiene muchas pestañas abiertas en el navegador.

De vuelta en nuestro index.htmlarchivo, agreguemos un `<head>` elemento con un `<meta>` elemento y un título dentro de él. El `<head>` elemento va dentro del `<html>` elemento y siempre debe ser el primer elemento debajo de la `<html>` etiqueta de apertura:


`<!DOCTYPE html>`

`<html lang="en">`
  `<head>`
    `<meta charset="UTF-8">`
    `<title>My First Webpage</title>`
  `</head>`
`</html>` 

### Elemeto del cuerpo
Este es necesario, ya que aqui se contendra todo lo que es texto, imagenes, enlaces, videos etc para mostrar al usario.
Ese elemento es el **body**, se declara `<body>` y va dentro de `<html>` y siempre abajo de `<head>`

`<!DOCTYPE html>`

`<html lang="en">`
  `<head>`
    `<meta charset="UTF-8">`
    `<title>My First Webpage</title>`
  `</head>`
  `<body>`
  `<body>`
`</html>` 

### ver archivos
+ Arrastrar el index.html al navegador
+ ir al docuemnto de origen, darle click derecho y buscar el navegador predeterminado
+ Comando en la terminal: Ubuntu- Navegue hasta el directorio que contiene el archivo y escribagoogle-chrome index.html 
Otra forma es:
+ Usar la extension del servidor en vivo con VSCode. (Pero no se recomeinda al principio depender de servidores)

### Acceso directo a VS Code
Para poder crear de manera mas facil el elemento en la primera linea ingrese "!" y presione Enter→, para elegir el primero u estara el texto estandar de HTML, en segundos.

## TRABAJAR CON TEXTO
### como crear parrafos: 
Cuando el navegador encuentre nuevas líneas como esta en su HTML, las comprimirá en un solo espacio. El resultado de esta compresión es que todo el texto se agrupa en una línea larga.

Si queremos crear párrafos en HTML, necesitamos usar el **elemento párrafo** , que agregará una nueva línea después de cada uno de nuestros párrafos. Un elemento de párrafo se define envolviendo el contenido del texto con una `<p>` etiqueta.

### Cómo crear encabezados.
Los titulos se definen igual que los parrafos. pero con un `<h1>`.

h1, es uno de los diferentes tipos de elemento de texto que tenemos, y va desde el `<h1>` hasta el `<h6>`

### Cómo crear texto en negrita.
Para poder marcar/poner un texto en negrita o texto fuerte, usamos la etiqueta `<strong>`, puedes usarlo

solo:

_En codigo:_ "`<strong>` PALABRA FUERTE"

_En la page:_ **PALABRA FUERTE**

O puedes utilizarlo en un conjunto con otros elementos de texto, que seria lo regular:

_En codigo:_ La palabra que no es fuerte `<strong>` DENTRO LA PALABRA FUERTE `</strong>` y fuera las que no son

_En la page:_  La palbra que no es fuerte **DENTRO LA PALBRA FUERTE** y fuera las que no son

### Cómo crear texto en cursiva.
`<em>`, es la etiqueta que se usa para poner en las palabras en cursiva, y utiliza la misma forma de delcaracion que `<strong>`, ya sea sola o con otros elementos de text

### Las relaciones entre elementos anidados y sangria.
Sangria: Introduccion de varios caracteres en blanco(espacio) al comenzar un parrafo.

Al ser la sangria un elemente que se aplica en cualquier elemento dentro de otros elementos, se genera un anidamiento, eso es!, un anidamiento!... 
Cuando anidamos elementos dentro de otro elemento, se crea una relacion padre-hijo entre ellos. El hijo es el anidamiento, y el padre es al cual estan anidados.

EJ. 
`<html>`
  `<head>`
  `</head>`
  `<body>`
  `<p>Lorem ipsum dolor sit amet.</p>`
  `</body>`
 `</html>`

En este caso, el elmento parrafo(hijo), esta anidado al elemento body(padre)
Otro ejemplo de anidamento pero con dos hijos.

EJ.
`<html>`
  `<head>`
  `</head>`
  `<body>`
  `<p>Lorem ipsum dolor sit amet.</p>`
  `<p>Lorem ipsum dolor sit amet.</p>`
  `</body>`
 `</html>`

Los dos parrafos, del anterior codigo, son hermanos, ya que ambos son hijos de la etiqueta body y estan al mismo nivel de anidamiento entre si.

Nota: Utilizamos la sangria en codigo anidado para poder tenr una vision mas clara y legible del codigo, tanto nostros como los desarrolladores que trabajaran con nuestro html en el futuro. 

Recomendacion: Poner dos espacios de sangrado en los elementos secundarios



### Cómo crear comentarios HTML.
Los comentarios son textos no visibles para el usario
se declara de la siguiente manera:
`<!--HOLA MUNDO-->`


Esto no sirve a los clientes que miran la pagina web, si no al que le da un mantemiento, mejora, o crea el codgio.
Esta etiqueta nos ayuda a poner un comentario, recodatorio a nostros y otros desarrolladores.

ATAJO PARA CREAR COMENTARIO: ctrl + /

[ ALgo mas sonre `<strong>` y `<b>` o `<em>` y `<i>` y cuando usarlas ]...(https://medium.com/@zac_heisey/when-to-use-strong-b-em-and-i-tags-in-your-markup-fa4d0af8affb)  

## LISTAS
Para poner listas desordenadas, cuyo orden no importa, como lista de compras.
se puede utilizar el `<ul>` y dentro de este se pone el `<li>`
`<ul>`
  `<li>Item 1</li>`
  `<li>Item 2</li>`
  `<li>Item 3</li>`
`</ul>`

EJ. 
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

Y para listar odenadas, se utilizan dos etiquetas, el elemento `<ol>`,`<li>` que dentro del elmento `<ol>` va el `<li>`

EJ
`<ol>`
  `<li>Item 1</li>`
  `<li>Item 2</li>`
  `<li>Item 3</li>`
`</ol>`

Y esta lista ordenada va enumerada por defecto.

## LLINKS E IMAGENES
### Elementos de anclaje
Para crear un enlace en html, se debe crear un elemento ancla, para eso se define envolviendo el texto u otro elemento hmtl que queremos que se enlace con una `<a>` etiqueta.
EJ. `<a>click me</a>`

#### ATRIBUTO HTML
Brinda informacion a un elemento html y siempre va en la etiqueta de apertura del elemento.

UN atributo esta formado por dos partes: Nombre y valor (pero no todos los atributos requieren un valor).

 **atributo "href"** al poner href seguido de un link, el navegador le pondra un texto color azul y lo subrayara indicando que es un enlace.
en cambio si href no lleva ningun link, este sera un simple texto. Con el no solo puedes vincular links, si no tambien videos, archivos pdf, img, etc.

EJ
`<a href="https://www.theodinproject.com/about">click me</a>`
### Abrir enlaces en una nueva ṕestaña
El método que se muestra arriba abre enlaces en la misma pestaña que la página web que los contiene. 

Atributo target: Mientreas href especifica el enlace de destino, target especifica donde se abrira el recurso vinculado. Si no está presente, de forma predeterminada, tomará el **_self** valor que abre el enlace en la pestaña actual. 

Para abrir la pestaña depende del navegador, puede configurarse con **_blank**

EJ
`<a href="https://www.theodinproject.com/about" target="_blank" rel="noopener noreferrer">click me</a>`

**Atributo rel**
Se utiliza para describir la relacion entre la pagina actual y el documuento vinculado

**noopener** , es el valor que impide que el enlace obtenga acceso a la pagina web desde que se abrio.
el **noferrer** evita que el enlace abierto, sepa que pagina web o recurso tiene enlace o "referencia" hacía el. Tambien incluye el comportamiento de noopener y por lo tanto tambien puede utilizarse por si solo.
noopener evita ataques de phshing(cambian enlaces originales por uno falso, para engañar a los usarios [esto se conoce como tabnabbing]).
Se puede agregar el noferrer valor si no desea que el enlace abierto sepa que su pagina web enlaza con el.

nota: _Tenga en cuenta que puede estar bien si olvida agregar,_ rel="noopener noreferrer" _ya que las versiones más recientes de los navegadores brindan esta seguridad si solo_ target="_blank" _está presente. Sin embargo, de acuerdo con las buenas prácticas de codificación y para pecar de cautelosos, se recomienda siempre emparejar a_ target="_blank"con a rel="noopener noreferrer".

### Vinculos absolutos y relativos.
Por lo regular, se trabajara a menudo con dos tipos de vinculos:

+ Los que nos llevan a paginas web fuera de nuestro directorio o sitio web
- Y los vinculos que nos llevan a una direccion especifica dentro de nuestro sitio web

#### Absolutos:
A los enlaces que te conectan y mandan con una pagina fuera de de tu sitio web de internet se le conoce como absoluto y esta compuesto por la siguientes partes: `protocol://domain/path`, este tipo de enlaces siempre tendra: _un protocolo y tendra el destino de dominio_

En si no es nada mas sencillo que eso.

Lo complicado o lo dificl de recodar es como se pondria en un vinculo con un texto llamativo. Si tu quieres poner un link a una pagina como __avon__, pero no quieres que se vea el link si no el nombre para que el usuario pueda identificarlo de manera facil se utiliza lo siguiente:

` <a href="https://www.Avon.com/about" target="_blank" rel="noopener noreferrer">Avon</a> `

Seria algo similar a esto. como ya sabemos, especificando el destino _(href)_, explicando donde se abrirá el recurso vinculado _(target)_  ya sea en una pestaña nueva _( _blank)_ o de manera predeterminada tomara la pagina actual _( _self)_. con el control de seguiridad _(**noopener:** para que el enlace abierto no obtenga el acceso a la pagina web desde la que se abrio y **noferrer:** valor que impide que el enlace abierto sepa que pagina web o recurso tiene un enlace[o "referencia"] hacia el)_ y ya con las precausiones y protocolos definidos, solo se pone un texto descriptivo o llamativo para el usario _(Avon)_.

Y aun mas sencillo, es un link relativo, que seria el siguiente punto...

#### Relativos:
Los enlaces realtivos, son aquellos que se encuentran dentro de nuestro sitio web, y estos tienen el directiorio en el que se encuentra contenido nuestra pagina. ej `href="fuentes.html" `.

Si por alguna razon se cambio el lugar del archivo, o el archivo esta dentro de otra carpeta. solo se pone el nombre de la o las carpetas antes del archivo. ej ` href="Carpetax/fuentes.html" ` y asi estaria vinculada la pagina.

En muchos casos, esto funcionará bien; sin embargo, aún puedes encontrarte con problemas inesperados con este enfoque. En la mayoría de los casos , anteponerlo _./_ antes del enlace evitará estos problemas. Al agregar, _./_ está especificando en su código que debe comenzar a buscar el _archivo/directorio_ relativo al **_current_ directorio.**

Nota: Current es actual en ingles

#### Metafora

Los vínculos absolutos y relativos son un concepto complicado para construir un buen modelo mental; una metáfora puede ayudar:

Piense en su nombre de dominio `( town.com)` como una ciudad, el directorio en el que se encuentra su sitio web `( /museum)` como un museo y cada página de su sitio web como una sala del museo `( /museum/movie_room.html` y `/museum/shops/coffee_shop.html)`. Los enlaces relativos como `./shops/coffee_shop.html` son direcciones desde la sala actual (la sala de cine del museo `/museum/movie_room.html`) a otra sala (la tienda del museo). Los enlaces absolutos, por otro lado, son direcciones completas que incluyen el protocolo `( https)`, el nombre de dominio `( town.com)` y la ruta desde ese nombre de dominio ( `/museum/shops/coffee_shop.html `): `https://town.com/museum/shops/coffee_shop.html.`

### Imagenes
Sencillamente podemos al igual que como se coloca un link `<a "href"></a>`, podemos poner una imagen con `<img>` pero este no tiene un cierre, la etiqueta se cierra sola. Dentro de esta se pondra el atributo `_scr_` el cual incrusta la imagen en la pagina, indicandole al navegador en donde se ubica la imagen, ya sea dentro de la web o dentro de nuestra computadora.

Lo interesante de aqui es que podemos poner un vinculo de una imagen en internet:

Ej: ` <img src="https://www.theodinproject.com/mstile-310x310.png">`

O Simplemente descargando la img o pasando a la computadora una foto del recurso que se quiere mostrar. Una vez echo eso, se pone la ruta de la imgen de la siguiente manera:

Ej:  `<img src="./images/dog.jpg">`

Y depende mucho de la ruta, si esta en la misma carpeta que tu archivo .html pues solo de pone algo asi `<img src="Imagen.jpg">`, pero si eres organizado(que es lo mejor que podrias hacer) y tienes una carpeta llamada _"proyecto"_ y dentro de ella esta el archivo index.html y una carpeta llamada _"img"_ en donde se conetien las imagenes, seria algo asi: `<img src="./img/imagen.jpg">` (el `./` como se dijo anteriormente: Es para prevenir poblemas de direccion. el `./` esta especificando en tu codigo que debe comenzar a buscar el archivo/directorio relativo al current directorio) 


__nota:__
_Los formatos de imagen principales que se utilizan en la web(todos diseñados para hacer diferentes cosas) son:_
__JOG GIF PNG SVG__

ENLACE PARA SABER MAS SOBRE LOS TIPOS DE FORMATOS: https://internetingishard.netlify.app/html-and-css/links-and-images/#image-formats

### Directorios principales
Ah! ok, creo que entendi, si es como lo estoy pensando
Tu tienes una carpeta llamada _"the odin"_ y luego tienes otras dos carpetas dentro de estas, una se llama _"imagenes"_ y la otra _"acerca de"_ algo asi:

Carpeta: 1.`the odin` Archivos contenidos: `index.html`
Carpeta: 1.2`acerca de` Archivos contenidos: `about.html`
Carpeta: 1.3`img` Archivos contenidos: `imagen.jpg`

_"the odin"_ es el directorio principal, y si tu quieres utilizar la _imagen.jpg_ de _"img"_ en _about.htlm_. primero tendriamos que un nivel desde el directorio de paginas a su directorio principal para luego poder acceder al directorio de _"img"_ 

Para ir al directorio se uyilizan dos puntos en la ruta del archivo relativa como esta: `../`, ser veria de la sigente manera:
`<img src="../images/dog.jpg">`

Graficamente es esto:
De la `Carpeta: 1.2` sale el codigo de __"about"__ a la *carpeta principal* `Carpeta: 1` y luego entra a la `Carpeta: 1.3` en donde esta contenido __"imagen.jpg"__

### Atributo alternativo
__"alt"__ es un atributo que se utiliza para describir una imagen, es importante, siempre que tengas una imagen, es bueno agregar un texto descriptivo, para personas con problemas de la vista o tambien se utilizara en lugar de la img, en casi de que no se pueda cargar.

En codigo se podria ver asi:
`<img src="https://www.theodinproject.com/mstile-310x310.png" alt="The Odin Project Logo">`

### Atibutos de tamaño de img
Lo importantemente llamativo de una pagina web son sus imagenes y que seriamos sin esos pequeños agregados que nos dan la capacidad de tener una imagen en optimas condiciones, sin probocar que parpade ni salte de paginas.

Simplemente es una buena practica espesificar estos atributos en cad imagen, aun cuando el tamaño es correcto o se pueda modificar con css.

el codigo se veria de la siguiente manera:
 `<img src="https://www.theodinproject.com/mstile-310x310.png" alt="The Odin Project Logo" height="310" width="310">`

y asi se veria la imgen 


<img src="https://www.theodinproject.com/mstile-310x310.png" alt="The Odin Project Logo" height="310" width="310">

Conclusion: 
Elemento `<img>`, atributo `src=""`

## 