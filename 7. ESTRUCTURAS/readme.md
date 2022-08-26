# ESTRUCTURAS DE CONTROL
En programación, las estructuras de control permiten modificar el flujo de ejecución de las instrucciones de un programa.

Con las estructuras de control se puede:

De acuerdo con una condición, ejecutar un grupo u otro de sentencias 

De acuerdo con el valor de una variable, ejecutar un grupo u otro de sentencias

Ejecutar un grupo de sentencias mientras se cumpla una condición

Ejecutar un grupo de sentencias hasta que se cumpla una condición

Ejecutar un grupo de sentencias un número determinado de veces

Todos los lenguajes de programación modernos tienen estructuras de control similares. Básicamente lo que varía entre las estructuras de control de los diferentes lenguajes es su sintaxis; cada lenguaje tiene una sintaxis propia para expresar la estructura.

## ESTRUCTURA CONDICIONAL if

La finalidad de utilizar la estructura condicional es tomar una decisión con base en el valor booleano de una expresión, es decir, determinar si la
condición es verdadera o falsa.

De acuerdo a su complejidad se clasifica en:

* Simple. Donde la estructura ejecuta un bloque de instrucciones cuando la condición es verdadera, en caso contrario ignora ese bloque y continúa con la ejecución del
resto de las instrucciones.

EJEMPLO

