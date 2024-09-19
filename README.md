## Instrucciones Generales
- **Debe** respetar el nombre de las funciones y el nombre de los parámetros que más adelante se describen
- Deben contruir las funciones con **Python** 
- Debe crear los comentarios de cada función tomando en cuenta **Nombre**, **Entrada**, **Salida** y **Restricciones**
- Recordar que en este caso por evaluar vectores o matrices **no se debe recortar**, solo el recorrido es por sus índices
- Pueden hacer uso **Try/Except, isinstance, type**
- Pueden hacer el uso de las funciones que se va creando durante el examen.
- Las respuestas serán publicadas en este repositorio el martes 24 de septiembre.


## sumasEnDiagonal(matriz)

Escriba un programa con sintaxis Python cuya función principal se llame sumasEnDiagonal(matriz), que reciba como entrada una matriz (lista de listas de enteros) de tamaño cuadrado impar. Esta función retornará la suma de los elementos de las dos diagonales principales de la matriz. No se debe contar dos veces el elemento central de la matriz.

### Restricciones:
- La matriz debe ser cuadrada (mismo número de filas y columnas).
- El tamaño de la matriz debe ser un número impar.

Ejemplos del comportamiento de la función:

```python
>>> sumasEnDiagonal([[2, 0, 3],
                     [4, 5, 6],
                     [7, 8, 9]])
36  # (2 + 5 + 9) + (3 + 5 + 7) - 5

>>> sumasEnDiagonal([[1, 0, 1],
                     [0, 1, 0],
                     [1, 0, 1]])
4   # (1 + 1 + 1) + (1 + 1 + 1) - 1
```

## esParLigado(lista)

Escriba un programa con sintaxis Python cuya función principal se llame esParLigado(lista), que reciba como entrada una lista de números enteros. Esta función retornará True si siempre que aparece un número par, este es seguido por un número impar, o False en caso contrario. En el caso de que la lista termine en un número par, se considerará que no está ligado a un impar, por lo que la función retornará False.

```python
>>> esParLigado([2, 3, 4, 7, 8, 9])
True
>>> esParLigado([2, 4, 6, 8])
False
>>> esParLigado([5, 7, 9])
True
>>> esParLigado([2, 3, 6, 8, 10])
False
```

## matriz_triangular_inversa(matriz)

Escriba un programa con sintaxis Python cuya función principal se llame matriz_triangular_inversa(matriz), que reciba como entrada una matriz (lista de listas de enteros) de tamaño n x n. La función retornará True si todos los elementos que están debajo de la diagonal inversa de la matriz son múltiplos de 3, o False en caso contrario.

### Restricciones:
- El tamaño de la matriz debe ser cuadrado (n x n) con n mayor o igual a 4.

```python
>>> matriz_triangular_inversa([[3, 2, 1, 4],
                               [9, 3, 2, 1],
                               [6, 12, 3, 2],
                               [15, 9, 6, 3]])
True

>>> matriz_triangular_inversa([[3, 2, 1, 4],
                               [9, 3, 2, 1],
                               [6, 12, 3, 2],
                               [15, 8, 6, 3]])
False
```

## multiplicacionMatrices(matriz1, matriz2)

Escriba un programa con sintaxis Python cuya función principal se llame multiplicacionMatrices(matriz1, matriz2), que reciba como entradas dos matrices (listas de listas de enteros o flotantes) llamadas matriz1 y matriz2. La función retornará el producto de ambas matrices, si es posible realizar la multiplicación.

### Restricciones:
- Los parámetros de entrada deben ser matrices (listas de listas).
- El número de columnas de la matriz1 debe coincidir con el número de filas de la matriz2 para que la multiplicación sea válida.

```python
>>> multiplicacionMatrices([[1, 2],
                            [3, 4]],
                                   [[5, 6],
                                    [7, 8]])
[[19, 22],
 [43, 50]]

>>> multiplicacionMatrices([[1, 4, 6],
                            [2, 5, 8]],
                                      [[1, 0],
                                       [2, 1],
                                       [3, 4]])
[[25, 28],
 [34, 41]]
```
