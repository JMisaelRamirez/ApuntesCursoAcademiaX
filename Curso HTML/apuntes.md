# **APUNTES DE HTML**
## **1. Set Up**

* HTML permite estructura un pagina WEB

### **Extension _HTML Preview de George Oliveira**
Esta extension nos permite vizualizar el codigo HTML dentro de VSC

### **Etiquetas**
Las etiquetas se simbolizan de la siguiente manera <_letra_></_letra_>. Cada una de las etiquetas en HTML simbolizan algo.

Hay etiquetas que se cierran directamente. 
### **Elementos**

Los elementos (elements) en HTML se escriben entre etiquetass (< >) y pueden tener atributos que les proporcionan propiedades adicionales. Por ejemplo, el elemento (element) < p > se utiliza para crear un párrafo de texto, mientras que el elemento < img > se utiliza para insertar imágenes en una página.

Cada elemento en HTML tiene una sintaxis específica y un propósito determinado.
### **Atributos**
Tienen caracteristicas especiales en las etiquetas. Los atributos nos permiten hacer cosas diferentes dentro de una etiqueta. 

### **Entidades de caracteres**
Claro que sí, una entidad de carácter en HTML es un código especial que se utiliza para representar caracteres que de otra manera no se podrían incluir directamente en una página web.

Por ejemplo, si quisieras incluir el signo de mayor que (>) en tu página HTML, no podrías hacerlo simplemente escribiéndolo directamente en tu código, ya que ese símbolo se utiliza para cerrar etiquetas. En su lugar, tendrías que utilizar una entidad de carácter como ">" para que el símbolo sea interpretado correctamente por el navegador.

Las entidades de carácter se escriben comenzando con el símbolo "&", seguido del nombre o número de la entidad, y terminando con el símbolo ";". Por ejemplo, "<" es la entidad para el signo de menor que (<), "&" es la entidad para el símbolo "&", y "€" es la entidad para el símbolo del euro (€)

### **Document object module (DOM)**
Es la representacion del HTML en la pagina. Es como un arbol que tiene etiquetas dentro de etiquetas. Ejemplo: 

```html
<p> Parrafo
    <i>i
        <b>B</b>
    </i>
    <i>i
        <b>B</b>
    </i>
    <i>i
        <b>B</b>
    </i>
</p>
```
**OutPut:**
<p> Parrafo
    <i>i
        <b>B</b>
    </i>
    <i>i
        <b>B</b>
    </i>
    <i>i
        <b>B</b>
    </i>
</p>

## **2. Textos**
* HTML se trata de dar estructura a la pagina WEB
* ¿Cual es la diferencia de la etiqueta < i > y < em >?
* ¿Cual es la diferencia entre linea y bloque?





* Agregar el comando em
* Agregar que significa la letra de las etiquetas: Ejem->b : Bold
* Agregar a comandos la etiqueta strong. Representa mayor importancia, seriedad, o urgencia por su contenido y el elemento b es para llamar la antencion
* Elemeto small en una etiqueta: Representa menos impotancion. No es de mucha importancia. 
* El elemento span no significa nada, se utiliza dentro de un bloque y solo define lo que esta dentro de span como su hijo.

* Agregar la palabra reservada &nbsp;
---
```html
<p>Este es un texto <span>de un animal</span></p>
```
output:
<p>Este es un texto <span>de un animal</span></p>

---
---

Otra forma de indicar un hijo de otra etiqueta es: 
```html
<p>Este es un texto <p>de un animal</p></p>
```
output:
<p>Este es un texto <p>de un animal</p></p>

---

LA diferencia de span no realiza un salto de parrafo a comparacion de p y en la forma en la que estan definos ambas expresiones, las dos forman generan un hijo de un padre.

*La entidad de caracter &nbsp: 
Esta entidad de caracter nos permite agregar espacios a un texto. Agregando espacios a un texto con esta entidad nos ayuda a mantener riguido el texto al momento de mover el tamaño de la venta.

# Notas

* When you add a lower rank heading element to the page, it's implied that you're starting a new subsection.

After the h3 element with the Things cats love: text, add an unordered list (ul) element. Note that nothing will be displayed at this point.

        <h2>Cat Lists</h2>
        <h3>Things cats love:</h3>
        <ul></ul>

