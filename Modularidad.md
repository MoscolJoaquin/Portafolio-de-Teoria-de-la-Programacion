### 🧱 Modularidad

La **modularidad** es un principio fundamental de la programación que consiste en dividir un programa en **módulos o funciones independientes**, donde cada uno cumple una tarea específica. Este enfoque permite que los programas sean más **claros, organizados, reutilizables y fáciles de mantener**.

Al aplicar la modularidad, se evita la repetición de código y se facilita la detección y corrección de errores, ya que cada módulo puede probarse de manera independiente. Además, este principio es clave en el desarrollo de software estructurado y escalable [16].

---

#### 🔹 Paso de parámetros por valor

El **paso de parámetros por valor** consiste en enviar a una función una **copia del valor** de la variable original. Cualquier modificación que se realice dentro de la función **no afecta** al valor original de la variable.

**Ejemplo en lenguaje C:**

```c
#include <stdio.h>

void incrementar(int x) {
    x = x + 1;
}

int main() {
    int numero = 5;
    incrementar(numero);
    printf("%d", numero);
    return 0;
}
```
### Prueba de escritorio
| Paso | Variable `numero` (main) | Variable `x` (función) | Explicación |
|-----:|--------------------------|------------------------|-------------|
| 1 | 5 | — | Se declara `numero` con valor inicial 5 |
| 2 | 5 | 5 | Se llama a la función y se copia el valor |
| 3 | 5 | 6 | `x` se incrementa dentro de la función |
| 4 | 5 | — | La función termina |
| 5 | 5 | — | Se imprime `numero` |

En este ejemplo, la variable `numero` mantiene su valor original, ya que la función trabaja únicamente con una copia del dato recibido [17].

---

#### 🔹 Paso de parámetros por referencia

El **paso de parámetros por referencia** permite que la función reciba la **dirección de memoria** de la variable original, lo que posibilita modificar directamente su contenido.

**Ejemplo en lenguaje C:**

```c
#include <stdio.h>

void incrementar(int *x) {
    *x = *x + 1;
}

int main() {
    int numero = 5;
    incrementar(&numero);
    printf("%d", numero);
    return 0;
}
```
### Prueba de escritorio

| Paso | Variable `numero` (main) | Dirección apuntada por `x` | Explicación |
|-----:|--------------------------|----------------------------|-------------|
| 1 | 5 | — | Se declara `numero` con valor inicial 5 |
| 2 | 5 | &numero | Se envía la dirección de memoria |
| 3 | 6 | &numero | Se incrementa el valor apuntado |
| 4 | 6 | — | La función termina |
| 5 | 6 | — | Se imprime `numero` |

En este caso, el valor de la variable `numero` sí cambia, debido a que la función accede directamente a la dirección de memoria mediante un puntero [18].

---

#### 🔹 Importancia de la modularidad

- Mejora la legibilidad y organización del código  
- Facilita el mantenimiento y la corrección de errores  
- Permite la reutilización de funciones en distintos programas  
- Favorece el trabajo colaborativo en proyectos de software  

La modularidad es una base esencial para el desarrollo de programas eficientes y estructurados, especialmente en aplicaciones de mayor complejidad.

[Volver a la unidad 3](Unidad3.md)

