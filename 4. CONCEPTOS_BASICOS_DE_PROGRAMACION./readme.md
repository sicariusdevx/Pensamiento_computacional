# CONCEPTOS BASICOS DE PROGRAMACION

Cuando realizas una petición a tu equipo de cómputo, (por ejemplo,
guardar un documento en el procesador de textos), internamente se
ejecutan bloques de instrucciones escritos en un lenguaje de
programación que hacen posible las demandas del usuario.
Un lenguaje de programación es un idioma artificial creado para indicarle
a la computadora lo que debe hacer. Tiene ciertas reglas de escritura
(sintaxis) en las que utiliza símbolos y palabras clave, además de una
semántica (interpretación interna).

![image](https://user-images.githubusercontent.com/91554777/185528149-dfb66b51-7680-409e-a782-843d3fd770df.png)

Un programa es un bloque de instrucciones (código fuente) escritas en
cierto lenguaje de programación cuyo propósito es resolver un problema.

![image](https://user-images.githubusercontent.com/91554777/185528173-c89a6824-c028-4b39-a8de-67b8811edac9.png)

Para ejecutar un programa la computadora realiza una traducción de sus
componentes al lenguaje máquina, es decir, convierte las instrucciones en
cadenas de ceros y unos. Este proceso de conversión puede hacerse de
dos formas:

![image](https://user-images.githubusercontent.com/91554777/162348386-d47f858c-f37c-40c1-b284-3a36db07c36f.png)



1.- Por medio de un programa “intérprete” que traduce y ejecuta instrucción
por instrucción.

Los lenguajes interpretados son aquellos lenguajes de programación también de alto nivel en donde el código fuente debe ser traducido a un lenguaje que la máquina entienda y pueda realizar, no crean un archivo externo.

![image](https://user-images.githubusercontent.com/91554777/162349467-e2080f4c-c66a-45a8-8673-039b3215eab3.png)


Ejemplos: Python y Ruby

2.- A través de un programa “compilador” que toma al bloque de
instrucciones lo traduce sólo una vez y lo ejecuta.

Los lenguajes compilados son aquellos lenguajes de alto nivel que como su nombre lo sugiere, requieren de un compilador (programa que traduce un lenguaje de alto nivel en código máquina o lenguaje máquina) para traducirlo y crear la parte ejecutable.

Los lenguajes de alto nivel permiten escribir instrucciones en un idioma muy parecido al inglés así como hacer uso de notaciones matemáticas comunes.

Ejemplos: C y C++

![image](https://user-images.githubusercontent.com/91554777/185528241-25163e55-383f-429f-80a8-55429e785e78.png)

C, C++ y Go son lenguajes de programación compilados. JavaScript, Python y Ruby son lenguajes interpretados. ¿Cuál es la diferencia y las ventajas/desventajas de un lenguaje compilado versus uno interpretado?

Tanto compiladores como interpretadores son programas que convierten el código que escribes a lenguaje de máquina.

![image](https://user-images.githubusercontent.com/91554777/162349134-07503d15-a2e2-48df-90dd-b43a702d0481.png)


Lenguaje de máquina son las instrucciones que entiende el computador (el procesador para ser más exactos) en código binario (unos y ceros).

Un ejemplo de lenguaje interpretado

Ruby es un lenguaje interpretado, así que podemos crear un archivo llamado hola.rb con el siguiente código, o cualquier código válido en Ruby (a esto se le conoce como el código fuente):

puts "Hola Mundo"
Lo ejecutariamos directamente ingresando el siguiente comando en la consola:

$ ruby hello.rb
Nos apareceria debajo la cadena “Hola Mundo“.

Un ejemplo de lenguaje compilado

Un lenguaje compilado tiene un paso adicional. Necesitamos un compilador de C como gcc y podemoss crear un archivo llamado hello.c con el siguiente contenido, o cualquier código válido en C:

         #include <stdio.h>
        int main()
        {
            printf("Hola Mundo");
            return 0;
        }

Antes de ejecutarlo debes compilarlo con el siguiente comando:

    $ gcc hello.c -o hello
    
Eso crea un archivo llamado hello (sin extensión) con el código de máquina (llamado el ejecutable) que puedes correr en la consola con el siguiente comando:

    $ ./hello
    
Nos aparecería la cadena de texto “Hola Mundo” debajo. Si necesitas cambiar el código fuente debes volverlo a compilar y ejecutarlo nuevamente.

Ventajas y desventajas

En general, el ciclo de desarrollo (el tiempo entre el momento en que escribes el código y lo pruebas) es más rápido en un lenguaje interpretado. Eso se debe a que en lenguajes compilados es necesario realizar el proceso de compilación cada vez que cambias el código fuente, aunque con herramientas adicionales se puede automatizar.

Otra desventaja de un lenguaje compilado es que cuando compilas un programa debes crear ejecutables para cada uno de los sistemas operativos en los que lo vayas a utilizar. Un ejecutable creado para Linux no va a servir en Windows por ejemplo.

Sin embargo, un lenguaje compilado es mucho más rápido que uno interpretado. Esto se debe a que cuando es ejecutado ya se encuentra en código de máquina y eso también le permite hacer algunas optimizaciones que no son posibles con un lenguaje interpretado.

Además de la velocidad, otra desventaja de un lenguaje interpretado es que, para ser ejecutado, debes tener instalado el interpretador. Esto no es necesario en un lenguaje compilado que es convertido a lenguaje de máquina1.

En general, un lenguaje compilado está optimizado para el momento de la ejecución, aunque esto signifique una carga adicional para el programador. Por otro lado, un lenguaje interpretado está optimizado para hacerle la vida más fácil al programador, aunque eso signifique una carga adicional para la máquina.

El caso de Java
Java es un lenguaje particular porque es compilado, pero es compilado a un lenguaje intermedio llamado bytecode, que después es interpretado. Los creadores de Java querían crear un lenguaje compilado, pero que se pudiera ejecutar en cualquier sistema operativo y procesador sin necesidad de crear varios ejecutables.

Es por eso que si quieres ejecutar código Java debes instalar el JRE (Java Runtime Environment), que es el programa que se encarga de interpretar el bytecode al que son compilados los programas de Java.

Si deseas compilar código Java no es suficiente instalar el JRE, necesitas el JDK (Java Development Kit) que incluye el compilador, entre otras herramientas de desarrollo.

Otros lenguajes que están siguiendo este mismo modelo incluyen Elixir y C#, entre otros.

Se puede decir que los lenguajes de alto nivel se pueden dividir en tres ramas: puramente compilados (C++, Go, etc.), parcialmente compilados (Java, Elixir, etc.) e interpretados (Ruby, JavaScript, etc.).

Sin embargo, la brecha entre estas ramas cada vez es menor. Hoy existen lenguajes compilados a lenguaje de máquina como Go y Rust que se inclinan cada vez más en la productividad y felicidad del programador mientras que los lenguajes interpretados son cada vez más rápidos en ejecución.

Los lenguajes más próximos a la arquitectura hardware se denominan lenguajes de bajo nivel y los que se encuentran más cercanos a los programadores y usuarios se denominan lenguajes de alto nivel.

La programación en lenguajes de alto nivel es mucho más fácil; escribir programas en un lenguaje de alto nivel toma menos tiempo, los programas son más cortos y más fáciles de leer, y es más probable que estos programas queden correctos.


Los ordenadores tienen millones de interruptores que están encendidos (1) o bien apagados (0). Así, puedes darle instrucciones al ordenador por medio de bits (cadenas de 0s y 1s). Sin embargo, esto resulta demasiado complejo.

Es por ello que se crearon los lenguajes de programación de alto nivel, para escribir código legible que será traducido al lenguaje máquina (binario). Es decir, para que sean intermediarios entre los desarrolladores y el hardware.

![image](https://user-images.githubusercontent.com/91554777/162348638-87586bb6-d428-4c8b-8551-49e3d5016b56.png)

Los lenguajes de bajo nivel son aquellos que están más próximos al lenguaje de máquina (de ceros y unos). Es decir, tienen un control directo sobre el hardware.

A diferencia de los lenguajes de alto nivel, no necesitan compiladores. En cambio, se ejecutan directamente en el procesador y dependen de la arquitectura del hardware.

Los programas que se crean con estos lenguajes de bajo nivel dependen totalmente del hardware. Por esta razón, no se pueden migrar o utilizar en otras máquinas.

Además, pese a que aprovechan mejor las características del hardware, son los tipos de lenguajes más difíciles de entender y aprender.

Ejemplos ARM, MIPS, SPARC, PIC.

Existen dos tipos de lenguajes de bajo nivel: máquina y ensamblador.
