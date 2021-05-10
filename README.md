# Programateca: AyP 

Guía de Ejercicios de la materia Algoritmos y Programación UNIMET

**Author**: Luis Eduardo Bello

## Tabla de contenidos
1. [Command Line y Git](#command-line-y-git)
2. [Variables, Operadores y Strings](#variables-operadores-y-strings)
3. [Listas y Ciclos](#listas-y-ciclos)
4. [List comprehension, set & tuplas](#list-comprehension-set-y-tuplas)
5. [Diccionarios](#diccionarios)
6. [Funciones](#funciones)
7. [Comming soon...](#tabla-de-contenidos)


## Command Line y Git

---
**C1E1**

En tu carpeta de elección crea un nuevo directorio (carpeta) llamada **programateca**, y ahí crea otro directorio llamado c1e1, en este último directorio crea 2 archivos README.md y main.py, en el README.md deberas replicar el [siguiente PDF](https://drive.google.com/file/d/1oFYEZbAb9n_C4Yi0bir8adBdActJR9Aj/view?usp=drivesdk) (para eso puede usar este [cheatsheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf) de markdown que te explica como escribir Markdown), y en el main.py haz un programa que siga las instrucciones del README.

---
**C1E2**

Inicializa un repositorio local en el directorio c1e1 (carpeta del ejercicio anterior), haz un commit con el ejercicio resuelto; Luego modifica el archivo main.py, sustituyendo el codigo por el siguiente: 

```
name = "Tu nombre aqui (con las comillas)"
age = "Tu edad aqui (sin las comillas)"
career = "Tu carrera aqui (con las comillas)"
print(f"Hola Mundo! mi nombre es {name} y tengo {age}
años, estudio {career} en la UNIMET!")
```

Luego en Github crea un repositorio público  y enlaza el repositorio local con el repositorio de Github, por último sube los cambios a Github

---
**C1E3**

Crea un repositorio público en Github llamado c1e3 y clónalo vacío en tu carpeta de **programateca**, luego ya en tu computadora y con el uso del command line ve al directorio de c1e3 que clonaste y crea una carpeta por cada materia que estés viendo, ejemplo: algoritmos, física, matemáticas, y dentro de cada carpeta de cada materia tendrás que crear un archivo txt (ejemplo: `touch algoritmos.txt`) con las evaluaciones, fechas y porcentajes de esa materia, Ejemplo:

algoritmos.txt:

```
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


## Variables, Operadores y Strings

---
**C2E1**

Te han contrado en el centro meteorologico de la **NASA**, para que hagas ciertos calculos tomando en cuenta lo siguiente:  

- El volumen actual de un depósito de agua (en metros cúbicos)
`volumen_reservorio = 4.445e8`

- La cantidad de lluvia de una tormenta (en metros cúbicos)
`lluvia = 5e6`

Debes hacer los siguientes calculos:
- Disminuir la variable de lluvia en un 10% para tener en cuenta el agua de lluvia que circula libremente sobre la superficie de un terreno ✍️
- Agregue la variable de lluvia a la variable volumen_reservorio ✍️
- Aumentar volumen_reservorio en un 5% para tener en cuenta las aguas pluviales que fluyen en el embalse en los días posteriores a la tormenta ✍️
- Disminuir volumen_reservorio en un 2% para tener en cuenta la evaporación ✍️
- Resta 2.5e5 metros cúbicos de volumen_reservorio para tener en cuenta el agua que se canaliza a regiones áridas. ✍️
- Imprime el nuevo valor de la variable volumen_reservorio, con el mensaje: `"El volumen del reservorio es {volumen_reservorio}m3"` ✍️

**Nota**: 
Aqui usaramos notación científica para definir grandes números. 

4.445e8 <=> 4.445 * 10 ** 8 <=> 444500000.0

---
**C2E2**

Se le proporcionarán datos de ejemplo para un usuario, la hora de su visita y el sitio al que accedió.

 Debe usar las variables proporcionadas y las técnicas que ha aprendido para imprimir un mensaje de registro como este (con el nombre de usuario, la URL y la marca de tiempo reemplazados por valores de las variables apropiadas):

**Output**:

```
Ana ingreso al sitio https://petshop.com/pets/reptiles/pythons a las 07:00A.M.
```
**Starter Code**:

```
username = "Ana"
timestamp = "07:00"
url = "https://petshop.com/pets/reptiles/pythons"

# TODO: Hacer print usando las variables de arriba igual
# como aparace en el Output arriba ✍️
```

---

## Condicionales

---
**C3E1**

Realizar un programa donde se reciba un número por teclado e imprima un mensaje diciendo si el número es par o impar.

**Output:**

```
El número: **X** es par/impar
```

Donde  _X_  es el número ingresado por teclado.

**Bonus** en el mismo mensaje decir si el número es positivo o negativo

**Output:**

```
El número: **X** es par/impar y positivo/negativo
```

--- 
**C3E2**

Una famosa cadena de cines en Venezuela te contrató para hacerles un programa de descuento en las entradas basado en la edad del cliente, para ello tendrás que recibir por teclado la edad y nombre del cliente y verificar los siguientes casos:

- Si su edad es menor o igual a 4 años el precio de su entrada es gratis.
- Si su edad es menor o igual a 18 años el precio de su entrada es de $1.50
- Si su edad es mayor o igual a los 60 años su entrada tendrá un valor de $1
- La entrada para un adulto promedio es de $2.00

Deberas imprimir un mensaje dependiendo de la edad del cliente para saber el precio de su entrada.

**Output:**

```
El cliente: {nombre} tiene: {edad} años y su entrada de cine cuesta: ${precio_entrada}
```

---
**C3E3**

Te contrataron para realizar un programa donde calcule el premio de un juego.

Los premios son basados en puntos:

| **Puntos** | **Premio**    |
| ---------- | ----------    |
| 1-50       | No hay premio |
| 51-150     | Bronze        |
| 151-180    | Plata         |
| 181-200    | Oro           | 

Todos los límites inferior y superior aquí son inclusivos, y los puntos solo pueden tomar valores enteros positivos hasta 200.

En su declaración **if**, asigne la variable de resultado a un String que contenga el mensaje apropiado según el valor de los puntos. 

Si ganaron un premio, el mensaje debería decir:

**Output:**

```
 "Felicitaciones, Ganaste la medalla de {nombre_del_premio} por haber tenido {puntos} pts!"
```

Si no hay premio, el mensaje debe decir:

**Output:**

```
 "No hay premios para {puntos} pts"
```

## Listas y Ciclos

---

**C4E1**

Use un for loop para tomar la lista que se llama 'oracion' e imprima cada elemento de la lista en su propia línea.

**Output:**

```
Estoy
```

```
imprimiendo
```

```
una
```

```
lista
```

```
linea
```

```
por
```

```
linea
```

**Starter Code**
```
oracion = ["Estoy","imprimiendo","una","lista","linea","por","linea"]
```

---
**C3E2**

Escribe un for loop que imprima números enteros multiples de 5 menores e iguales a 30.

**Output:**

```
5
```

```
10
```

```
15
```

```
20
```

```
25
```

```
30
```

---
**C4E3**

a. Escribe un For Loop que itere sobre la lista 'estudiantes' y crea una lista 'usernames' para cada nombre. Para crear un username debes:

- Colocar todo el nombre en minúscula.
- Remplaza los espacios con guion bajo " _ ".


**Output:**
```
['emmie_grey', 'andre_hills', 'gurpreet_atherton', 'johan_stewart', 'joseff_hurst', 'margot_conrad', 'matteo_whitaker', 'mekhi_hussain', 'sherry_macdonald', 'mathew_cano', "cara_o'moore", 'kush_gonzalez', 'soren_clark', 'inaayah_broadhurst', 'ruth_lawrence', 'nafisa_nairn', 'zachariah_velasquez']
```

**Starter Code** :
```
students = ["Emmie Grey",
"Andre Hills",
"Gurpreet Atherton",
"Johan Stewart",
"Joseff Hurst",
"Margot Conrad",
"Matteo Whitaker",
"Mekhi Hussain",
"Sherry Macdonald",
"Mathew Cano",
"Cara O'Moore",
"Kush Gonzalez",
"Soren Clark",
"Inaayah Broadhurst",
"Ruth Lawrence",
"Nafisa Nairn",
"Zachariah Velasquez"]
```


**Pista:** Puedes remplazar los espacios con el método .replace(), para saber como funciona chequea esta documentación:


[https://www.w3schools.com/python/ref_string_replace.asp](https://www.w3schools.com/python/ref_string_replace.asp)


b. Ahora en vez de crear una nueva lista, queremos actualizar la lista existente students con el mismo Output

---
**C4E4**

Debe escribir un While Loop que tome los números en una lista dada llamada: `num_list`

Su código debe **sumar** los números impares en la lista, pero solo hasta los primeros 5 números impares.

- Sumar los primeros 5 números impares en la lista.
- Si hay mas de 5 números impares, detenerse de sumar en el 5to número y mostrar mensaje con la cantidad de números impares y la suma total.

**Starter Code**:
```
num_list = [422, 136, 524, 85, 96, 719, 85, 92, 10, 17, 312, 542, 87, 23, 86, 191, 116, 35, 173, 45, 149, 59, 84, 69 , 113, 166]
```


**Output**:
```
"La cantidad de números impares es: {contador_impares}"
"La suma total de los números impares es: {suma_impares}"
```

---
**C4E5**


Los números primos son números enteros que pueden ser divisibles entre: 1 y si mismo. Los primeros números primos son 2, 3, 5, 7.

Por ejemplo, 6 es divisible por cuatro números : 1, 2, 3, 6.

1 X 6 = 6

2 X 3 = 6

Entonces sabemos que 6 **no** es un número primo.

Escribe un programa para verificar si los números provistos en la lista chequear_primos son números primos.

**Output:**

Si los números son primos, el código debe imprimir:

```
{número} es un número primo
```

Si el número **NO** es un número primo, debe imprimir:

```
`{número} no es un número primo, porque {numero} es divisible entre {divisible}`
```

---
**C4E6**

Escriba un programa que itere los enteros del 0 al 50. 

- Para múltiplos de tres imprima "**Fizz**" en lugar del número
- Para los múltiplos de cinco imprima "**Buzz**".
- Para números que son múltiplos de tres y cinco, imprime "**FizzBuzz**". 
- Para el resto de los números imprima el número.

---
**C4E7**


Una famosa cadena de noticias te contrato para que diseñaras un programa el cual muestre los titulares en Twitter, sin embargo esta plataforma limita los tweets a 140 caracteres.

Escribe un **Loop** con **Break** en donde recorras la lista `titulares` dada, y en cada iteración inserta los titulares en una variable `tweet`. 
Tienes que tomar en cuenta lo siguiente:

- Al concatenar los strings a la variable `tweet` ten en cuenta el espacio que debes dejar entre titulares y separarlos por coma ','.
- Si es necesario tienes que truncar los titulares para que queden exactamente 140 caracteres en la variable `tweet`

**Input**
```
# Variables a usar.
titulares = ["Oso se come a hombre en el Avila",
             "Anuncian nuevas leyes para la nación",
             "Si lees esto, estudia los resumenes de clase para el Quiz ;)",
             "Gato rescata a bombero atrapado en un árbol",
             "La UNIMET tiene nueva cancha de fútbol",
             "Los estudiantes de algoritmos y programción son los mejores!"]
```

**Output:**

```
`Oso se come a hombre en el Avila, Anuncian nuevas leyes para la nación, Si lees esto, estudia los resumenes de clase para elQuiz ;), Gato r`
```

**Hints:**

Al igual que las listas los String se pueden usar **`slice()`**, donde cada carácter se puede asimilar como una posición en una lista/vector.

nombre = "Juan Pablo"

print(nombre[0] ) # output= J

print(nombre[0:4]) # output= Juan

Si quieres saber más sobre **slice** te dejo este link de referencia:


[https://www.w3schools.com/python/showpython.asp?filename=demo_string2](https://www.w3schools.com/python/showpython.asp?filename=demo_string2)


---

## List comprehension, set y tuplas

---
**C6E1**


a. Use **List comprehension** para crear una nueva lista primeros_nombres que contenga solo los primeros nombres en minúsculas de la lista estudiantes.

**Starter Code**
```
estudiantes = ["Emmie Grey",
"Andre Hills",
"Gurpreet Atherton",
"Johan Stewart",
"Joseff Hurst",
"Margot Conrad",
"Matteo Whitaker",
"Mekhi Hussain",
"Sherry Macdonald",
"Mathew Cano",
"Cara O'Moore",
"Kush Gonzalez",
"Soren Clark",
"Inaayah Broadhurst",
"Ruth Lawrence",
"Nafisa Nairn",
"Zachariah Velasquez"]
```


**Output esperado:**
```
['emmie', 'andre', 'gurpreet', 'johan', 'joseff', 'margot', 'matteo', 'mekhi', 'sherry', 'mathew', 'cara', 'kush', 'soren', 'inaayah', 'ruth', 'nafisa', 'zachariah']
```


b. Use un **List comprehension** para crear una lista multiplos_3 que contenga los primeros 20 múltiplos de 3.

**Output**:

```
[3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 33, 36, 39, 42, 45, 48, 51, 54, 57, 60]
```


---
**C6E2**

a. Usa zip para escribir un bucle **for** que cree una lista que especifique el label y las coordenadas de cada punto. Cada elemento debe formatearse como:

**Output**

```
 {label}: x, y, z.
```

 Por ejemplo:

```
 F: 23, 677, 4.
```

b.Usa enumerate para modificar la lista de casting para que cada elemento contenga el nombre seguido de la altura correspondiente del personaje. 

Por ejemplo, el primer elemento del elenco debería cambiar de "Barney Stinson" a "Barney Stinson 72".

---
**C6E3**

Dada un String de caracteres en minúscula. La tarea es verificar si el string dado es un heterograma o no. Un heterograma es una palabra, frase u oración en la que ninguna letra del alfabeto aparece más de una vez.

```
s = 'The big dwarf only jumps'
#Output: Es un heterograma ya que cada caracter aparece 1 vez

s = 'Estudiante'
#Output: No es un heterograma ya que [e] aparece mas de 1 vez

```

---

## Diccionarios

---
**C7E1**


Cuenta la cantidad de frutas en su cesta. Para hacer esto, tiene el  diccionario y la lista de frutas. Use el diccionario y la lista para contar el número total de frutas y los otros artículos que no son frutas en su cesta.

**Starter Code:**
```
catidad_frutas, cantidad_no_frutas = 0, 0
cesta = {'manzanas': 4, 'naranjas': 19, 'hamburgesas': 3, 'sandwiches': 8}
frutas = ['manzanas', 'naranjas', 'peras', 'parchitas', 'uvas', 'cambures']
```

**Output:**
```
Hay {} frutas en la cesta. y {} objetos que no son frutas.
```

---
**C7E2**

Podemos crear un diccionario, contador, que realiza un seguimiento del recuento total de cada palabra en la lista quote.

**Starter Code:**
```
contador = {}
quote =  ['Tienes', 'que', 'bailar', 'como', 'si', 'no', 'hubiera', 'nadie', 'mirando', 'Ama', 'como', 'si', 'nunca', 'te', 'lastimaran', 'Canta', 'como', 'si', 'no', 'hubiera', 'nadie', 'escuchando', 'Y', 'vive', 'como', 'si', 'fuera', 'el', 'cielo', 'en', 'la', 'tierra.']
```

**Output:**

```
**`{'Tienes': 1, 'que': 1, 'bailar': 1, 'como': 4, 'si': 4, 'no': 2, 'hubiera': 2, 'nadie': 2, 'mirando': 1, 'Ama': 1, 'nunca': 1, 'te': 1, 'lastimaran': 1, 'Canta': 1, 'escuchando': 1,'Y': 1, 'vive': 1, 'fuera': 1, 'el': 1, 'cielo': 1, 'en': 1,'la': 1, 'tierra.': 1}`**
```

---
**C7E3**

Se le ha contratado en la compañía `super-security` para que cree un sistema de autenticación de usuarios. Para esto deberá crear una función el cual acepte 3 parámetros, el **usuario, clave (**estos datos debera pedirlos por teclado**)** y  **un diccionario llamado **db** en donde se tiene la información de la compañía de quienes tienen acceso al sistema, esta función deberá decir si el usuario tiene acceso o no.**

**Starter Code:**
```
# Escribe tus funciones aqui.



# Funcion principal.
def main():
	# Esta es la base de datos:
	db = {
			"benjamisharifker2001" : "1234",
			"kevinelpreparador" : "estudienp@lQuiz",
			"elsaman" : "unimet123"
	}

	# Escribe tu llamado a funcion aqui
	
# Llamado a función principal.
main()
```

**Outputs Esperados:**

Si es autenticado correctamente:

```
El usuario {nombre_de_usuario} ha sido autenticado!
```

Si no:

```
Usuario o clave incorrecta
```

---


## Funciones

---
**C8E1**

Escriba una función llamada densidad_de_poblacion que tome dos argumentos: poblacion y area, y devuelva una densidad de población. calculada a partir de esos valores.

---
**C8E2**


Escriba una función llamada `leer_tiempo()`

 La función debe tomar **un** argumento, un número entero y **devolver** un **string** que indique cuántas semanas y días son. 

Por ejemplo, llamando a la función e imprimiendo el resultado de esta manera:

**INPUT:**
```
print(leer_tiempo(10))
```

**Output:**

```
1 semana(s) y 3 dias(s).
```

---