![image](https://user-images.githubusercontent.com/91554777/158930619-e2d58b1c-b8d2-4c0c-8ebf-0240905f15ef.png)

Algoritmo y diagrama de flujo donde se pida la edad del usuario; si es mayor de edad debe aparecer un mensaje indicándolo.

ALGORITMO

1. inicio
2. declarar(edad)int
3. mostar("ingresa tu edad")
4. asignar(edad)
5. SI(edad >= 18)
    MOSTAR("eres mayor de edad")
6. fin

![image](https://user-images.githubusercontent.com/91554777/158934020-f979a26c-e941-4d0c-9594-09c4f28560e5.png)


* Compuesta. Evalúa una condición, si ésta es verdadera ejecuta el bloque de instrucciones más cercano, en caso contrario, realiza acciones alternativas.

EJEMPLO

![image](https://user-images.githubusercontent.com/91554777/158930716-3465e05b-0a6b-4f72-97d9-37f524278675.png)

Se desea escribir un algoritmo y diagarama de flujo para un programa que pida la altura de una persona, si la altura es menor o igual a 150 cm envíe el mensaje: Persona de altura baja; si la altura está entre 151 y 170 escriba el mensaje: Persona de altura media y si la altura es mayor al 171 escriba el mensaje: Persona alta.

ALGORITMO

1. inicio
2. declara(altura)float
3. mostar("ingresa tu altura  en metros, ejemplo: 1.59")
4. asigna(altura)
5. SI(altura <= 1.50)
  ENTONCES muestra("persona de baja altura")
  SINO
    SI(altura <= 1.70)
    ENTONCES muesta("persona de altura media")
    SINO
      SI(altura > 1.70)
      ENTONCES muestra("persona alta")
      FINSI
    FINSI
  FINSI
5. fin

DIAGRAMA DE FLUJO

![image](https://user-images.githubusercontent.com/91554777/158934744-185c56c3-a1f8-4560-9a1d-3a389960b9fd.png)

Quieres ver corriendo el código en JS https://jseditor.io/

    var altura;
    altura = parseFloat(prompt("ingresa tu altura en metros, ejemplo 1.89"))
    if(altura <= 1.50){
        alert("persona de baja altura")
    }else if(altura <= 1.70){
        alert("persona de altura media")

    }else if(altura > 1.70){
        alert("persona alta")
    }



* Múltiple o según sea. Evalúa una condición y dependiendo de su valor booleano elige el bloque de instrucciones a ejecutar de entre varias opciones.

EJEMPLO

![image](https://user-images.githubusercontent.com/91554777/158938740-fdb87d55-ab33-4689-8390-4149afae1c0d.png)

Realizar algoritmo y diagrama de flujo para el siguiente problema: Dado un numero entre 1 y 7 escriba su correspondiente día de la semana así:
1- Lunes 2- Martes 3- Miércoles 4- Jueves 5- Viernes 6- Sábado 7- Domingo

ALGORITMO

1. inicio
2. declara(dia)int
3. muestra("Ingrese un número para escribir su día")
4. asigna(dia)
5. EN CASO DE (dia) HAGA
    caso 1: mostar("lunes")
    caso 2: mostar("martes")
    caso 3: mostar("miércoles")
    caso 4: mostar("jueves")
    caso 5: mostar("viernes")
    caso 6: mostar("sábado")
    caso 7: mostar("domingo")
    SINO mostrar("Ingresaste un número fuera del rango 1-7")
  FIN CASO
6. fin

DIAGRAMA DE FLUJO

![image](https://user-images.githubusercontent.com/91554777/158935273-82e0dcc6-0534-43d0-a7ac-1c840f7fc7d7.png)

Quieres ver corriendo el código en JS https://jseditor.io/

    var dia;
    dia = prompt("Ingrese un número para escribir su día");
    dia=parseInt(dia);
    switch(dia){
        case 1:alert("lunes");
        break;
        case 2:alert("martes");
        break;
        case 3:alert("miércoles");
        break;
        case 4:alert("jueves");
        break;
        case 5:alert("viernes");
        break;
        case 6:alert("sábado");
        break;
        case 7:alert("domingo");
        break;
        default:alert("debe ingresar un número en el rango de 1-7")

    }

## ESTRUCTURAS DE CONTROL ITERATIVAS
Las instrucciones de repetición, de iteración o bucles, facilitan la repetición de un bloque de instrucciones, un número determinado de veces o mientras se cumpla una condición.

Por lo general, existen dos tipos de estructuras iterativas o bucles en los lenguajes de programación. Encontraremos un tipo de bucle que se ejecuta un número preestablecido de veces, que es controlado por un contador o índice, incrementado en cada iteración.

Por otro lado, encontraremos un tipo de bucle que se ejecuta mientras se cumple una condición. Esta condición se comprueba al principio o el final de la construcción.

Existen distintos tipos de estructuras como son:

• Para (for). Con ella se establece el número de veces que una serie de instrucciones debe repetirse, lo cual determinas como parte de la solución a un problema en un algoritmo. Sus componentes son:

o Expresión inicial. Indica con qué valor numérico inicia el ciclo.

o Condición. Es la expresión relacional o lógica por evaluar, con ella se determina cuándo se detendrá el ciclo

o Incremento. Indica el valor numérico que se le sumará a la expresión inicial tras completar el ciclo.

Con for, las instrucciones se repiten el número de veces que le decimos, normalmente le ponemos un número ( o el valor de una variable o una constante).

![image](https://user-images.githubusercontent.com/91554777/159377598-b75e59e9-d57d-4e9e-9e78-1a625daccca1.png)


![image](https://user-images.githubusercontent.com/91554777/159377169-bd0aa604-e919-4ac4-906a-e29a7092cd97.png)

### EJEMPLOS:

Elaborar un algoritmo y diagrama de flujo para un programa que cuente del 0 al 10 e imprima dicho conteo.

ALGORITMO
1. inicio
2. declarar(numero) int
3. asignar(numero=0)
4. PARA(numero <= 10)
    mostrar(numero)
    numero = numero + 1
    FIN PARA
5. fin

DIAGRAMA DE FLUJO

![image](https://user-images.githubusercontent.com/91554777/159378378-aaef6558-0440-4291-8dbb-537919e10a28.png)


Elaborar un algoritmo y diagrama de flujo para un programa que cuente desde el 0 hasta el 1000 de dos en dos

ALGORITMO
1. inicio
2. declarar(numero) int
3. asignar(numero=0)
4. PARA(numero <= 1000)
    mostrar(numero)
    numero = numero + 2
    FIN PARA
5. fin

DIAGRAMA DE FLUJO

![image](https://user-images.githubusercontent.com/91554777/159380702-72eb63b4-cdc4-461e-82c5-ab3844b0a86e.png)

## ALERT
Debemos de tratar de no caer en ciclos infinitos porque eso colapsaria nuestro sistema

Algoritmo y diagrama de flujo que imprima el valor de una variable en iteracion.

ALGORITMO

1. inicio
2. declarar(contador)int
3. asignar(contador)
4. PARA(contador > 0)
    mostrar(contador)
    FIN PARA
6. fin

![image](https://user-images.githubusercontent.com/91554777/159386586-7e25dbcb-b137-49aa-85c1-8fca9a46bef9.png)

Realizar algorito y diagrama de flujo que solicite un número y que imprima la tabla del multiplicar del 1 al 10 de ese número

ALGORITMO
1. inicio
2. declarar(numero,contador,resultado)int
3. asignar(contador=1)
5. mostrar("ingresa el número del que quieres saber su tabla de multiplicar del 1 al 10")
6. asignar(numero)
7. PARA(contador <= 10)
    resultado=numero*contador
    mostar(numero * contador = resutado)
    contador=contador + 1
    FIN PARA
8. fin

DIAGRAMA DE FLUJO

![image](https://user-images.githubusercontent.com/91554777/159388185-d6eaf814-17ab-4f1d-a7b6-545150919894.png)

Quieres ver corriendo el código en JS https://jseditor.io/

    var contador;
    var numero;
    var resultado;
    numero = prompt("ingresa el número del que quieres saber su tabla de multiplicar del 1 al 10")
    for(contador = 1;contador <= 10;contador++){
        resultado=numero * contador;
        document.write(numero + " * " + contador + " = " + resultado + "<br>")
    }


Mientras (while). Se emplea para ejecutar un bloque de instrucciones en un ciclo sin necesidad de establecer el número de veces que lo hará. Se compone por una expresión lógica, relacional o aritmética, que es evaluada en una condición.

![image](https://user-images.githubusercontent.com/91554777/159615891-59e21286-ab60-4dd2-bfac-5f22f8f857fa.png)

A diferencia de para, en el ciclo mientras no se sabe necesariamente con exactitud como cambia la variable de control, lo que si se debe saber con precisión es donde comienza el ciclo y donde termina. Por lo tanto, como no se sabe toda esa información, tampoco se sabe el número de iteraciones que realizará el ciclo.

Un bucle while itera o repite un bloque de código mientras una condición tiene el valor true. Se puede escribir de la siguiente manera:

![image](https://user-images.githubusercontent.com/91554777/159604598-08b0bb7f-a8fb-4f0f-af78-ecc63b91dad4.png)

NOTA: EN LA MAYORIA DE LENGUAJES EL BUCLE WHILE PUEDE TAMBIEN TENER UNA VARIABLE CONTADOR

Algoritmo y diagrama de flujo de un programa que imprima los números del 1 al 10

ALGORITMO

1. inicio
2. declarar(contador)int
3. asignar(contador)
4. MIENTRAS(contador<=10)
    mostrar(contador)
    contador=contador+1
    FINMIENTRAS
5. fin

DIAGRAMA DE FLUJO

![image](https://user-images.githubusercontent.com/91554777/159613295-37a42d3b-5805-4b6e-a96b-f4a370b54acd.png)

Quieres ver corriendo el código en JS https://jseditor.io/

    var contador;
    contador=1;
    while(contador<=10){
        document.write(contador + "<br>")
        contador++
    }


EJEMPLO

Realizar un algoritmo y diagrama de flujo que imprima en pantalla la palabra “Hola”, mientras se presione número 1. 

ALGORITMO
1. inicio
2. declarar(numero)int
3. mostrar("ingresa un número")
4. asignar(numero)
5. MIENTRAS(numero != 1)
   mostrar("número incorrecto")
   mostrar("ingresa un número")
   asignar(numero)
   FINMIENTRAS
6. mostrar("numero correcto")
7. fin

DIAGRAMA DE FLUJO

![image](https://user-images.githubusercontent.com/91554777/159609434-c4a51247-8fd4-4619-aecf-d3e63a2e0629.png)

Quieres ver corriendo el código en JS https://jseditor.io/

    var numero;
    numero = prompt("ingresa un numero");
    while(numero!=0){
        alert("numero incorrecto")
        numero = prompt("ingresa un numero")
    }
    alert("numero correcto")

Realiza un algoritmo y diagrama de flujo para un programa que almacene la cadena de caracteres para una contraseña y email, pregunte al usuario por la contraseña y email e imprima por pantalla si la contraseña y el email introducidos por el usuario coincide con los guardadados en las variables, repetir hasta que coincida el dato.
ALGORITMO

1. inicio
2. declarar(email,contra,email_validar,contra_validar)string
3. asignar(email_contra)
4. asignar(contra_validar)
5. mostrar("ingresa tu correo")
6. asignar(email)
7. mostrar("ingresa tu conraseña")
8. asignar(contra)
9. MIENTRAS(email != email_validar && contra != contra_validar) 
    mostrar("email o contraseña incorrectos")
    mostrar("ingresa tu correo")
    asignar(email)
    mostrar("ingresa tu conraseña")
    asignar(contra)
    FINMIENTRAS
10. mostrar("bienvenido")
11. fin

DIAGRAMA DE FLUJO



![image](https://user-images.githubusercontent.com/91554777/159611442-7021d29f-c727-44d4-baef-84cc1d862425.png)



Quieres ver corriendo el código en JS https://jseditor.io/

    var contra;
    var correo;
    var correo_validar;
    var contra_validar;
    correo = prompt("ingresa tu correo");
    contra = prompt("ingresa tu contraseña");
    correo_validar="prueba@correo.com";
    contra_validar="123456";
    while(correo!=correo_validar && contra!=contra_validar){
        alert("correo o contraseña incorrecta");
        correo = prompt("ingresa tu correo");
        contra = prompt("ingresa tu contraseña");
    }
    alert("Bienvenido(a)");
    
Hacer Mientras (do...while). Se usa cuando el problema a resolver requiere que se ejecute por lo menos una vez el ciclo. Se compone por una condicional cuya expresión se evalúa después de ejecutar el bloque de instrucciones. El ciclo finaliza cuando la condición se vuelve falsa.

![image](https://user-images.githubusercontent.com/91554777/159619170-34494e7b-90aa-43a7-a9a8-447b7422d664.png)


EJEMPLO

Algoritmo y diagrama de flujo de un programa que imprima los números del 1 al 10

ALGORITMO

1. inicio
2. declarar(numero)int
3. asignar(numero)
4. HACER mostar(numero)
    numero=numero+1
    MIENTRAS(numero<=10)
    FIN HACERMIENTRAS
5. fin

![image](https://user-images.githubusercontent.com/91554777/159619991-6304e160-fc52-49db-9e82-5d3043aa927b.png)


INGRESA A LA SIGUIENTE PRESENTACION
    
https://docs.google.com/presentation/d/1HuS9KM8UKOnO84M0GBDz_WBeKo23BVJs34tpq2WZHSU/edit?usp=sharing
