#ControlDeFlujo 
#### 1.1. `While junto una condición

El bucle `while` se ejecuta mientras una condición dada sea verdadera. Aquí hay un ejemplo básico que cuenta hasta 5

```python
# Bucle while para contar hasta 5
contador = 1
while contador <= 5:
    print(contador)
    contador += 1
```

En este caso, el bucle se ejecutará mientras `contador` sea menor o igual a 5. El valor de `contador` se incrementa en cada iteración.
#### 1.2. Bucle `while` con `else`:

Similar al bucle `for`, el bucle `while` también puede tener una cláusula `else` que se ejecutará cuando la condición del bucle sea falsa:

```python
# Bucle while con else
contador = 1
while contador <= 5:
    print(contador)
    contador += 1
else:
    print("Fin del bucle")
```

Este bucle imprimirá los números del 1 al 5 y luego imprimirá "Fin del bucle" cuando la condición del `while` sea falsa.

#### 1.3. Bucle `while` con Break y Continue

Puedes usar `break` para salir del bucle antes de que se complete la iteración normal y `continue` para pasar a la siguiente iteración sin ejecutar el código restante dentro del bucle. Aquí hay un ejemplo:

```python
# Bucle while con break y continue
contador = 1
while contador <= 5:
    if contador == 3:
        contador += 1
        continue  # Salta a la siguiente iteración sin imprimir el número 3
    print(contador)
    if contador == 4:
        break  # Sale del bucle cuando el contador llega a 4
    contador += 1
```

Este bucle imprimirá los números del 1 al 2, luego saltará el número 3, imprimirá el número 4 y saldrá del bucle.

#### 1.4. Bucle `while` Infinito

Un bucle `while` puede convertirse en un bucle infinito si la condición nunca se vuelve falsa. Es importante evitar bucles infinitos para no bloquear la ejecución del programa.

```python
# Bucle while infinito
while True:
    # Código aquí
    pass  # pass se utiliza para tener una declaración válida que no hace nada
```

Este bucle se ejecutará indefinidamente hasta que se interrumpa manualmente.

Estos son algunos aspectos adicionales del bucle `while` en Python. Si tienes más preguntas o necesitas más ejemplos, no dudes en preguntar.

El bucle `for` es extremadamente versátil y puede utilizarse para recorrer diferentes tipos de datos y estructuras. Aquí hay algunos conceptos y ejemplos adicionales: