# UNIVERSIDAD NACIONAL DEL ALTIPLANO

<p align="center">
  <img src="descargar.jpg" alt="Mi foto" width="320"/>
</p>

## Facultad De Ingeniería Estadistica E Informática

**Alumno:** Eliseo Tarqui Ajahuana  
**Curso:** Estructura de datos  
**Ingeniero:** Fred Torres Cruz

## 📚 Indice

1. [Introducción](#introducción)
2. [Operadores](#operadores)
3. [Estructuras De Control](#estructuras-de-control)
4. [Funciones](#funciones)
5. [Arrays](#arrays)
6. [Funcion](#funcion) 


## Introducción
Las estructuras de datos son un modo de representar información en una computadora, aunque además, cuentan con un comportamiento interno. ¿Qué significa? Que se rige por determinadas reglas/restricciones que han sido dadas por la forma en que está construida internamente.

En el ámbito de la informática, las estructuras de datos son aquellas que nos permiten, como desarrolladores, organizar la información de manera eficiente, y en definitiva diseñar la solución correcta para un determinado problema.

Ya sean las más utilizadas comúnmente - como las variables, arrays, conjuntos o clases- o las diseñadas para un propósito específico -árboles, grafos, tablas, etc.-, una estructura de datos nos permite trabajar en un algo nivel de abstracción almacenando información para luego acceder a ella, modificarla y manipularla.

## Operadores
Los operadores son símbolos especiales que se utilizan para realizar operaciones sobre variables y valores. Estas operaciones pueden ser matemáticas, lógicas, de comparación, de asignación, entre otras. Los operadores permiten construir expresiones que combinan datos y producen nuevos resultados, lo cual es esencial en la resolución de problemas mediante programación.

Por ejemplo, el operador + se usa para sumar dos valores, mientras que el operador == se emplea para comparar si dos expresiones son iguales. Gracias a los operadores, es posible tomar decisiones, repetir instrucciones, realizar cálculos, y controlar el flujo de un programa.

### Ejemplo:  

```cpp  
 
#include <iostream>

using namespace std;

int main() {
	int a, b;
	cout <<"Ingresa el primer numero " << endl;
	cin >> a;
	cout <<"Ingresa el segundo numero " << endl;
	cin >> b;
	
	int suma = a + b;
	int resta = a - b;
	int multiplicacion = a * b;
	int division = a / b;
	
	cout << "Suma " << suma << endl;
	cout << "Resta " << resta << endl;
	cout << "Multiplicacion " << multiplicacion << endl;
	cout << "Division " << division << endl;
	
	return 0;
}
```

## Estructuras De Control
Las estructuras de control son bloques de código que permiten modificar el flujo de ejecución de un programa. Es decir, controlan qué instrucciones se ejecutan, cuándo y cuántas veces.

### 1. Estructuras condicionales
permiten tomar diciciones según condicionales lógicas.

### Ejemplo con if:

```cpp
int edad = 18;
if (edad >= 18) {
    cout << "Eres mayor de edad" << endl;
}
```
### Otras formas condicionales:
* if-else
* switch

### 2. Estructuras repetitivas (bucles)
Permiten repetir instrucciones mientras se cumpla una condición.

### Tipos de bucles:
* While
* do-while
* for

### Ejemplo con for:

```cpp
for (int i = 0; i < 5; i++) {
    cout << "Repetición " << i << endl;
}
```
### Ejemplo con while:
```cpp
int i = 0;
while (i < 3) {
    cout << "i vale: " << i << endl;
    i++;
}
```
### Estructuras de control anidadas
Son estructuras de control dentro de otras, como if dentro de un for, o for dentro de otro for.
```cpp
for (int i = 1; i <= 3; i++) {
    if (i % 2 == 0) {
        cout << i << " es par" << endl;
    } else {
        cout << i << " es impar" << endl;
    }
}
```
Las estructuras de control son muy importantes en la programación porque nos permiten que un programa no se limite a ejecutar instrucciones de forma lineal. Gracias a ellas, el software puede tomar decisiones, repetir acciones, y adaptarse a diferentes situaciones, lo que le da un comportamiento dinámico e inteligente.

### **¿Por qué son tan importantes?**
* Permiten la toma de decisiones
* Automatizan procesos repetitivos
* Hacen el código más eficiente y flexible
* Forman la base de la lógica algorítmica

## Funciones

Una función es un bloque de código reutilizable que realiza una tarea específica. Puedes pensar en una función com una pequeña "máquina" dentro de tu programa, le das una entrada (si hace falta), y te devuelve una salida (si aplica), ejecutando un conjunto de instrucciones.

### ¿Para que sirven?
* Para organizar mejor el código
* Para evitar repetir instrucciones
* Para dividir un problema grande en partes más pequeñas y fáciles de resolver
* Para hacer que tu código sea más claro y mantenible.

### Ejemplo:
```cpp
int sumar(int a, int b) {
    return a + b;
}

int main() {
    int resultado = sumar(3, 5);
    cout << "La suma es: " << resultado << endl;
    return 0;
}
```


## Arrays
En programación, un array (también llamado arreglo) es una estructura de datos que permite almacenar múltiples valores del mismo tipo en una sola variable, organizados de forma secuencial en la memoria del computador.

### 🧪 Ejemplo básico de un array en C++

```cpp
#include <iostream>
using namespace std;

int main() {
    // Declaramos un array de 5 enteros
    int numeros[5] = {10, 20, 30, 40, 50};

    // Mostramos los elementos del array
    for (int i = 0; i < 5; i++) {
        cout << "Elemento " << i << ": " << numeros[i] << endl;
    }

    return 0;
}
```
## Funcion
##  ¿Qué es una función en C++?

Una **función** en C++ es un bloque de código reutilizable que realiza una tarea específica. Permite **organizar el programa en partes más pequeñas**, facilitando su lectura, mantenimiento y reutilización.

### 📌 Ventajas de usar funciones:
- Evita repetir código.
- Mejora la estructura del programa.
- Permite dividir un problema grande en subproblemas más simples.

---

### 🧪 Ejemplo básico de una función en C++

```cpp
#include <iostream>
using namespace std;

// Definimos una función que suma dos números
int sumar(int a, int b) {
    return a + b;
}

int main() {
    int resultado = sumar(5, 3);
    cout << "La suma es: " << resultado << endl;
    return 0;
}
```

