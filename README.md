# Pseudoc-digo-y-Diagrama-de-flujo-
Instrucciones para Reto 3: 
1. Plantear el algoritmo para obtener los números primos hasta n, usando pseudocódigo y diagramas de flujo.
2. Revise el procedimiento matemático para hallar raíces cuadradas (son divisiones y restas), plantee el algoritmo en pseudocódigo y en diagrama de flujo.

## Numeros primos

```pseudocode
n : entero
i : entero
inicio
 1. Para cada número `i` desde 2 hasta `n` hacer:
   1.1. `esPrimo` = verdadero
   1.2. Para cada número `j` desde 2 hasta `i - 1` hacer:
        1.2.1. Si `i` módulo `j` es igual a 0 entonces:
              1.2.1.1. `esPrimo` = falso
              1.2.1.2. Salir del bucle (no es necesario continuar dividiendo)
   1.3. Si `esPrimo` es verdadero entonces:
        1.3.1. Imprimir `i` (es un número primo)
fin
```
El link del diagrama de flujo creado en mermaid: https://www.mermaidchart.com/raw/fd08382e-7803-4b3d-ba94-6187ceebe263?theme=dark&version=v0.1&format=svg

[![Untitled-diagram-2024-02-25-220053.png](https://i.postimg.cc/MTg1wpFT/Untitled-diagram-2024-02-25-220053.png)](https://postimg.cc/cgMvM0Zy)

## Raíces cuadradas
```pseudocode
n: entero
x: entero
inicio
1. Inicializar:
   - `n` es el número al que se le desea encontrar la raíz cuadrada.
   - `x` es la estimación inicial de la raíz cuadrada de `n`.
   - `epsilon` es la precisión deseada del resultado (por ejemplo, 0.0001).

2. Mientras que la diferencia absoluta entre `x*x` y `n` sea mayor que `epsilon` hacer:
   2.1. Calcular un nuevo valor para `x` como el promedio de `x` y `n / x` (esto es, `x = (x + n / x) / 2`).

3. Devolver `x` como la aproximación de la raíz cuadrada de `n`.
fin
```
El link del diagrama de flujo creado en mermaid: https://www.mermaidchart.com/raw/ee98c1f9-7982-4def-a635-fafb73bd2625?theme=dark&version=v0.1&format=svg

[![Untitled-diagram-2024-02-25-221501.png](https://i.postimg.cc/TY6C5ttP/Untitled-diagram-2024-02-25-221501.png)](https://postimg.cc/XXswTkSM)
