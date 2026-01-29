### 📦 Programación modular
- Analizar los conceptos fundamentales de la programación modular.
- Aplicar módulos y funciones en la resolución de problemas computacionales.
- Mejorar la organización, reutilización y mantenimiento del código.

### 📊 Estructuras de datos estáticas
- Comprender el funcionamiento de los arreglos unidimensionales (vectores).
- Aplicar arreglos bidimensionales (matrices) en la resolución de problemas.
- Identificar el uso de arreglos multidimensionales.
- Manejar cadenas de caracteres (strings) en el lenguaje C.

---

## 🧩 Programación Modular

### 📦 Conceptos básicos de la programación modular
La **programación modular** es una técnica que consiste en dividir un programa extenso en partes más pequeñas llamadas **módulos**, donde cada módulo se encarga de cumplir una función específica dentro del sistema.

Este enfoque permite que los programas sean más fáciles de entender, desarrollar y mantener, evitando códigos largos y complejos. Cada módulo puede ser diseñado y probado de forma independiente, lo que facilita la detección y corrección de errores.

La idea principal de la programación modular es que cada módulo:
- Tenga una única responsabilidad.
- Sea reutilizable en otros programas.
- Pueda modificarse sin afectar al resto del sistema.

---

### 🧠 Uso de módulos y funciones en la resolución de problemas
Una **función** es un bloque de código que realiza una tarea específica y puede ser reutilizado varias veces dentro de un programa. Cuando varias funciones relacionadas se agrupan, forman un **módulo**.

Resolver problemas mediante programación modular implica:
- Dividir el problema principal en subproblemas más pequeños.
- Asignar cada subproblema a una función o módulo.
- Integrar las soluciones parciales en un programa completo y funcional.

Este método mejora la lógica del programa, facilita su comprensión y permite desarrollar aplicaciones más grandes sin aumentar innecesariamente la complejidad.

---

### 🛠️ Ventajas de la programación modular
- Permite una mejor organización del código.
- Facilita el mantenimiento y la corrección de errores.
- Favorece la reutilización de funciones en otros proyectos.
- Reduce la complejidad de los programas grandes.
- Mejora el trabajo colaborativo en equipo.

---
#### 📊Paso de parámetros por valor

El **paso de parámetros por valor** consiste en enviar a una función una **copia del valor** de la variable original. Cualquier modificación que se realice dentro de la función **no afecta** al valor original.

**Ejemplo en lenguaje C:**

```
#include <stdio.h>

void duplicar(int valor) {
    valor = valor * 2;
}

int main() {
    int cantidad = 10;
    duplicar(cantidad);
    printf("%d", cantidad);
    return 0;
}
```
### 📈Prueba de escritorio
| Paso | Variable `cantidad` (main) | Variable `valor` (función) | Explicación                                            |
| ---- | -------------------------- | -------------------------- | ------------------------------------------------------ |
| 1    | 10                         | —                          | Se declara la variable `cantidad` con valor inicial 10 |
| 2    | 10                         | 10                         | Se llama a la función y se copia el valor              |
| 3    | 10                         | 20                         | La variable `valor` se duplica dentro de la función    |
| 4    | 10                         | —                          | Finaliza la ejecución de la función                    |
| 5    | 10                         | —                          | Se imprime el valor de `cantidad`                      |

En este ejemplo se observa que la variable cantidad conserva su valor original, ya que la función trabaja únicamente con una copia del dato recibido y no con la variable original.

#### 📊Paso de parámetros por referencia

El **paso de parámetros por referencia** permite que una función reciba la **dirección de memoria** de una variable, lo que hace posible modificar directamente su valor original.

**Ejemplo en lenguaje C:**

```c
#include <stdio.h>

void duplicar(int *valor) {
    *valor = (*valor) * 2;
}

int main() {
    int cantidad = 10;
    duplicar(&cantidad);
    printf("%d", cantidad);
    return 0;
}
```
### 📈Prueba de escritorio
| Paso | Variable `cantidad` (main) | Dirección apuntada por `valor` | Explicación                                            |
| ---- | -------------------------- | ------------------------------ | ------------------------------------------------------ |
| 1    | 10                         | —                              | Se declara la variable `cantidad` con valor inicial 10 |
| 2    | 10                         | &cantidad                      | Se envía la dirección de memoria a la función          |
| 3    | 20                         | &cantidad                      | Se modifica el valor apuntado por el puntero           |
| 4    | 20                         | —                              | Finaliza la ejecución de la función                    |
| 5    | 20                         | —                              | Se imprime el valor de `cantidad`                      |

En este caso, el valor de la variable `cantidad` sí se modifica, ya que la función recibe su dirección de memoria y accede directamente a ella mediante un puntero, permitiendo cambiar el valor original desde la función.

#### 🔹 Importancia de la modularidad

- Mejora la legibilidad y organización del código  
- Facilita el mantenimiento y la corrección de errores  
- Permite la reutilización de funciones en distintos programas  
- Favorece el trabajo colaborativo en proyectos de software  

La modularidad es una base esencial para el desarrollo de programas eficientes y estructurados, especialmente en aplicaciones de mayor complejidad.

[Volver a la unidad 3](Unidad3.md)

