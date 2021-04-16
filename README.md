# Programateca: AyP 
Guía de Ejercicios de Algoritmos y Programación 

## Variables, Operadores y Strings

---
**C2E1.**

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

**C2E2.**

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

** Output: **

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

** Output: **

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



`https://www.w3schools.com/python/ref_string_replace.asp`



b. Ahora en vez de crear una nueva lista, queremos actualizar la lista existente students con el mismo Output

---

**C4E4**
Debe escribir un While Loop que tome los números en una lista dada llamada: `num_list`

Su código debe **sumar** los números impares en la lista, pero solo hasta los primeros 5 números impares.

- Sumar los primeros 5 números impares en la lista.
- Si hay mas de 5 números impares, detenerse de sumar en el 5to número y mostrar mensaje con la cantidad de números impares y la suma total.

**Output**:

```
"La cantidad de números impares es: {contador_impares}"
"La suma total de los números impares es: {suma_impares}"
```
**Starter Code**:
```
num_list = [422, 136, 524, 85, 96, 719, 85, 92, 10, 17, 312, 542, 87, 23, 86, 191, 116, 35, 173, 45, 149, 59, 84, 69 , 113, 166]

```

---