Use list item (li) elements to create items in a list. Here is an example of list items in an unordered list:

<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
Within the ul element nest three list items to display three things cats love:

cat nip, laser pointers, lasagna

## **3. Encabezados**

Los header son encabezados. La seleccion de el tipo de _h_ no se hace para dar dirente tipo de estilos, para eso se utiliza css, mas bien, se hace para dar dirente significado a la estructura de html

```html
<h1>Titulo</h1><!--header (encabezado)-->
<h2>Subtitulo</h2>
<h3>Subtitulo</h3>
<h4>Subtitulo</h4>
<h5>Subtitulo</h5>
<h6>Subtitulo</h6>
```
OutPut:

<h1>Titulo</h1>
<h2>Subtitulo</h2>
<h3>Subtitulo</h3>
<h4>Subtitulo</h4>
<h5>Subtitulo</h5>
<h6>Subtitulo</h6>

> Cuando se utiliza _h1_ lo que se le esta diciendo a la pagina es que este es el titulo de la pagina. 

## **4. Listas**
### **Listas desordenadas (Unorder list)**
Una lista desordenada esta indicada por biñetas (bullet list)

```html
<p>Mis hablidades blandas</p>
<ul><!--ul: unorder list-->
    <li></li> <!--li: list-->
    <li></li>
</ul>
```
Output:
<p>Mis hablidades blandas</p>
<ul>
    <li>Amable</li>
    <li>Paciente</li>
    <li>Tolerante</li>
</ul>

### **Listas ordenadas (Order Lists)**
Una lista ordenada esta enumerada. Ejemplo:

```html
<ol> <!--ol: Order List-->
    <li>Abrir la puerta</li>
    <li>Sacar la basura</li>
    <li>Cerrar la puerta</li>
</ol>
```

OutPut:

<ol>
    <li>Abrir la puerta</li>
    <li>Sacar la basura</li>
    <li>Cerrar la puerta</li>
</ol>

### **Listas de definicion (Definition Lists)**
Una lista de definicion sirve para definir palabras. Ejem:

```html
<dl><!--dl: Definition List-->
    <dt>HTML</dt><!--dt: Defintion Text. Define la palabra a definir-->
    <dd>Es un lenguaje de marcado de texto.</dd><!--dd: Do Definition-->
    <dd>Se utiliza para el desarrollo de paginas de internet.</dd>
</dl>
```

OutPut:

<dl><!--dl: Definition List-->
    <dt>HTML</dt><!--dt: Defintion Text. Define la palabra a definir-->
    <dd>Es un lenguaje de marcado de texto.</dd>
    <dd>Se utiliza para el desarrollo de paginas de internet.</dd>
</dl>

## **5. Formatos**

### **Agregar codigo en HTML**
El elemento code nos permite agregar codigo de cualquier lenguaje en HTML

```html
<p>Este es un codigo de CSS:
    <code>{backgroud: blue;}</code>
</p>
<p>Utiliza este codigo de HTML
    <code></code>
</p>
```

OutPut:

<p>Este es un codigo de CSS:
    <code>{backgroud: blue;}</code>
</p>

### **Rupura de linea (Line Break)**
Este elemento nos permite colocar el texto en otra linea.

```html
<p> <!--br: Break. Tambien dice: Aqui termina esta linea-->
    Quiero que<br />este texto<br />este en<br />varias lineas.
</p>
```

OutPut:
<p>
    Quiero que<br />este texto<br />este en<br />varias lineas.
</p>


### **Subindice y Superindice**

```html
<!--Subindice. sub: Sub Indice-->
<p>CO<sub>2</sub></p>
<!--Superindice. sup: Super Indice-->
<p>n<sup>3</sup></p>
```
Ouput:
<!--Subindice. sub: Sub Indice-->
<p>CO<sub>2</sub></p>
<!--Superindice. sup: Super Indice-->
<p>n<sup>3</sup></p>

## **6. Citas**

### **Citas de bloque**
```html
<blockquote> <!--blockquote: Cita de bloque-->
    <p>La piedra angular del crecimiento es el dolor</p>
    <cite>Bill Wilson</cite><!--cite: Cita-->
</blockquote>
```

