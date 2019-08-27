
## HTTP Protocol

### Commands
`host`
comando host resuelve un nombre a dirección IP

> para usar el comando host hay que instalar dnsutils en linux.

Cada aplicación utiliza un puerto: Los puertos son a nivel de software.
```html
$ host www.u-cursos.cl
www.u-cursos.cl has address 200.9.100.67
```
``nmap``: Ver un "mapa de  "<br>
``traceroute``: Ver más o menos que recorrido han seguido los paquetes
 de internet
``curl``: Hace peticiones http, y le puedo indicar que datos enviar
``ab``: esta pensado en hacer test de estress.
### Programas Útiles
> kibanna
> httpclient
> nmap
> ElasticSearch
Rellenar los datos de una dashboard con
Elasticsearch:
kibana:
Cualquier servicio que atiende clientes deje registro.

Scaneo de puertos: con telnet

### Servicios en los distintos puertos
*tcp:** transfer control protocol
**udp:** datagramas sin control
**ftp:**
**puerto 80:** http
**443:** https
hasta el 1024 hay que accerder con permisos de super usuario.
**smt**
**telnet**
Puedo instalar diferente software, que va a hacer uso de cada puerto.


la respuesta que recibe el cliente, al interectuar via web, usualmente viene en html.
**La tarea 1:** son varios archivos en la Tarea1.
HTML, CSS y JavaScript.


# HTML
> lenguaje de etiquetado, que le indica al cliente como está esctructurada la información.
Es bueno imaginar el html como un arbol

los tag `meta` sirven para añadir información invisible, como por ejemplo las categorías de información que utiliza mi página (like hashtags)
el atributo. `action`: señala la acción que va realizar el formulario al enviarse.
`miltiparformdata` es para enviar archivos

### Ejemplos & Consejos
Es mejor tener varias copias de la imagen para cada tamaño de la foto. Pq asi no sobrecargamos la imagen.


_"sistema de facturación un archivo XML pesa 30kb pero comprimido pesa 4-3 kb,pq optimizar?, porque el volumen de información de certificados son alrededor de 1000 diarios, lo que en poco tiempo puede generar mucho espacio"_

### Organizmos Reguladores
**W3C:** Regulación de la web.

### Programas útiles
> Validator w3c.

### Code & Commads
```html
<img>: incluye las imagenes.
<meta>
```

Format
## CSS
Son reglas, sirven para definir el estilo (visualización).
el estilo se puede aplicar en `<head>` ( a nivel de documento). en un atributo particular `<p style="">..` en el que solo modifico este elemento.
Se pueden mezclar clases.

**Clases** definen un estilo que se puede agregar a un elemento. esto se puede hacer de la forma:
`.class{ atributte1 atributte2}` o `p.class{ atributte1 atributte2}`
la diferencia es que `.class` lo puedo aplicar a cualqueir atributo, mientras que, `p.class` lo puedo aplicar solo a parrafos.
tbm de la forma:
`input{}`: define el estilo para todos los atributos de tipo "input". `:rule {}`
### Ejemplos & Consejos
La forma más usada de definir estilo es con una hoja de estilos a parte. Y luego llamar el estilo que necesito dónde lo necesito.
usar el atributo `placeholder` en los input como sugerencia de lo que necesito rellenar en el input.

**Ej1:**
.
El navegador se encargad de dibujar o mostrar ciertas cosas, en algunos casos no especificados, y en otros especificados.
Por ejemplo el date picker cuando coloco el atributo date.
Eso significa que un mismo "html" puede tener diferentes comportamiento.
_¿Cómo lo hago para dar un soporte universar?_
Tenemos que generar nosotros el html que queremos mostrar.

_¿Tengo que usar algo que ya se ha hecho muchas veces?_
Si les pedimos validador de rut, email. No es necesario reimplementarlo. Pueden buscar uno ya hehco y usarlo.

_Que se apegue al standard_

### Programas Útiles
> caniuse.com: Buscar que soporte tienen ciertos atributos ej: date.
### Organizmos Reguladores
### Code & Commands
### Material extra del Tópico
Se puede "programar" en CSS

Format
## JavaScript


No es simple pq hacemos uso de los recursos del cliente. Esto pq hacemos uso del intérprete JS que está en el equipo del cliente.
Se usa el tag `<script>`

El tipo de las variables se define por contexto (lenguaje interpretado).
`var f=1;`

El objeto `document`se usa para acceder al documento html en el que estoy (y darle instruccione como write).

Las funciones reciben los valores como parametro igual que en C.
Para usar referencias hay que crear un objeto con `new`

### Ejemplos & Consejos
### Programas Útiles
### Organizmos Reguladores
### Code & Commands
1. Set JavaScript:

```html
<script language="JavaScript">
<!--
  ...
-->
</script>
```
2. Use especial objects:

```html
<script>
... document.write(i + "!=" +f+ "<br>")
</script>
```
3. Lanzar una acción por evento. Acceder a un valor del input por el nombre

```html
<element ... Event = "Action"
<input ... onclick="calculate">
<input ... onchange="erease">
<script>
... document..
</script>
```
4. Crear una referencia

