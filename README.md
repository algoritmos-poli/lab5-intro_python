# Laboratorio de introducción a Python

## Objetivos

### Objetivo General 

Desarrollar la capacidad de crear soluciones de software funcionales utilizando Python.

### Objetivos especificos

1. Aplicar los Fundamentos de la Programación Estructurada.
2. Dominar el Entorno de Desarrollo Profesional.
3. Construir Software con Programación Orientada a Objetos (POO).

## Referencias

1. **Notebooks de repaso** [[link]](https://github.com/algoritmos-poli/intro_python)
2. **POO en Java y Python (ejemplo comparativo)** [[link]](https://github.com/algoritmos-poli/sesiones_presenciales/tree/main/clase6/java_vs_python)
3. **Implementación de listas enlazadas - Comparación**:
   * **Lista enlazada simple** [[java]](https://github.com/algoritmos-poli/sesiones_presenciales/tree/main/clase6/linded_list/single_LL/java) [[python]](https://github.com/algoritmos-poli/sesiones_presenciales/tree/main/clase6/linded_list/single_LL/python)
   * **Lista enlazada simple con doble extremo** [[java]](https://github.com/algoritmos-poli/sesiones_presenciales/tree/main/clase6/linded_list/single_LL_double_end/java) [[python]](https://github.com/algoritmos-poli/sesiones_presenciales/tree/main/clase6/linded_list/single_LL_double_end/python)
   * **Lista doble** [[java]](https://github.com/algoritmos-poli/sesiones_presenciales/tree/main/clase6/linded_list/doubly_LL/sin_herencia/java) [[python]](https://github.com/algoritmos-poli/sesiones_presenciales/tree/main/clase6/linded_list/doubly_LL/sin_herencia/python)

> [!tip]
> Adjunto en el laboratorio se encuentra [**Beginner's Python Cheat Sheet**](beginners_python_cheat_sheet_pcc_all.pdf) contiene un resumen completo de todo lo que se necesita para codificar programas en python. Tengalo a la mano, le facilitará la vida cuando este codificando en python.
 
## Actividad

Este laboratorio consiste en el desarrollo de algunos ejercicios en Python empleando scripts y notebooks de python.

### Problemas para codificar en un IDE

1. Complete los scripts de python que se encuentran dentro del directorio [`src`](src/) de acuerdo a las instrucciones que allí se dan empleando el IDE de su preferencia.
2. Refactorice el codigo del laboratorio 1 ([link](https://github.com/algoritmos-poli/lab1-repaso_POO)) reescribiendolo en lenguaje Python.

### Problemas para codificar en un Notebook

Empleando Jupyter Notebook o colab, resolver cada uno de los siguientes problemas. El notebook debe ser claro y contener una parte de texto donde se encuentre el enunciado del problema y una parte de código donde se muestre su solución en python. La siguiente tabla muestra los problemas por notebook:

|Notebook|Ejercicio|
|---|---|
|notebook1.ipynb|1,2,3|
|notebook2.ipynb|4,5|

A continuación se muestran los enunciados de los problemas:

1. **Grafico de barras**: Escriba un programa que solicite al usuario ingresar las ventas del día para cinco tiendas. El programa deberá mostrar un gráfico de barras que compare las ventas de cada tienda. Cree cada barra en el gráfico de barras mostrando una fila de asteriscos. Cada asterisco debe representar $100 en ventas.
   
   A continuación, se muestra un ejemplo de la salida del programa:

   ```
   Ingrese las ventas del día para la tienda 1: 1000 [Intro]
   Ingrese las ventas del día para la tienda 2: 1200 [Intro]
   Ingrese las ventas del día para la tienda 3: 1800 [Intro]
   Ingrese las ventas del día para la tienda 4: 800 [Intro]
   Ingrese las ventas del día para la tienda 5: 1900 [Intro]

   GRÁFICO DE BARRAS DE VENTAS
   Tienda 1: **********
   Tienda 2: ************
   Tienda 3: ******************
   Tienda 4: ********
   Tienda 5: *******************
   ```

2. **Cuadro de asteriscos**: Escriba un programa que solicite al usuario un número entero positivo no mayor a 15. A continuación, el programa deberá mostrar en pantalla un cuadrado utilizando el carácter `'X'`.
   
   El número ingresado por el usuario determinará la longitud de cada lado del cuadrado.
   
   Por ejemplo, si el usuario ingresa 5, el programa deberá mostrar lo siguiente:

   ```
   XXXXX
   XXXXX
   XXXXX
   XXXXX
   XXXXX
   ```

   Si el usuario ingresa 8, el programa deberá mostrar lo siguiente:

   ```
   XXXXXXXX
   XXXXXXXX
   XXXXXXXX
   XXXXXXXX
   XXXXXXXX
   XXXXXXXX
   XXXXXXXX
   XXXXXXXX
   ```

3. **Operaciones con arreglos**: Escriba un programa que contenga un arreglo inicializado con datos de prueba. Puede utilizar cualquier tipo de dato primitivo de su elección. El programa también deberá incluir las siguientes funciones:
   * **`getTotal`**: Esta función debe aceptar un arreglo unidimensional como argumento y devolver la suma total de los valores en el arreglo.
   * **`getAverage`**: Esta función debe aceptar un arreglo unidimensional como argumento y devolver el promedio de los valores en el arreglo.
   * **`getHighest`**: Esta función debe aceptar un arreglo unidimensional como argumento y devolver el valor más alto contenido en el arreglo.
   * **`getLowest`**: Esta función debe aceptar un arreglo unidimensional como argumento y devolver el valor más bajo contenido en el arreglo.
   
   Demuestre el funcionamiento de cada uno de los métodos en el programa. 

4. **Clase Empleado**: Escriba una clase llamada `Employee` que tenga los siguientes campos:
   * **`name`**: El campo `name` hace referencia a un objeto de tipo String que almacena el nombre del empleado.
   * **`idNumber`**: El campo `idNumber` es una variable de tipo int que almacena el número de identificación del empleado.
   * **`department`**: El campo `department` hace referencia a un objeto de tipo String que almacena el nombre del departamento donde trabaja el empleado.
   * **`position`**: El campo `position` hace referencia a un objeto de tipo String que almacena el cargo del empleado.

   La clase deberá un constructor que mermita pasar:
   * Los siguientes valores como argumentos y los asigne a los campos correspondientes: nombre del empleado, número de identificación, departamento y cargo.
   * Los siguientes valores como argumentos y los asigne a los campos correspondientes: nombre del empleado y número de identificación. A los campos department y position se les deberá asignar una cadena de texto vacía ("").
   * Cuando no se pasen argumentos que asigne cadenas de texto vacías ("") a los campos name, department y position, y el valor 0 al campo idNumber.

   Escriba los métodos mutadores (`setters`) apropiados para almacenar valores en estos campos, y los métodos accesores (`getters`) para devolver los valores de estos campos. Una vez que haya escrito la clase, desarrolle un programa aparte que cree tres objetos de tipo Employee para almacenar los siguientes datos:

   |Name|ID Number|Department|Position|
   |---|---|---|---|
   |Susan Meyers |47899| Contabilidad| Vicepresidente|
   |Mark Jones |39119| TI| Programador|
   |Joy Rogers|81774| Fabricación| Ingeniero|

   El programa deberá almacenar estos datos en los tres objetos y, posteriormente, mostrar en pantalla la información de cada empleado.

5. **Examen de Licencia de Conducir**: La Oficina de Licencias de Conducir local le ha solicitado escribir un programa que califique la parte escrita del examen de licencia de conducir. El examen consta de 20 preguntas de opción múltiple. A continuación se presentan las respuestas correctas:
   
   |Pregunta|Respuesta correcta|
   |---|---|
   |1|B|
   |2|D|
   |3|A|
   |4|A|
   |5|C|
   |6|A|
   |7|B|
   |8|A|
   |9|C|
   |10|D|
   |11|B|
   |12|C|
   |13|D|
   |14|A|
   |15|D|
   |16|C|
   |17|C|
   |18|B|
   |19|D|
   |20|A|

   Para aprobar el examen, un estudiante debe responder correctamente a 15 de las 20 preguntas.

   Escriba una clase llamada `DriverExam` que almacene las respuestas correctas del examen en un atributo de tipo `list`. La clase también deberá tener un atributo de tipo `list` que almacene las respuestas del estudiante. La clase deberá tener los siguientes métodos:
   * **`passed`**: Devuelve `true` si el estudiante aprobó el examen, o `false` si reprobó.
   * **`totalCorrect`**: Devuelve el número total de preguntas respondidas correctamente.
   * **`totalIncorrect`**: Devuelve el número total de preguntas respondidas incorrectamente.
   * **`questionsMissed`**: Un arreglo de tipo int que contenga los números de las preguntas que el estudiante respondió incorrectamente.
  
   Demuestre el uso de la clase en un programa completo que solicite al usuario ingresar las respuestas de un estudiante y que luego muestre los resultados devueltos por los métodos de la clase `DriverExam`.

   **Validación de entrada**: Acepte únicamente las letras `A`, `B`, `C` o `D` como respuestas.
