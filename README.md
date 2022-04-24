# Programateca: Guia de Ejercicios de Clase

Guía de Ejercicios de la materia Algoritmos y Programación UNIMET

**Authors**: Luis Eduardo Bello y Jose Roberto Quevedo

Tabla de contenidos

- [Programateca: Guia de Ejercicios de Clase](#programateca-guia-de-ejercicios-de-clase)
  - [1. Bienvenida](#1-bienvenida)
    - [C1E1](#c1e1)
  - [2. Command Line y Git](#2-command-line-y-git)
    - [C2E1](#c2e1)
    - [C2E2](#c2e2)
    - [C2E3](#c2e3)
  - [3. Tipos de datos, variables y operadores](#3-tipos-de-datos-variables-y-operadores)
    - [C3E1](#c3e1)
    - [C3E2](#c3e2)
    - [C3E](#c3e)
    - [C3E4](#c3e4)
  - [4. Expresiones lógicas, condicionales, funciones built-in de Python](#4-expresiones-lógicas-condicionales-funciones-built-in-de-python)
    - [C4E1](#c4e1)
    - [C4E2](#c4e2)
    - [C4E3](#c4e3)
    - [C4E4](#c4e4)
  - [5. Ciclos de repetición (While & For) y listas (arrays)](#5-ciclos-de-repetición-while--for-y-listas-arrays)
    - [C5E1](#c5e1)
    - [C5E2](#c5e2)
    - [C5E3](#c5e3)
    - [C5E4](#c5e4)
  - [6. List comprehension, tuplas & sets](#6-list-comprehension-tuplas--sets)
    - [C6E1](#c6e1)
    - [C6E2](#c6e2)
    - [C6E3](#c6e3)
  - [7. Diccionarios](#7-diccionarios)
    - [C7E1](#c7e1)
    - [C7E2](#c7e2)
    - [C7E3](#c7e3)
    - [C7E4](#c7e4)
  - [8. Estructuras de Datos Combinadas](#8-estructuras-de-datos-combinadas)
  - [9. Funciones](#9-funciones)
    - [C9E1](#c9e1)
    - [C9E2](#c9e2)
    - [C9E3](#c9e3)
    - [C9E4](#c9e4)
  - [10. Try Except, Funciones Lambda, módulos](#10-try-except-funciones-lambda-módulos)
    - [C10E1](#c10e1)
    - [C10E2](#c10e2)
    - [C10E3](#c10e3)
    - [C10E4](#c10e4)
    - [C10E5](#c10e5)
  - [12. Introducción a la programación orientada a objectos (POO): clases y objetos](#12-introducción-a-la-programación-orientada-a-objectos-poo-clases-y-objetos)
  - [13. POO: Herencia, composición y polimorfismo](#13-poo-herencia-composición-y-polimorfismo)
    - [C13E1](#c13e1)
  - [Clase 14: Manejo de archivos TXT](#clase-14-manejo-de-archivos-txt)
    - [C14E1](#c14e1)
    - [C14E2](#c14e2)
  - [Clase 15: Recursividad](#clase-15-recursividad)
    - [C15E1](#c15e1)
    - [C15E2](#c15e2)
    - [C15E3](#c15e3)

## 1. Bienvenida

### C1E1

Lee el tutorial en [Notion](#https://www.notion.so/algoritmosyprogramacionunimet/0-Getting-you-started-6fcccdb959ec42a7b0be15d84bd75181) sobre como configurar tu computadora para empezar el curso

---

## 2. Command Line y Git

### C2E1

En tu carpeta de elección crea un nuevo directorio (carpeta) llamada **programateca**, y ahí crea otro directorio llamado c1e1, en este último directorio crea 2 archivos README.md y main.py, en el README.md deberas replicar el [siguiente PDF](https://drive.google.com/file/d/1oFYEZbAb9n_C4Yi0bir8adBdActJR9Aj/view?usp=drivesdk) (para eso puede usar este [cheatsheet](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) de markdown que te explica como escribir Markdown), y en el main.py haz un programa que siga las instrucciones del README.

---

### C2E2

Inicializa un repositorio local en el directorio c1e1 (carpeta del ejercicio anterior), haz un commit con el ejercicio resuelto; Luego modifica el archivo main.py, sustituyendo el codigo por el siguiente:

```python
name = "Tu nombre aqui (con las comillas)"
age = "Tu edad aqui (sin las comillas)"
career = "Tu carrera aqui (con las comillas)"
print(f"Hola Mundo! mi nombre es {name} y tengo {age}
años, estudio {career} en la UNIMET!")
```

Luego en Github crea un repositorio público y enlaza el repositorio local con el repositorio de Github, por último sube los cambios a Github

---

### C2E3

Crea un repositorio público en Github llamado c1e3 y clónalo vacío en tu carpeta de **programateca**, luego ya en tu computadora y con el uso del command line ve al directorio de c1e3 que clonaste y crea una carpeta por cada materia que estés viendo, ejemplo: algoritmos, física, matemáticas, y dentro de cada carpeta de cada materia tendrás que crear un archivo txt (ejemplo: `touch algoritmos.txt`) con las evaluaciones, fechas y porcentajes de esa materia, Ejemplo:

algoritmos.txt:

```text
Algoritmos y Programación
Quiz -    10%    - Semana 5
Examen I    - 20%     - Semana 7
Trabajo I    - 5%    - Semana 7
Trabajo II    - 5%    - Semana 10
Examen II    - 30%    - Semana 11
Proyecto    - 30% - Semana    12
```

Y así con todas las materias, por cada archivo txt haz un commit a medida que lo vayas creando y súbelo a Github

---

## 3. Tipos de datos, variables y operadores

### C3E1

1. disminuir la variable de lluvia en un 10% para tener en cuenta el agua de lluvia que circula libremente sobre la superficie de un terreno.
2. Agregue la variable de lluvia a la variable volumen_reservorio.
3. Aumentar volumen_reservorio en un 5% para tener en cuenta las aguas pluviales que fluyen en el embalse en los días posteriores a la tormenta.
4. Disminuir volumen_reservorio en un 2% para tener en cuenta la evaporación.
5. Resta 2.5e5 metros cúbicos de volumen_reservorio para tener en cuenta el agua que se canaliza a regiones áridas.
6. Imprime el nuevo valor de la variable volumen_reservorio.

**Nota:** Aquí usaremos notación científica para definir grandes números.

4.445e8 <=> 4.445 \* 10 \*\* 8 <=> 444500000.0

---

### C3E2

Se le proporcionarán datos de ejemplo para un usuario:

- La hora de su visita
- El sitio web al que accedió.

Debe usar las variables proporcionadas y las técnicas que ha aprendido para imprimir un mensaje de registro como este (con el nombre de usuario, la URL y la marca de tiempo reemplazados por valores de las variables apropiadas)

**Output:**

```shell
Ana ingreso al sitio https://petshop.com/pets/reptiles/pythons a las 07:00A.M.
```

---

### C3E

**Nota**: Usar archivo e3.py

Escribe un programa en donde pidas por teclado el nombre y el año de nacimiento de la persona y muestre como resultado el siguiente mensaje:

```shell
{nombre} debe cumplir o cumplio {edad} años este año
```

---

### C3E4

Escriba un programa que reciba por teclado los números a y b y encuentre el valor de c que satisfaga el teorema de pitágoras.

**Nota:** El teorema de pitágoras establece que

![Teorema de pitagoras](https://latex.codecogs.com/png.latex?%5Cdpi%7B150%7D%20%5CLARGE%20c%5E2%20%3D%20a%5E2%20+%20b%5E2)

---

## 4. Expresiones lógicas, condicionales, funciones built-in de Python

### C4E1

Realizar un programa donde se reciba un número flotante por teclado e imprima un mensaje diciendo si el número es par o impar y evaluar si es positivo/negativo.

**Output:**

```shell
El número: **X** es par/impar y positivo/negativo
```

Donde **X** es el número ingresado por teclado.

---

### C4E2

Una famosa cadena de cines en Venezuela te contrató para hacerles un programa de descuento en las entradas basado en la edad del cliente, para ello tendrás que recibir por teclado la edad y nombre del cliente y verificar los siguientes casos:

- Si su edad es menor o igual a 4 años el precio de su entrada es gratis.
- Si su edad es menor o igual a 18 años el precio de su entrada es de $1.50
- Si su edad es mayor o igual a los 60 años su entrada tendrá un valor de $1
- La entrada para un adulto promedio es de $2.00

Deberás imprimir un mensaje dependiendo de la edad del cliente para saber el precio de su entrada.

**Output:**

```shell
El cliente: {nombre} tiene: {edad} años y su entrada de cine cuesta: ${precio_entrada}
```

---

### C4E3

Te contrataron para realizar un programa donde calcule el premio de un juego.

Los premios son basados en puntos:

| Puntos  | Premio        |
| ------- | ------------- |
| 1-50    | No hay premio |
| 51-150  | Bronze        |
| 151-180 | Plata         |
| 181-200 | Oro           |

Todos los límites inferior y superior aquí son inclusivos, y los puntos solo pueden tomar valores enteros positivos hasta 200.

En su declaración **if**, asigne la variable de resultado a un String que contenga el mensaje apropiado según el valor de los puntos.

Si ganaron un premio, el mensaje debería decir:

**Output:**

```python
 "Felicitaciones, Ganaste la medalla de {nombre del premio} por haber tenido {puntos} pts!"
```

Si no hay premio, el mensaje debe decir:

**Output:**

```python
 "No hay premios para {puntos} pts"
```

---

### C4E4

Desarrolla en Python el juego de _Piedra, Papel y Tijeras_ en donde pediras por teclado la opción del jugador 1, luego la opción del jugador 2, y posteriormente dará el resultado diciendo quien gano.

---

## 5. Ciclos de repetición (While & For) y listas (arrays)

---

### C5E1

**1.1** Use un for loop para tomar la lista que se llama 'oracion' e imprima cada elemento de la lista en su propia línea.

**Output:**

```shell
Estoy
```

```shell
imprimiendo
```

```shell
una
```

```shell
lista
```

```shell
linea
```

```shell
por
```

```shell
linea
```

**1.2** Escribe un for loop que imprima números enteros multiples de 5 menores e iguales a 30.

**Output:**

```shell
5
```

```shell
10
```

```shell
15
```

```shell
20
```

```shell
25
```

```shell
30
```

---

### C5E2

**2.1**

Escribe un For Loop que itere sobre la lista 'estudiantes' y crea una lista 'usernames' para cada nombre. Para crear un username debes:

- Colocar todo el nombre en minúscula.
- Remplaza los espacios con guion bajo " \_ ".

**Output:**

```python
["Elijah Evans", "Charissa Mueller", "Kirby Park",
     "Jescie Hill",
     "Leroy Herring",
     "Francis Castaneda",
     "Bree Gregory",
     "Kermit Stevens",
     "Jordan Terry",
     "Paul Trujillo",
     "Linda Beck",
     "Dara Mckinney",
     "Idola Pearson",
     "Phelan Vazquez",
     "Cleo Dyer",
     "Kameko Mccall",
     "Kitra Tillman",
     "Oren Miles",
     "Martin Kerr",
     "Orlando Noble",
     "Ferdinand Carr",
     "Scott Norman",
     "Autumn Winters",
     "Phillip Heath",
     "Ryder Mueller",
     "Armand Lucas",
     "Naida Hart",
     "Deborah Spencer",
     "Blythe Kidd",
     "Colleen Keller"]
```

**Pista:** Puedes remplazar los espacios con el método .replace(), para saber como funciona chequea esta documentación:

`https://www.w3schools.com/python/ref_string_replace.asp`

**2.2**

Ahora en vez de crear una nueva lista, queremos actualizar la lista existente llamada estudiantes. Mismo Output.

---

### C5E3

Debe escribir un while Loop que tome los números en una lista dada llamada: `num_list`

```python
num_list = [422, 136, 524, 84, 96, 719, 85, 92, 10, 17, 312, 542,
            86, 24, 86, 190, 116, 36, 174, 46, 150, 58, 84, 60, 114, 167]
```

Su código debe **sumar** los números impares en la lista, pero solo hasta los primeros 5 números impares.

- Sumar los primeros 5 números impares en la lista.
- Si hay mas de 5 números impares, detenerse de sumar en el 5to número y mostrar mensaje con la cantidad de números impares y la suma total.

**Output:**

```python
"La cantidad de números impares es: {contador_impares}"
"La suma total de los números impares es: {suma_impares}"
```

---

### C5E4

Desarrolla un programa que permita calcular el cuadrado mas cercano a un numero,ejemplo: el cuadrado mas cercano de **40** es 36 (ya que 6\*6)

---

## 6. List comprehension, tuplas & sets

---

### C6E1

**1.1**

```python
nombres = ["Elijah Evans", "Charissa Mueller", "Kirby Park",
               "Jescie Hill",
               "Leroy Herring",
               "Francis Castaneda",
               "Bree Gregory",
               "Kermit Stevens",
               "Jordan Terry",
               "Paul Trujillo",
               "Linda Beck",
               "Dara Mckinney",
               "Idola Pearson",
               "Phelan Vazquez",
               "Cleo Dyer",
               "Kameko Mccall",
               "Kitra Tillman",
               "Oren Miles",
               "Martin Kerr",
               "Orlando Noble",
               "Ferdinand Carr",
               "Scott Norman",
               "Autumn Winters",
               "Phillip Heath",
               "Ryder Mueller",
               "Armand Lucas",
               "Naida Hart",
               "Deborah Spencer",
               "Blythe Kidd",
               "Colleen Keller"]
```

Use una comprensión de la lista para crear una nueva lista primeros_nombres que contenga solo los primeros nombres en minúsculas.

**Output esperado:**

```python
['elijah', 'charissa', 'kirby', 'jescie', 'leroy', 'francis', 'bree', 'kermit', 'jordan', 'paul', 'linda', 'dara', 'idola', 'phelan', 'cleo', 'kameko', 'kitra', 'oren', 'martin', 'orlando', 'ferdinand', 'scott', 'autumn', 'phillip', 'ryder', 'armand', 'naida', 'deborah', 'blythe', 'colleen']
```

**1.2.**

Use una comprensión de lista para crear una lista multiplos_3 que contenga los primeros 20 múltiplos de 3.

**Output esperado:**

```python
[3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 33, 36, 39, 42, 45, 48, 51, 54, 57, 60]

```

---

### C6E2

**2.1.**

Usa zip para escribir un bucle **for** que cree una lista que especifique el label y las coordenadas de cada punto. Cada elemento debe formatearse como:

**Output**

```python
 {label}: x, y, z.
```

Por ejemplo:

```shell
 F: 23, 677, 4.
```

**2.2.**

Usa enumerate para modificar la lista de casting para que cada elemento contenga el nombre seguido de la altura correspondiente del personaje.

Por ejemplo, el primer elemento del elenco debería cambiar de "Barney Stinson" a "Barney Stinson 72".

---

### C6E3

**3.1**

Determine cuales son los elementos iguales entre dos listas.

**nota**: Revise el método _[intersection](https://www.w3schools.com/python/ref_set_intersection.asp)_

**3.2**

Realice un programa que le pida al usuario una palabra y determine cual vocales contiene dicha palabra.

Output:

```shell
La palabra {output} tiene a las vocales {vowels}
```

---

## 7. Diccionarios

### C7E1

Cuenta la cantidad de frutas en su cesta. Para hacer esto, tiene el diccionario y la lista de frutas. Use el diccionario y la lista para contar el número total de frutas y los otros artículos que no son frutas en su cesta.

**Output**

```python
Hay {} frutas en la cesta. y {} objetos que no son frutas.
```

---

### C7E2

Podemos crear un diccionario, contador, que realiza un seguimiento del recuento total de cada palabra en la lista quote.

**Output:**

```python
`{'Tienes': 1, 'que': 1, 'bailar': 1, 'como': 4, 'si': 4, 'no': 2, 'hubiera': 2, 'nadie': 2, 'mirando': 1, 'Ama': 1, 'nunca': 1, 'te': 1, 'lastimaran': 1, 'Canta': 1, 'escuchando': 1,'Y': 1, 'vive': 1, 'fuera': 1, 'el': 1, 'cielo': 1, 'en': 1,'la': 1, 'tierra.': 1}`
```

---

### C7E3

Encuentre las letras repetidas dentro de una palabra

**Output:**

```shell
La palabra {word} contiene a las letras {letters} repetidas
```

---

### C7E4

Determine si la representación binaria de dos números son anagramas

_Un anagrama es un procedimiento que consiste en crear una palabra a partir de la reordenación de las letras de otra palabra._

**Ejemplo:**

```python
a = 8 # 1000
b = 4 # 0100
c = 5 # 0110
d = 4 # 0100
```

**Output:**

```shell
Los números {a} y {b} son un anagrama
```

**Pista**: Utilice la función _[bin](https://www.programiz.com/python-programming/methods/built-in/bin)_

---

## 8. Estructuras de Datos Combinadas

---

**C8E1**

Le han dado una lista de _k_ listas, cada una de las listas esta ordenada de manera ascendente. Combine las _k_ listas en una sola lista ordenada y retorne dicha lista.

**Input:**

```python
lists = [[1,4,5],[1,3,4],[2,6]]
```

**Output:**

```python
[1,1,2,3,4,4,5,6]
```

---

**C8E2**

Dada la lista _orders_, que representa las ordenes que ciertos clientes han hecho en un restaurante. Específicamente, `orders[i] = [customer_name,table_number,food_item]`

Imprima la tabla _display_table_, que es una tabla cuyas filas denotan cuantos items de comida cada mesa ha ordenado, en donde, la primera columna es el número de la mesa y el resto de las columnas corresponden al nombre de los platos ordenados alfabéticamente. La primera fila debe ser el encabezado de la tabla.

**Input:**

```python
orders = [
    ["David", "3", "Ceviche"],
    ["Corina", "10", "Beef Burrito"],
    ["David", "3", "Fried Chicken"],
    ["Carla", "5", "Water"],
    ["Carla", "5", "Ceviche"],
    ["Rous", "3", "Ceviche"]
  ]
```

**Output:**

```python
[
  ["Table","Beef Burrito","Ceviche","Fried Chicken","Water"],
  ["3","0","2","1","0"],
  ["5","0","1","0","1"],
  ["10","1","0","0","0"]
]
```

**C8E3**

Dada la lista _students_ que es una lista de diccionario, calcule el promedio de notas de los estudiantes y determine cual es el estudiante con mayor nota dentro del grupo.

**Input**:

```python
student = [
  {
    "name": "Jose",
    "grade": 16
  },
  {
    "name": "Luis",
    "grade": 17
  },
  {
    "name": "Antonio",
    "grade": 14
  },
  {
    "name": "Gabrielle",
    "grade": 12,
  },
  {
    "name": "Alejandro",
    "grade": 11,
  }
]
```

**Output**:

```python
"El promedio de notas es: 14.0ptos"
"El estudiante con mayor nota es Luis con 17ptos"
```

---

**C8e4**

Realice una calculadora de vectores, la entrada de esta será una lista de tuplas, suponga que cada tupla de la lista es un vector, realice las operaciones de suma, resta y producto punto.

**Input:**

```python
vectors = [
  (1, 7, 2),
  (2, 3, 5)
]
```

**Output:**

```python
"El vector suma es: (3, 10, 7)"
"El vector resta es: (-1, 4, -3)"
"El producto punto es: 33"
```

---

## 9. Funciones

### C9E1

Elabore una función que dado un número determine si es un número primo o no

**Output:**

```python
print(is_prime(2)) # True
print(is_prime(6)) # False
```

---

### C9E2

Realice un función que dado una lista de números `nums`, para cada número _i_ (`nums[i]`) determine cuantos números dentro de la lista son menores que el, es decir, para cada `nums[i]` debe contar los números `nums[j]` tal que `nums[j] < nums[i]` y `j!=i`. Debe regresar su respuesta como otra lista.

**Input:**

```python
nums = [8,1,2,2,3]
```

**Output:**

```python
print(count_smaller(nums)) # [4,0,1,1,3]
```

---

### C9E3

Realice una función que haga un registro de los datos de los pacientes de un consultorio médico y los guarde dentro de una lista que la función deberá devolver. Los datos que deberá solicitar son:

1. Número de cédula
2. Nombre
3. Apellido
4. Teléfono
5. Razón de consulta

### C9E4

Escriba una función llamada leer_tiempo.

La función debe tomar **un** argumento, un número entero y **devolver** un **string** que indique cuántas semanas y días son.

Por ejemplo, llamando a la función e imprimiendo el resultado de esta manera:

```
`print(`leer_tiempo`(10))`
```

`Debe dar como **Output:**`

```
`1 semana(s) y 3 dias(s).`
```

---

## 10. Try Except, Funciones Lambda, módulos

### C10E1

Realice una función _lambda_ que reciba dos pares ordenado `(x,y)` y determine la distancia entre los puntos. La distancia entre dos puntos se calcula utilizando la ecuación:

![distancia](https://latex.codecogs.com/png.latex?%5Cdpi%7B120%7D%20%5Chuge%20d%20%3D%20%5Csqrt%7B%28x_2-x_1%29%5E2%20+%20%28y_2%20-%20y_1%29%5E2%7D)

---

### C10E2

Desarrolle una función que pueda castear un string a un número flotante, considerando que el separador por defecto es `.` puede puede ser `,`.

**Input:**

```python
num = parse_float('1,9') # 1.9
num = parse_float('2.3') # 2.3
num = parse_float('Error') # Exception
```

---

### C10E3

Desarrolle un archivo _utils_ en donde se encuentren las funciones: `get_costumer_information`, `add_to_basket`, `calculate_subtotal` y `calculate_tax`, estas funciones servirán de apoyo al código principal para desarrollar un programa que le permita al usuario ingresar su información de facturación, escoger productos de un menú y luego informarle el total sobre su compra.

---

### C10E4

**C10E4.1**

map(<funcion, List[]>) es una función de Python que toma como parámetros una función y una lista, este retorna una lista con el que se le aplico la función pasada como parámetro a cada elemento de lista.

Usa map() para encontrar la media de cada elemento en la lista 'numeros' y crear una nueva lista llamada promedios.

Puedes leer más sobre map() aquí:

<https://www.w3schools.com/python/ref_func_map.asp>

**Nota:** Para este ejercicio es obligatorio aplicar el uso de lambda expressions en Python.

**Output esperado:**

```
[57.0, 58.2, 50.6, 27.2]
```

**C10E4.2**

filter(<funcion, list[]>) es una función de Python que toma como parámetros una función y una lista, este retorna una lista con el que se le aplico la función pasada como parámetro a cada elemento de lista y solo se insertan aquellos elementos que cumplen con la condición.

Usa filter() para obtener los nombres en ciudades que tienen menos de 8 caracteres y crea una nueva lista llamada ciudades_pequenas[]

Puedes leer más sobre filter() aquí:

<https://www.w3schools.com/python/ref_func_filter.asp>

**Nota:** Para este ejercicio es obligatorio aplicar el uso de lambda expressions en Python.

**Output esperado:**

```
['Caracas', 'Barinas']
```

---

### C10E5

Escriba una función llamada generar_contrasena que seleccione tres palabras aleatorias de la lista lista_palabras[] y las concatene en un solo String. Su función no debe aceptar ningún argumento y debe hacer referencia a la variable global lista_palabras para crear la contraseña.

Puedes usar una funcion de la librería random llamada choice para encontrar un elemento aleatorio de una secuencia no vacía. Más información en el link debajo:

<https://docs.python.org/3.7/library/random.html?highlight=choice>

---

## 12. Introducción a la programación orientada a objectos (POO): clases y objetos

---

## 13. POO: Herencia, composición y polimorfismo

### C13E1

Te han contratado en Saman-Train🚉, esta línea compañía desea llevar el control de las horas de su personal para su respectivo pago; para esto, una vez que el personal se presta a dar servicio, se toman los siguientes datos: cédula del personal, tipo de tren Supersónico o Carbón, y el número de horas de trabajo. Dependiendo de las horas se les paga al personal.

| Tipo de Tren | Sueldo por hora |
| :----------: | :-------------: |
| Supersónico  |       60        |
|    Carbón    |       30        |

Usted deberá desarrollar un programa utilizando POO de forma de producir un output que contenga lo siguiente:

Para cada personal:

- Cédula de Identidad del personal
- Tipo de tren
- Monto Total a ser pagado al personal. Si el personal toma más de 8 horas de trabajo, se le otorgará un aumento del 30% sobre el monto total a pagar en caso de que sea supersonico y 35% en caso de que sea carbón.

Al final del día para la Samán Train:

- La cantidad total de personal con su información
- La cantidad de personal por tipo de tren
- La cantidad de personal a quienes se les otorgó el aumento
- El Promedio de pago por tipo de tren


## Clase 14: Manejo de archivos TXT

### C14E1

Se te ha proporcionado la letra de una canción en el documento txt original en donde fue escrita,  pero el archivo esta corrupto, debes:

1.1. Agrega a una lista llamada 'letra' en donde cada posición debe ser una linea de la canción.

1.2. Luego en la lista debes sustituir

- @ por a
- 3 por r
- 0 por o

1.3. Por último imprime la lista letra, linea por linea.

---

### C14E2

Vas a crear un documento  del cast que aparecieron en el programa de televisión **Flying Circus de Monty Python** (esta información se recopiló de imdb.com). Para eso debes:

1. Escribir una función, que tome como parámetros el nombre del archivo 'flying_circus_cast' y retorna una lista con solo los nombres de los actores. Cada línea de ese archivo consiste en el nombre de un actor, una coma y luego información (desordenada) sobre los roles que desempeñaron en el programa.

2. Luego debes escribir otra función que tome la lista anteriormente creada y escribir en un nuevo archivo los nombre de los actores linea por linea.

--
## Clase 15: Recursividad

### C15E1

Podemos definir la sumatoria de un numero x si:  (1 + 2 + ... + x) para un entero x ≥ 1:

Complete el siguiente programa de Python para calcular la suma: ej de 10 seria:  1 + 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9 + 10

**Output esperado:**

```
55
```

Tiene que ser de forma **recursiva**.

---

### C15E2

Podemos determinar cuántos dígitos tiene un número entero positivo dividiendo repetidamente entre 10 (sin conservar el resto) hasta que el número sea menor que 10, que consta de solo 1 dígito.

Sumamos 1 a este valor por cada vez que dividimos entre 10.

Este seria el algoritmo recursivo:

1. Si n <10 retorna 1.

2. De lo contrario, devuelva 1 + el número de dígitos en

n / 10 (ignorando el resto).

Implemente este algoritmo recursivo en Python y pruébelo usando una función main que llame a esta función  con los parámetros de 15, 105 y 15105 (Puedes pedir el valor por teclado).

**Nota**: Recuerde que si n es un número entero, n / 10 será un número entero sin el resto.

---

### C15E3

Escribe una función recursiva de Python que recibe un parámetro que representa una lista de enteros y devuelve el máximo numero en la lista.

El algoritmo debe realizarse de la siguiente manera, el máximo será el primer valor de la lista (indice 0) o el máximo del resto de la lista (indice 1 al -1).

Si la lista solo tiene 1 entero, entonces su máximo es este valor único, naturalmente.

Algoritmo puede verse como:

Si A es una lista de enteros, y desea establecer la lista B para todos los enteros en A excepto el primero, puede escribir:

B = A [1: len (A)]

(Esto establece B en los enteros en A que comienzan en el índice 1 y terminan en el índice len(A) -1, el último índice.
