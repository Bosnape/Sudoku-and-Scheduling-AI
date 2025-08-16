# Entrega 1 - Introducción a la Inteligencia Artificial

## Resumen del Proyecto

Este repositorio contiene la implementación de dos problemas fundamentales de Inteligencia Artificial:

1. **Agente de Búsqueda:** Resolvedor de Sudokus usando el algoritmo A*.
2. **Algoritmo Genético:** Optimizador de horarios personales.

## Participantes

- Pablo Cabrejos
- Sofia Flores
- Isabella Camacho
- Santiago Gomez

## Tecnologías Utilizadas

- **Python 3.13**
- **Jupyter Notebooks**
- **Algoritmos de búsqueda informada (A*)**
- **Algoritmos evolutivos (GA)**
- **Librerías:** heapq, time, matplotlib **[PENDIENTE: Completar librerías adicionales]**

## 1. Agente de Búsqueda: Resolvedor de Sudokus

### Descripción del Problema

Se implementó un agente de búsqueda informada utilizando el algoritmo A* para resolver puzzles de Sudoku. El problema consiste en llenar una cuadrícula de 9x9 con números del 1 al 9, respetando las reglas del Sudoku: cada fila, columna y caja 3x3 debe contener todos los números sin repetición. El espacio de estados se representa como una matriz 9x9 donde cada celda puede contener un número del 1 al 9 o estar vacía (representada por 0). Las acciones consisten en colocar un número válido en una celda vacía, y el modelo de transición genera un nuevo estado aplicando la acción seleccionada. Se implementaron dos heurísticas: h1 (número de celdas vacías) y h2 (sumatoria de posibilidades de las celdas vacías), junto con una optimización MRV (Minimum Remaining Values) que selecciona la celda con menos opciones disponibles para reducir el factor de ramificación.

## 2. Algoritmo Genético: Optimizador de Horarios Personales

### Descripción del Problema

Se desarrolló un algoritmo genético para optimizar horarios personales considerando múltiples actividades como clases, trabajo, gimnasio, hobbies y descansos. El problema consiste en asignar actividades a bloques de tiempo discretos (por ejemplo, bloques de 30 minutos) maximizando el bienestar personal mientras se cumplen restricciones de tiempo y prioridades. El cromosoma se representa como una secuencia de actividades asignadas a cada bloque temporal, donde cada gen corresponde a una actividad específica. La función de fitness evalúa la calidad del horario penalizando solapamientos de actividades, horas de sueño insuficientes y violaciones de restricciones de tiempo, mientras recompensa más tiempo en actividades prioritarias y una distribución equilibrada. Las restricciones incluyen franjas fijas para clases y trabajo, límites diarios de horas por actividad, prioridades asignadas a diferentes actividades y requisitos mínimos de descanso. **[PENDIENTE: Implementar algoritmo genético completo]**

## Información adicional

La explicación completa del desarrollo de ambos problemas se encuentra en la [Wiki del repositorio](https://github.com/Bosnape/Sudoku-and-Scheduling-AI/wiki).
