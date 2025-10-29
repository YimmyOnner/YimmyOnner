# 🛠️ Prácticas: PSeInt, Diagramas de Flujo y Programación en C

En esta sección se agrupan exclusivamente las actividades prácticas relacionadas con pseudocódigo (PSeInt), diagramas de flujo y la implementación en **C**. Cada ítem enlaza a la evidencia PDF correspondiente y se incluye una breve descripción y ejemplo.

- **Taller1**  
  Enlace: [Taller1.pdf](./../Evidencias/Taller1.pdf)

- **Aprendizaje_Autonomo**  
  Enlace: [Aprendizaje_Autonomo.pdf](./../Evidencias/Aprendizaje_Autonomo.pdf)

- **Aprendizaje_Practico_Experimental2**  
  Enlace: [Aprendizaje_Practico_Experimental2.pdf](./../Evidencias/Aprendizaje_Practico_Experimental2.pdf)

- **Primer_Algoritmo_Secuencial**  
  Enlace: [Primer_Algoritmo_Secuencial.pdf](./../Evidencias/Primer_Algoritmo_Secuencial.pdf)


---

### Ejemplo de código (extracto representativo)

```c
#include <stdio.h>

int main() {
    float peso, altura, imc;
    printf("Ingrese peso (kg): ");
    scanf("%f", &peso);
    printf("Ingrese altura (m): ");
    scanf("%f", &altura);
    imc = peso / (altura * altura);
    printf("IMC = %.2f\n", imc);
    return 0;
}
```

<div align="left">
[![⬅️ Volver al Inicio](https://img.shields.io/badge/⬅️_Volver_al_Inicio-blue?style=for-the-badge)](../index.md)
</div>
