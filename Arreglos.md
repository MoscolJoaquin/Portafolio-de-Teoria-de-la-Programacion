## 📊 Estructuras de Datos Estáticas

### 📈 Arreglos Unidimensionales (Vectores)
Un **arreglo unidimensional** o **vector** es una estructura de datos estática que permite almacenar una colección de elementos del mismo tipo en posiciones de memoria contiguas, todos bajo un mismo nombre.

Desde un punto de vista lógico, un vector puede imaginarse como una fila de casilleros numerados, donde cada número representa un **índice** que permite acceder a un valor específico. Es importante recordar que los índices siempre comienzan desde la posición cero.

**Características principales:**
- Homogeneidad: todos los elementos deben ser del mismo tipo de dato (int, float, char, etc.).
- Acceso mediante índices numéricos.
- Tamaño fijo definido en tiempo de compilación.

### Codigo en C:
<img width="550" height="396" alt="image" src="https://github.com/user-attachments/assets/a6132275-dbaf-460b-8922-650fa4afb559" />

Los arreglos unidimensionales se utilizan comúnmente para agrupar datos relacionados, como calificaciones, edades o registros numéricos, sin necesidad de declarar múltiples variables individuales.

---

### ⬛ Arreglos Bidimensionales (Matrices)
Los **arreglos bidimensionales**, también conocidos como **matrices**, organizan los datos en dos dimensiones: filas y columnas. Esta estructura es similar a una tabla o a una hoja de cálculo.

Para acceder a un elemento específico se utilizan dos índices: uno para la fila y otro para la columna, lo que permite una ubicación precisa dentro de la matriz.

**Características principales:**
- Acceso mediante la sintaxis matriz[fila][columna].
- Los datos se almacenan de forma lineal en memoria, fila por fila.
- Su recorrido suele realizarse mediante ciclos anidados.

## Codigo en C:
<img width="700" height="588" alt="image" src="https://github.com/user-attachments/assets/c7326d89-dc9a-408d-8ae0-6af2f62849bf" />

Las matrices son muy utilizadas para representar tablas de datos, tableros de juegos, mapas y operaciones matemáticas.

---

### 📦 Arreglos Multidimensionales
Los **arreglos multidimensionales** son estructuras que poseen tres o más dimensiones. Representan una extensión natural de los arreglos bidimensionales y permiten almacenar datos más complejos.

Una forma sencilla de comprenderlos es pensar que una matriz es una hoja, mientras que un arreglo tridimensional es un conjunto de hojas, como un libro.

**Características principales:**
- Requieren un índice por cada dimensión.
- El consumo de memoria aumenta considerablemente.
- Su comprensión exige un mayor nivel de abstracción lógica.

### Codigo en C:
<img width="906" height="641" alt="image" src="https://github.com/user-attachments/assets/bf269f43-2b27-4ee7-a689-911490eb3bdc" />

---
#### 🔹 Importancia del uso de arreglos

- Permiten almacenar y manipular grandes volúmenes de datos  
- Facilitan la implementación de algoritmos eficientes  
- Optimiza el uso de memoria  
- Son fundamentales para estructuras de datos más avanzadas
---

### 🔤 Cadenas de Caracteres (Strings)
En el lenguaje C, una **cadena de caracteres** es un arreglo de tipo `char` que se utiliza para almacenar texto. No existe un tipo de dato primitivo llamado string, por lo que las cadenas se manejan como arreglos especiales.

Estas cadenas finalizan con un carácter especial llamado **carácter nulo** (`\0`), el cual indica el final del texto y es indispensable para su correcto funcionamiento.

**Características principales:**
- Siempre deben terminar con el carácter nulo `\0`.
- Se manipulan mediante funciones de la librería `<string.h>`.
- No pueden reasignarse con el operador `=` después de su declaración.


## [Volver a la Unidad 3](Unidad3.md)

