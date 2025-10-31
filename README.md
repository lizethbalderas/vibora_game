## Descripción General

El juego consiste en mover la **serpiente** por la ventana para comer la **comida** y crecer sin chocar consigo misma ni salir de los límites.  
Esta versión añade:
- **Comida móvil:** se desplaza **un paso a la vez** en direcciones aleatorias, sin salir de la ventana.  
- **Colores aleatorios (5 opciones, sin rojo):** en cada ejecución, la **serpiente** y la **comida** tienen **colores distintos** elegidos al azar de una paleta de 5 colores (excluyendo rojo).

---

## Contenido del Repositorio

- **snake.py** → Script principal.  
  Maneja el movimiento de la serpiente, la comida, la detección de colisiones, el pintado en pantalla y los controles.

---

## Controles

| Tecla | Acción                 |
|:------|:-----------------------|
| **→** | Mover a la derecha     |
| **←** | Mover a la izquierda   |
| **↑** | Mover hacia arriba     |
| **↓** | Mover hacia abajo      |

---

## Cambios Realizados

Se implementaron las siguientes mejoras sobre el código base de **Snake (FreeGames)**:

1. **La comida se mueve al azar un paso a la vez**  
   - En cada “tick” del juego la comida intenta desplazarse **1 celda** en una dirección aleatoria (arriba/abajo/izquierda/derecha).  
   - Se valida con una función de límites para que **no salga de la ventana**.

2. **Colores aleatorios y distintos (sin rojo)**  
   - Se definió una **paleta de 5 colores** (excluyendo el rojo).  
   - En cada ejecución, la **serpiente** toma un color aleatorio y la **comida** toma **otro color distinto** de la misma paleta.  
   - Garantiza que **no coincidan** entre sí y que **nunca** sea rojo.

> Nota: El color rojo se mantiene únicamente para indicar **fin del juego** en caso de colisión, conservando la retroalimentación visual.

---
**Autores**
Lizeth Jaqueline Balderas Sánchez
Felipe Gutiérrez Herrera
