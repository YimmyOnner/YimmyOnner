# 💻 Lenguaje C

> “El lenguaje C es uno de los más utilizados en la historia de la programación por su eficiencia, flexibilidad y control sobre el hardware.”
> — *Goin, 2022; Guerra Salazar et al., 2023*

---

## ⚙️ Codificación

La **codificación** consiste en traducir un algoritmo escrito en pseudocódigo a un **lenguaje de programación** formal.
Esto implica reemplazar las palabras en español por sus equivalentes en inglés y **agregar detalles técnicos** como la declaración de variables, constantes y librerías.

📁 El código fuente en C se guarda con la extensión `.c`, por ejemplo:

```bash
nombre_archivo.c
```

---

## 🧰 Librerías o Bibliotecas

Las **librerías** son archivos con código reutilizable que permiten realizar operaciones comunes.
Siempre se incluyen al inicio del programa mediante la directiva `#include`.

```c
#include <stdio.h>   // Entrada y salida estándar
#include <stdlib.h>  // Funciones del sistema
#include <string.h>  // Manejo de cadenas
#include <math.h>    // Operaciones matemáticas
#include <time.h>    // Control del tiempo
```

📘 La extensión de los archivos de librería es `.h`.
Ejemplo: `#include <libreria.h>`

---

## 🚀 Estructura básica del programa en C

En pseudocódigo usamos **Inicio** y **Fin**; en C, todo comienza dentro de la función `main()`:

```c
#include <stdio.h>

int main() {
    printf("Hola, mundo!\n");
    return 0;
}
```

🔹 El programa se **compila** con:

```bash
gcc hola_mundo.c -o hola_mundo
```

🔹 Y se **ejecuta** con:

```bash
./hola_mundo
```

---

## 🧮 Tipos de datos en C

Los **tipos de datos** determinan qué tipo de información puede almacenar una variable.

| Tipo de dato | Descripción                          | Ejemplo                    |
| ------------ | ------------------------------------ | -------------------------- |
| `int`        | Números enteros                      | `int edad = 25;`           |
| `float`      | Números decimales                    | `float nota = 8.5;`        |
| `double`     | Números decimales de mayor precisión | `double pi = 3.141592;`    |
| `char`       | Caracter individual                  | `char letra = 'A';`        |
| `char[]`     | Cadena de caracteres                 | `char nombre[] = "Maria";` |
| `bool`       | Valores lógicos (verdadero/falso)    | `bool activo = true;`      |

📗 *Fuente: Guerra Salazar et al., 2023*

---

## 🧾 Declaración de variables

Las variables deben declararse **antes de usarse**.
Ejemplos:

```c
int a, b;
float promedio = 0.0;
char opcion = 'S';
char nombre[20] = "Yimmy";
```

También pueden declararse **e inicializarse** al mismo tiempo.

---

## 🔢 Constantes

Las **constantes** son valores que no cambian durante la ejecución del programa.
Pueden declararse de dos maneras:

```c
// Opción 1: Constante tipada
const float PI = 3.1416;
const char UNIVERSIDAD[] = "UNL";

// Opción 2: Directiva de preprocesador
#define MAX 100
#define IVA15 0.15
```

---

## 🔄 Asignación de valores

Se usa el símbolo `=` para asignar valores:

```c
a = a + 5;
sueldo = 450;
estadoCivil = 'D';
```

También se usan **operadores compuestos** y **de incremento/decremento**:

```c
b++;
++b;
b--;
--b;
```

---

## 💬 Entrada y salida de datos

### Entrada → `scanf()`

```c
scanf("%d", &edad);
scanf("%f", &promedio);
scanf("%s", nombre);
```

### Salida → `printf()`

```c
printf("La edad es %d\n", edad);
printf("El promedio es %.2f\n", promedio);
printf("Nombre: %s\n", nombre);
```

---

## 🧮 Ejemplo práctico (pseudocódigo → C)

### 🧾 Pseudocódigo

```pseint
Algoritmo Calculo_Area_Rectangulo
  Definir base, altura, area Como Real
  Escribir "Ingrese la base y la altura:"
  Leer base, altura
  area <- base * altura
  Escribir "El área es: ", area
FinAlgoritmo
```

### 💻 Código en C

```c
#include <stdio.h>

int main() {
    float base, altura, area;

    printf("Ingrese la base del rectángulo: ");
    scanf("%f", &base);
    printf("Ingrese la altura del rectángulo: ");
    scanf("%f", &altura);

    area = base * altura;
    printf("El área del rectángulo es: %.2f\n", area);

    return 0;
}
```

---

## 🧠 Prueba de escritorio

| Entrada    | Proceso              | Salida                           |
| ---------- | -------------------- | -------------------------------- |
| base = 5   | area = base * altura | El área del rectángulo es: 15.00 |
| altura = 3 | 5 * 3 = 15           |                                  |

---

## 🧩 Palabras reservadas

`int`, `for`, `while`, `return`, `printf`, `scanf`, `if`, `else`, `switch`, `break`, `continue`

---

## 🗒️ Comentarios

```c
// Este es un comentario de una línea

/*
   Este es un comentario
   de varias líneas
*/
```

---

## 📘 Conclusión

El **lenguaje C** es un pilar de la programación estructurada.
Permite escribir código eficiente, cercano al hardware y con gran control sobre los recursos del sistema.
Su aprendizaje brinda una base sólida para otros lenguajes como C++, Java o Python.

---

## 📚 Referencias

* Goin, M. (2022). *Caminando junto al Lenguaje C*. Editorial UNRN.
* Guerra Salazar, J. E., Ramos Valencia, M. V., & Vallejo Vallejo, G. E. (2023). *Programando en C desde la práctica: problemas resueltos*. Puerto Madero Editorial.
* Figueroa Piscoya, J. et al. (2021). *Ejercicios básicos de programación estructurada*.
