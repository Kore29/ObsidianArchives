#ExercicesPython
Escribe un programa en Python que simule el lanzamiento de un dado de seis caras. El programa debe realizar lo siguiente:

1. Preguntar al usuario cuántas veces desea lanzar el dado.
2. Simular el lanzamiento del dado la cantidad de veces especificada por el usuario.
3. Imprimir los resultados de cada lanzamiento y calcular el porcentaje de veces que se obtuvo cada número del 1 al 6.
4. Mostrar un mensaje indicando cuál fue el número que más veces se obtuvo y su porcentaje correspondiente.

Tu tarea es escribir un programa que cumpla con estos requisitos, utilizando el módulo `random` de Python para simular los lanzamientos del dado.

**Ejemplo de ejecución:**
``` python
Bienvenido al simulador de lanzamiento de dado.

¿Cuántas veces deseas lanzar el dado? 1000

Resultados de los lanzamientos:
Lanzamiento 1: 3
Lanzamiento 2: 6
Lanzamiento 3: 1
...

Porcentaje de cada número:
Número 1: 16.2%
Número 2: 15.8%
Número 3: 16.7%
Número 4: 16.5%
Número 5: 16.1%
Número 6: 18.7%

El número que más veces se obtuvo fue el 6, con un 18.7% de los lanzamientos.
```
#### CODE

```python
import random

# Solicitar al usuario la cantidad de lanzamientos
num_lanzamientos = int(input("¿Cuántas veces deseas lanzar el dado? "))

# Inicializar un diccionario para almacenar los conteos de cada número
conteos = {1: 0, 2: 0, 3: 0, 4: 0, 5: 0, 6: 0}

# Realizar los lanzamientos y contar los resultados
for lanzamiento in range(num_lanzamientos):
    # Generar un número aleatorio entre 1 y 6 (inclusive)
    numero = random.randint(1, 6)
    # Incrementar el conteo del número obtenido
    conteos[numero] += 1

# Imprimir los resultados de cada lanzamiento
for numero, conteo in conteos.items():
    print(f"Lanzamiento {numero}: {conteo}")

# Calcular y mostrar el porcentaje de cada número
total_lanzamientos = sum(conteos.values())
for numero, conteo in conteos.items():
    porcentaje = (conteo / total_lanzamientos) * 100
    print(f"Número {numero}: {porcentaje:.1f}%")

# Encontrar el número que más veces se obtuvo
numero_mas_frecuente = max(conteos, key=conteos.get)
porcentaje_mas_frecuente = (conteos[numero_mas_frecuente] / total_lanzamientos) * 100
print(f"\nEl número que más veces se obtuvo fue el {numero_mas_frecuente}, con un {porcentaje_mas_frecuente:.1f}% de los lanzamientos.")

```
