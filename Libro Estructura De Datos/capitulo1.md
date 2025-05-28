# UNIVERSIDAD NACIONAL DEL ALTIPLANO

<p align="center">
  <img src="descargar.jpg" alt="Mi foto" width="320 "/>
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
7. [Operadores & y *](#operadores-and-asterisco)


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

## Operadores and asterisco
En C++, los operadores & (ampersand) y * (asterisco) tienen un uso especial en el manejo de punteros, aunque también se pueden usar en otros contextos. A continuación se explica cada uno:

### Operador & (operador de dirección)
El operador & se utiliza para obtener la dirección de memoria de una variable. Es decir, nos da un puntero el valor.

```cpp

int numero = 10;
int* puntero = &numero; // El puntero almacena la dirección de 'numero'
```
&numero devuelve la dirección de memoria de la variable numero, esa dirección se guarda en un puntero, que en este caso es int* puntero.

### Operador * (operador de desreferenciación)

El operador * se utiliza para acceder al almacenado en una dirección de memoria es decir al contenido del puntero.

## Ejemplo
```cpp
int a = 10;
int* p = &a;
cout << *p; // Imprime 10
```
*p se puede decir que "el valor almacenado en la dirección que guarda p", como p apunta a "a", *p accede al contenido de a.

## Ejemplo completo
```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 42;
    int* ptr = &a;      // 'ptr' guarda la dirección de 'a'
    
    cout << "Valor de a: " << a << endl;
    cout << "Dirección de a: " << &a << endl;
    cout << "Contenido de ptr: " << ptr << endl;
    cout << "Valor apuntado por ptr: " << *ptr << endl;

    return 0;
}
```
## Operador ->
 El operador-> se usa para acceder a los miembros de una estructura o clase a trav´ es de un puntero.
 Este operador es una forma abreviada de hacer lo que ser´ ıa equivalente a (*ptr).miembro.
 ### Ejemplo 
 ```cpp
 puntero->miembro
 ```
 Es lo mismo que:
 ```cpp
 (*puntero).miembro
 ```
 Es decir, ptr-> es lo mismo que (*ptr).x, pero más limpio y claro.

 ### Ejemplo práctico
 ```cpp
 #include <iostream>
using namespace std;

struct Persona {
    string nombre;
    void saludar() {
        cout << "Hola, soy " << nombre << endl;
    }
};

int main() {
    Persona p = {"Ana"};
    Persona* ptr = &p;      // ptr apunta al objeto p

    ptr->saludar();         // Accedemos a la función mediante puntero
    cout << ptr->nombre;    // Accedemos al atributo mediante puntero

    return 0;
}
```
El operador -> es una herramienta esencial en C++ para trabajar con punteros a objetos. Su principal ventaja es que permite acceder de forma clara y directa a los miembros (atributos o métodos) de un objeto apuntado, sin necesidad de usar la notación más compleja (*ptr).miembro.

Su uso es fundamental en estructuras de datos dinámicas, como listas enlazadas, árboles o cualquier situación en la que se manipulan objetos a través de punteros. Entender y dominar el operador -> es clave para escribir código más legible, eficiente y orientado a objetos en C++.

¿Quieres que también redacte una conclusión comparando los operadores . y ->?

## Listas enlazadas
Una lista enlazada es una colección de elementos, llamados nodos, donde cada nodo contiene dos partes:

1. Un dato (por ejemplo, un número o un objeto)

2. Un puntero (o enlace) al siguiente nodo en la lista

A diferencia de los arrays, las listas enlazadas no almacenan sus elementos en posiciones contiguas de memoria, lo que permite insertar o eliminar nodos fácilmente sin necesidad de mover otros elementos.
Ejemplo
```cpp
[10 | * ] → [20 | * ] → [30 | NULL]
```
Cada no tiene, un valor (por ejemplo 10,20 y 30), un puntero al siguiente nodo.

## Tipos de listas enlazadas

- Lista simplemente enlazada: Cada nodo apunta solo al siguiente nodo.
- Lista doblemente enlazasa: Cada nodo apunta al anterior y al siguiente nodo.
- Lista Circular: El último nodo apunta al primero, formando un ciclo.

Las ventajas son las inserciones y eliminaciones eficientes en cualquier posición, también el tamaño dinámico (crece o se reduce en tiempo de ejecución), finalmente ideal para estructuras como pilas, colas y árboles.

### Ejemplo
```cpp
#include <iostream>
using namespace std;

struct Nodo {
    int dato;
    Nodo* siguiente;
};

int main() {
    Nodo* primero = new Nodo{10, nullptr};
    primero->siguiente = new Nodo{20, nullptr};
    primero->siguiente->siguiente = new Nodo{30, nullptr};

    Nodo* actual = primero;
    while (actual != nullptr) {
        cout << actual->dato << " ";
        actual = actual->siguiente;
    }
    return 0;
}
```





