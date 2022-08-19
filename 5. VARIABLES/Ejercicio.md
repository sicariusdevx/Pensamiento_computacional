## EJERCICIO 1

¿Qué tipo de dato debe tener una variable para representar la calificación promedio de un
curso?

      float

¿Qué tipo de dato debe tener una variable para representar el número de personas en un
hogar?

      integer

¿Qué tipo de dato debe tener una variable para contener el nombre de pila de una persona?

      string

¿Qué tipo de dato debe tener una variable para registrar si está lloviendo o no?

      boolean

¿Qué tipo de dato debe tener una variable para representar la cantidad de dinero que
tienes?

      float
      
## EJERCICIO 2

Realiza un algoritmo que calcule el promedio de un alumno el cual tiene cuatro calificaciones, una por periodo, de cada materia.

      01. Inicio
      02. Declarar calif1(float),calif2(float),calif3(float),calif4(float),promedio(float)
      03. Inicializar calif1=0,calif2=0,calif3=0,calif4=0,promedio=0
      04. mostrar "Introduce las calificaciones del periodo"
      05. asignar calif1,calif2,calif3,calif4,
      06. promedio = (calif1 + calif2 + calif3 + calif4) / 4
      07. mostrar "el promedio del alumno es {promedio}"
      08. Fin
      
## EJERCICIO 3

Realiza un algoritmo para un programa que solicite al usuario su nombre y le salude usando ese nombre

      01. Inicio
      02. declarar nombre(string)
      03. Mostrar "Introduce tu nombre: "
      04. Leer nombre
      05. Mostrar "Hola, Bienvenido ", nombre
      06. Fin

## EJERCICIO 4

Realiza un algoritmo para  un programa que solicite al usuario ingresar la cantidad de kilómetros recorridos por una motocicleta y la cantidad de litros de combustible que consumió durante ese recorrido. El consumo por kilómetro es de 20.8

      01. Inicio
      02. declarar dist(float), consumo(float)
      03. mostrar "Introduce la distancia recorrida en km: "
      04. leer dist
      05. consumo = 20.8 * dist
      06. mostrar "Se consumieron ",consumo, " litros"
      07. fin

Ahora llevalos a PSINT

Pseudocódigo Ejercicio 2:

Algoritmo Promedio
    Definir calif1, calif2, calif3, calif4, prom Como Real;
    Escribir "Introduce los valores de las calificaciones";
    Escribir "Calificacion 1: ";
    Leer calif1;
    Escribir "Calificacion 2: ";
    Leer calif2;
    Escribir "Calificacion 3: ";
    Leer calif3;
    Escribir "Calificacion 4: ";
    Leer calif4;
    prom <- (calif1 + calif2 + calif3 + calif4) / 4;
    Escribir "El promedio final es: ",prom;
FinAlgoritmo

Pseudocódigo ejercicio 3

Algoritmo Promedio
    Definir nombre Como Cadena;
    Escribir "Introduce tu nombre";
    Leer nombre;
    Escribir "Hola ",nombre,". Bienvenido a PILARES.";
FinAlgoritmo

Pseudocódigo Ejercicio 4

Algoritmo Promedio
    Definir dist, consumo Como Cadena;
    Escribir "Introduce la distancia recorrida en km ";
    Leer dist;
    consumo = 20.8 * dist
    Escribir "Se consumienron ",consumo," litros;
FinAlgoritmo