Output:

<blockquote>
    <p>La piedra angular del crecimiento es el dolor</p>
    <cite>Bill Wilson</cite>
</blockquote>

### **Citas con comillas**

```html
<p>Bill Wilson, dijo:
    <q>El dolor es la piedra angular del crecimiento. La humildad es el reconocimineto de que y quienes somos en la realidad seguido de un esfuerzo sincero de querer cambiar.</q>
</p>
```

OutPut:

<p>Bill Wilson, dijo:
    <q>El dolor es la piedra angular del crecimiento. La humildad es el reconocimineto de que y quienes somos en la realidad seguido de un esfuerzo sincero de querer cambiar.</q>
</p>

## **7. Time**
Los elementos de tiempo, en este caso,**&lt;time&gt;** nos permiten brindarle informacion a Google de alguna fecha importante que deseemos destacar dentro de nuestra pagina web, asi cuando los usuarios busque algun evento publicado en nuestra pagina, google lo podra buscar. 

El atributo **datetime** nos ayuda a definir la hora o fecha de algun evento. Puede ser que se coloque la fecha por separado o incluso junto.


```html
<!--Ejemplo 1: -->
<p>Nos vemos el 
    <time datetime = "2024-04-20">sabado</time> <!--time: tiempo, datetime-->
    a las
    <time datetime = "16:20:00.5-08:00">4:20</time>
</p>
<!--Ejemplo 2: -->
<p>Nos vemos a las
    <time datetime = "2024-04-20 10:00-0800">10</time>
</p>
```

OutPut:

<p>Nos vemos el 
    <time datetime = "2024-04-20">sabado</time> <!--time: tiempo, datetime-->
    a las
    <time datetime = "16:20:00.5-08:00">4:20</time>
</p>
<!--Ejemplo 2: -->
<p>Nos vemos a las
    <time datetime = "2024-04-20 10:00-0800">10</time>
</p>

## **8. Vinculos**

Los vinculos son etiquetas que te prermiten ir a otras paginas o direcciones. Se utiliza el atributo **href** el cual se le asigna un vinculo o direccion. 

```html
<p>Da click en la palabra 
    <a href = "facebook.com">Facebook</a> para dirigirte a Facebook
</p> <!--href: HyperLink Reference-->
```
Output:

<p>Da click en la palabra <a href = "facebook.com">Facebook</a> para dirigirte a Facebook</p>

## **9. Rutas**

### **Vinculo relativo**
Un vinculo relativo es cuando se coloca un slash (barra inclinada) y se coloca . para que se dirija a la carpeta actual, .. para que se dirija a la carpeta padre. 

```html
<p>Diriguete al siguiente 
    <a href = "./codigoPruebaHTML.html">Link</a>,
    <a href = "../codigoPruebaHTML.html">Link 2</a>
</p>
```

OutPut:

<p>Diriguete al siguiente 
    <a href = "./codigoPruebaHTML.html">Link</a>,
    <a href = "../codigoPruebaHTML.html">Link 2</a>
</p>

### **Vinculo Absoluto**
Este tipo de vinculos incluye la direccion completa para ir a un lugar.

```html
<p>Dirigite a Google con el siguiente
    <a href = "https://www.google.com/">Link</a>
</p>
```

OutPut:

<p>Dirigite a Google con el siguiente
    <a href = "https://www.google.com/">Link</a>
</p>

## **10. Navegacion**
Una pagina Web esta constituida por diferentes archivos HTML. Para navegar entre los archivos HTMl se utilizan las rutas (Vinculos). En realidad, cuando creamos archivos de HTML podremos navegar entre estos, pero, si quisieramos que mas gente acceda a nuestra pagina web, estas personas deberan de tener los archivos HTML para aceder a esta lo cual nos indica que seria imposible pasarle nuestros archivos HTML a cada persona, para ello, es comveniente comprar un servidor, que son computadoras que contienen nuestros archivos, y ademas, un dominio, por ejemplo www._nombreDelDominio_.com para que cada vez que las personas accedan a nuestro dominio los servidores proporcionen cada archivo HTML cuando las personas requieran acceder a este. 



