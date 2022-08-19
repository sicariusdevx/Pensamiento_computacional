En informática los datos se guardan en casillas (celdas) de memoria de la computadora, las celdas tienen un nombre, identificadores.

Los identificadores representan los datos de un prohrama.

Hay dos tipos de identificadores: constntes y variables.
## CONSTANTES
Es un dato numérico o alfanumérico que no cambia de valor durante la ejecución de un programa, por ejemplo en número Pi.


## VARIABLES  🖱️
El concepto de variable en informática hace referencia a un nombre que representa un valor y se utiliza de forma habitual en programación para guardar distintos tipos de datos para poder operar con ellos posteriormente.

![image](https://user-images.githubusercontent.com/91554777/158277246-07c3482d-31ca-4138-9ea7-aac30aa81edf.png)


Por ejemplo, en un programa informático para sumar dos números introducidos por el usuario, se guarda cada valor en una variable diferente y finalmente se realiza la operación sumando las variables. Así cada vez que se ejecute el programa el usuario podrá introducir números diferentes y obtener su suma.

Esto da pie a definir a una variable como una porción de memoria, que posee un nombre,
que sirve para almacenar un valor de cierto tipo de dato, el cual cambia durante la ejecución
del programa.

En lenguajes de programación  es necesario declarar una variable para poder utilizarla durante la codificación de un programa. La declaración consiste en indicar el nombre de dicha variable, así como su tipo, para que el lenguaje de programación pueda utilizarla de forma apropiada.

Normalmente, una variable se declara al principio de un programa o script, aunque en algunos lenguajes de programación se pueden declarar en el mismo momento de su uso.

Para declarar y asignar un valor a una variable al mismo tiempo se sigue la siguiente estructura o forma:

=

string Nombre = “Juan”

Dependiendo del lenguaje de programación la forma de declarar y asignar valores a las variables puede variar ligeramente.

Lo habitual es que una vez que una variable ha sido declarada puede modificarse a lo largo de un programa informático. Por ejemplo, si una variable de tipo entero que recoge la edad de una persona ya ha sido declarada, puede modificarse a lo largo del programa nombrando directamente su nombre y asignándole un valor: Edad = 8, y en otra parte del programa modificarla con una operación del tipo Edad = Edad + 1, para que el valor de la variable aumente en uno.

![image](https://user-images.githubusercontent.com/91554777/158277137-67d2b323-e292-4043-8616-758fd29c4712.png)

## CLASIFICACION DE LAS VARIABLES

## Por su contenido

Variables Numéricas: Son aquellas en las cuales se almacenan valores numéricos, positivos o negativos, es decir almacenan números del 0 al 9, signos (+ y -) y el punto decimal.

Ejemplo:
iva = 0.15 pi = 3.1416 costo = 2500

Variables Lógicas: Son aquellas que solo pueden tener dos valores (cierto o falso) estos representan el resultado de una comparación entre otros datos.

Variables Alfanuméricas: Esta formada por caracteres alfanuméricos (letras, números y caracteres especiales).

Ejemplo:
letra = "a" apellido = "lopez" direccion = "Av. Libertad #190"

![image](https://user-images.githubusercontent.com/91554777/158303021-6b9becae-ec80-471d-b640-fc79105ffa73.png)


## Por su uso

Variables de Trabajo: Variables que reciben el resultado de una operación matemática completa y que se usan normalmente dentro de un programa.

Ejemplo:
Suma = a + b /c

Contadores: Se utilizan para llevar el control del numero de ocasiones en que se realiza una operación o se cumple una condición. Con los incrementos generalmente de uno en uno.

Acumuladores: Forma que toma una variable y que sirve para llevar la suma acumulativa de una serie de valores que se van leyendo o calculando progresivamente.

![image](https://user-images.githubusercontent.com/91554777/158283615-cde1694d-13f2-4161-9efb-f9a99539629c.png)

## Reglas para definir variables

Siguiendo las siguientes 7 reglas para definir una variable, no tendrás problema:

* Una variable, siempre debe iniciar con una letra (mayúscula o minúscula) ó un guión bajo (_).
* Una variable, puede contener números, solamente después de  la primer letra (siguiendo la regla anterior).
* No es permitido dejar un espacio en blanco a lo largo de la variable.
* Aunque una variable puede ser del largo que tú desees, lo recomendable es que sea una variable corta (regularmente entre 20 y 30 caracteres como máximo).
* No puedes utilizar palabras reservadas para la declaración de una variable.
* El nombre de una variable es case sensitive (es decir, a mayuúsculas y minusculas).
* Utiliza un nombre que exprese algo del contexto en el cual la estás declarando.

Dicho esto, algunas declaraciones de variables correctas serían las siguientes:

nombrePaterno

IdCliente

_conteoCiclos

Mientras que algunas declaraciones incorrectas, serían las siguientes:

3puesto

numero Telefono

int



EJEMPLO

* Vamos a realizar un algoritmo que calcule el resultado de sumar dos números.

      1.- inicio
      2.- declarar numero1(int),numero2(int),resultado(int)
      3.- asignar numero1=5, numero2=15, resultado=0
      4.- resultado = numero1 + numero2
      5.- mostrar resultado
      6.- fin
      
* Agrega al mismo programa que muestre un saludo 

      1.- inicio
      2.- declarar numero1(int),numero2(int),resultado(int), saludo(str)
      3.- asignar numero1=5, numero2=15, resultado=0, saludo = "hola"
      4.- resultado = numero1 + numero2
      5.- mostrar saludo, resultado
      6.- fin

* Ahora solicitaremos los datos al usuario y cambiaremos el saludo por su nombre

      1.- inicio
      2.- declarar numero1(int),numero2(int),resultado(int), nombre(str)
      3.- mostrar "ingresa un numero"
      4.- asignar numero1
      5.- mostrar "ingresa otro numero"
      6.- asignar numero2
      7.- mostrar "ingresa tu nombre"
      8.- asignar nombre
      9.- resultado = numero1 + numero2
      10.- mostrar saludo, resultado
      11.- fin
