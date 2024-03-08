#ControlDeFlujo 
#### 1.1. Recorrer `Rangos

El bucle `for` es ideal para recorrer elementos en una lista u otros tipos de datos iterables:

```python
# Bucle for para recorrer una lista
frutas = ["manzana", "naranja", "uva"]
for fruta in frutas:
    print(fruta)
```

En caso de que hagamos un condicional preguntando si hay manzanas pongamos un texto, ejemplo:

```python
    if fruta == "melocoton":
        print("hola, me gustaria compraros melocoton")
    else:
        print("No teneis melocoton, adios")
```

Escaneara cada uno de los componentes y por lo tanto pondrá una vez el primer print, y dos el segundo print.

#### 1.2. `Desempaquetar Elementos

Puedes desempaquetar elementos de una tupla o lista directamente en el bucle `for`. Por ejemplo:

```python
# Bucle for con desempaquetado de tuplas
pares = [(1, 2), (3, 4), (5, 6)]
for a, b in pares:
    print(a + b)
```

Esto imprimirá la suma de los elementos en cada tupla de la lista `pares`.

![[ForDesempaquetar.png]]
#### 1.3. Bucle `for` con `else`

Puedes usar la cláusula `else` con un bucle `for` para especificar un bloque de código que se ejecutará cuando el bucle haya recorrido todos los elementos

```python
# Bucle for con else
numeros = [1, 2, 3, 4, 5]
for numero in numeros:
    print(numero)
else:
    print("Fin del bucle")
```

Esto imprimirá cada número en la lista y luego imprimirá "Fin del bucle".

