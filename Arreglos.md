### 📦 Arreglos

Los **arreglos** son estructuras de datos que permiten almacenar **varios valores del mismo tipo** bajo un mismo nombre, organizados en posiciones consecutivas de memoria. Cada elemento del arreglo se identifica mediante un **índice**, el cual inicia generalmente en cero.

El uso de arreglos facilita el manejo de grandes cantidades de datos, optimiza el uso de memoria y simplifica la implementación de algoritmos en programación estructurada [19].

---

#### 🔹 Arreglo unidimensional

Un **arreglo unidimensional** es una lista lineal de elementos, donde cada valor se accede mediante un solo índice. Es comúnmente utilizado para almacenar conjuntos simples de datos, como notas, edades o contadores.

**Ejemplo en lenguaje C:**

```c
#include <stdio.h>

int main() {
    int numeros[5] = {2, 4, 6, 8, 10};

    for (int i = 0; i < 5; i++) {
        printf("%d ", numeros[i]);
    }
    return 0;
}

```

| Paso | Índice `i` | Arreglo `numeros`        | Salida | Explicación |
|-----:|------------|--------------------------|--------|-------------|
| 1 | — | {2, 4, 6, 8, 10} | — | Se declara e inicializa el arreglo |
| 2 | 0 | {2, 4, 6, 8, 10} | 2 | Se imprime `numeros[0]` |
| 3 | 1 | {2, 4, 6, 8, 10} | 4 | Se imprime `numeros[1]` |
| 4 | 2 | {2, 4, 6, 8, 10} | 6 | Se imprime `numeros[2]` |
| 5 | 3 | {2, 4, 6, 8, 10} | 8 | Se imprime `numeros[3]` |
| 6 | 4 | {2, 4, 6, 8, 10} | 10 | Se imprime `numeros[4]` |

En este ejemplo, el arreglo almacena cinco números enteros y se recorren utilizando un ciclo `for` para mostrar sus valores.

---

#### 🔹 Arreglo bidimensional

Un **arreglo bidimensional** está compuesto por filas y columnas, similar a una tabla o matriz. Se utiliza para representar datos organizados en dos dimensiones, como matrices matemáticas o tablas de información.

**Ejemplo en lenguaje C:**

```c
#include <stdio.h>

int main() {
    int matriz[2][3] = {
        {1, 2, 3},
        {4, 5, 6}
    };

    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 3; j++) {
            printf("%d ", matriz[i][j]);
        }
        printf("\n");
    }
    return 0;
}
```
| Paso | `i` (fila) | `j` (columna) | Valor impreso | Explicación |
|-----:|------------|---------------|---------------|-------------|
| 1 | 0 | 0 | 1 | Primera fila, primera columna |
| 2 | 0 | 1 | 2 | Primera fila, segunda columna |
| 3 | 0 | 2 | 3 | Primera fila, tercera columna |
| 4 | 1 | 0 | 4 | Segunda fila, primera columna |
| 5 | 1 | 1 | 5 | Segunda fila, segunda columna |
| 6 | 1 | 2 | 6 | Segunda fila, tercera columna |


En este caso, la matriz contiene dos filas y tres columnas, y se recorre mediante ciclos anidados.

---

#### 🔹 Arreglo tridimensional

Un **arreglo tridimensional** extiende el concepto de los arreglos bidimensionales, añadiendo una tercera dimensión. Se emplea para representar estructuras más complejas, como capas, volúmenes o conjuntos de matrices.

**Ejemplo en lenguaje C:**

```c
#include <stdio.h>

int main() {
    int arreglo[2][2][2] = {
        {
            {1, 2},
            {3, 4}
        },
        {
            {5, 6},
            {7, 8}
        }
    };

    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++) {
            for (int k = 0; k < 2; k++) {
                printf("%d ", arreglo[i][j][k]);
            }
            printf("\n");
        }
        printf("\n");
    }
    return 0;
}
```
| Paso | `i` | `j` | `k` | Valor impreso | Explicación |
|-----:|-----|-----|-----|---------------|-------------|
| 1 | 0 | 0 | 0 | 1 | Primera capa, fila 0, columna 0 |
| 2 | 0 | 0 | 1 | 2 | Primera capa, fila 0, columna 1 |
| 3 | 0 | 1 | 0 | 3 | Primera capa, fila 1, columna 0 |
| 4 | 0 | 1 | 1 | 4 | Primera capa, fila 1, columna 1 |
| 5 | 1 | 0 | 0 | 5 | Segunda capa, fila 0, columna 0 |
| 6 | 1 | 0 | 1 | 6 | Segunda capa, fila 0, columna 1 |
| 7 | 1 | 1 | 0 | 7 | Segunda capa, fila 1, columna 0 |
| 8 | 1 | 1 | 1 | 8 | Segunda capa, fila 1, columna 1 |

Este ejemplo muestra un arreglo tridimensional de tamaño 2×2×2, recorrido mediante tres ciclos anidados.

---

#### 🔹 Importancia del uso de arreglos

- Permiten almacenar y manipular grandes volúmenes de datos  
- Facilitan la implementación de algoritmos eficientes  
- Optimiza el uso de memoria  
- Son fundamentales para estructuras de datos más avanzadas

## [Volver a la Unidad 3](Unidad3.md)

