#ControlDeFlujo 
Los controles de flujo complementarios son instrucciones que permiten modificar el comportamiento normal de los bucles y condicionales en Python. Estas instrucciones son `break`, `continue` y `pass`.
#### 1.1. `break`

La instrucción `break` se utiliza para salir de un bucle de manera prematura. Cuando se encuentra un `break`, el control del programa salta inmediatamente fuera del bucle más cercano que lo contiene.

```python
for i in range(5):
    if i == 3:
        break
    print(i)
```
En este ejemplo, el bucle `for` se detiene cuando `i` es igual a 3 debido a la instrucción `break`, y la ejecución del programa continúa después del bucle.
#### 1.2. `continue`

La instrucción `continue` se utiliza para omitir el resto del código dentro de un bucle para una iteración específica y continuar con la siguiente iteración del bucle.

```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```
En este ejemplo, cuando `i` es igual a 2, la instrucción `continue` hace que el bucle pase a la siguiente iteración sin ejecutar el código restante dentro del bucle para ese valor de `i`.
#### 1.3. `pass`

La instrucción `pass` no hace nada. Se utiliza cuando la sintaxis requiere una declaración, pero no se necesita ninguna acción. Es útil como marcador de posición cuando se está escribiendo código y se planea agregar la implementación más tarde.

```python
for i in range(5):
    if i == 2:
        pass
    else:
        print(i)

```

En este ejemplo, cuando `i` es igual a 2, la instrucción `pass` no hace nada y el bucle continúa con la siguiente iteración sin imprimir nada.

Estas instrucciones complementarias de control de flujo son útiles para modificar el comportamiento de los bucles y condicionales en situaciones específicas dentro del programa en Python.