```JavaScript
var xmas = new Date(2007,12,25);
var solstice = xmas;
solstice.setDate(21); //modifico el valor de date
document.write(xmas,Date(2007,12,22));
```
5. Acceder al valor de un input en un formulario
```JavaScript
var principal = document.loan.principal.value;
```

### Material extra del Tópico
Chrome fue creado pensado en ser eficiente en el uso de JavaScript.
Firefox tiene un procesador más rápido...
"Pero hoy por hoy no tengo certeza de cual es más rápido (profe)".
Datofreak: Entre 1500-1600 ingenieros para desarrollar chrome.
**WebGl:** Aplicaciónes gráficas con soporte en la web.
Solo necesitas el navegador vs tener que desarrollar para cada framework.

## CGI
Programas que se ejecutan en el servidor.
Pueden ser escritos en cualquier lenguaje.
Acuerdo de programas de como se ejecutan los programas que se ejecutan en el lado del servidor.

### Ejemplos & Consejos
Ejemplos de lenguaje, pueden ser C (aunque en la practica no se usa). Y ultimamente disponible WebAsembly (programación eficiente).

### Programas Útiles
### Commands
### Organizmos Reguladores
### Code
### Material extra del Tópico

## PHP
Permite añadir código al HTML
Conocido por arquitectura LAMP
tambie se pueden generar imágenes y PDF en línea.
se puede comunicar con diferentes bases de
**Se ejecuta en el lado del servidor** y al cliente solo le llega el resultado en HTML.

### Ejemplos & Consejos
Se puede acceder a los strings como arreglos.
todo son arreglos

```php
<?php
  $arr = array("foo" => "bar", 12 => true);
?>
```

Si no se le dan valores de índices al arreglo, php les asgina un ídices que es el mayor entero más uno.
`$_SESSION` guarda las variables de sesion http, diferente a la sesión de log en una página.

ejemplo: le pasamos una variable con get a un script php como por
`localhost:/...../hola.php?Juan`
Del lado del servidor
```php
<?php
  echo "<p>hola<p>".$_GET[0];
?>
```
Si no se valida en el lado del servidor los datos como en este ejmplo se pueden hacer validaciones de usuario.
porque yo podría ingresar valores imap_mail_como
`localhost:/...../hola.php?Juan</p><img scr= www.fotofea.cl>`
```html
  <p>Hola Juan
  <img scr= www.fotofea.cl>
```
¿Cuando es útil tener variable con nomre de varibles?
preguntar al profe...

### Programas Útiles
### Commands & Code
`php -a` PHP se puede usar desde la línea de comandos. Abre una interactive Shell
Sintaxis


```php
  <?php
    echo "Esto es una prueba"; //comentarios
    //variables
    $un_bool= TRUE; // una valor booleano;
  ?>
```
Para usar variable globales usamos `global`
```
  <?php
    $a = 1;
    $b = 2;
    function suma(){
      global $a, $b;
      echo $a + $b;
    }
  ?>
```
el modificador `static`
variables con nombres variables ej:`$$a` <br>
```php
  <?php
  $a = 'hola';
  $$a = 'mundo';
  ?>
```
Tambien al ser interpretado los valores de las varibales dependen del contexto.

### Organizmos Reguladores

### Material extra del Tópico
se puede accerder a información del cliente con:
  `$_SERVER = USER_AGENT`



# Aplicación en General

info

### Ejemplos & Consejos
Hay que tener en consideración el tipo de usuario, los diferentes tipos de usuarios, a la hora de dasarollar la aplicación.
si es una página si o si debería ser responsive.

**Vulnerabilidades:**
Aveces no se procesan ciertos archivos en le lado del servidor, entonces el servidor hacer Directory Listing. Pero con eso nosotros dejamos habilidatos publicamente a cualquiera que se conecte al servidor todos estos directorios.

Nunca podemos controloar lo que nos envía el usuario

Los servidores almancenan información de los "clientes y navegadores que nos están visitando"
Las injecciones de códgido, son en lenguaje que se procesa en el navegador.

### Programas Útiles
> wev.dev
### Commands
`'indef of'site:uchile.cl` lista los archivos y directorios indexados en un servidor, asociados a una dirección

### Organizmos Reguladores
### Code
### Material extra del Tópico
WAI recomendaciones de accesibilidad de la web
Bot net: es una red de dispositivos conectados, usualmente una applicación maliciosa, para hacer pedidos a tal día a tal hora a cierta dirección. Una botnet es capar de dejar fuera de linea a cualquier empresa.


Format
## php & DataBases


### Ejemplos & Consejos
La legalidad de lo que hay en internet esta sujeta a la legislación territorial. Ejemplo de material "pedofilico en .ru" <br>
Nunca guardar archivos según los campos entregados con el cliente. <br>
Para verficar el tipo (o MIME type) revisar la extensión en el binario del archivo,nunca confiar en el nombre. <br>
Generar nombres seguros para los archivos en el lado del servidor. <br>
El tamaño maximo de carga de archivos, default de php es de 10mb.
También la cantidad máxima de archivos que puedo agregar en un upload.

### Programas Útiles
### Commands
`curl`
### Organizmos Reguladores
**Sintaxis:** Ansi SQL
nx-domains.
### Code
### Material extra del Tópico
