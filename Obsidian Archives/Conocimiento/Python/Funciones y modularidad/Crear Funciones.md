#FuncionesYModularidad 
En Python, una función es un bloque de código reutilizable que realiza una tarea específica. Las funciones son utilizadas para organizar y estructurar el código, permitiendo que se pueda dividir un programa en partes más pequeñas y manejables. Esto facilita la lectura, la depuración y la reutilización del código.

#### Función Simple

Aquí se define una función llamada `saludar` que no toma ningún parámetro. Simplemente imprime un saludo predefinido. Luego, la función es llamada.

```python
def saludar():
    print("Hola Marti, como estas?")
saludar()
```

#### Función con Parámetros

En este bloque, se define la función `saludar2` que toma dos parámetros (`nombre` y `sexo`). Dependiendo del valor del parámetro `sexo`, la función asigna un adjetivo diferente y luego imprime un saludo personalizado.

```python
def saludar2(nombre,sexo):
    sexo = sexo.lower()
    if (sexo == "mujer"):
        adjetivo = "reina"
    elif (sexo == "hombre"):
        adjetivo = "genio"
    else:
        adjetivo = "amor"
    print(f"Hola {nombre}, {adjetivo} ¿como estas?")
saludar2("Raul","HOmBre")
```

#### Función con Parámetros

En este bloque, se define la función `crear_contraseña_random` que toma un parámetro `num`. La función realiza algunos cálculos y luego devuelve una contraseña y el valor `num`. Luego, se desempaqueta el resultado de la función y se imprimen los valores.

```python
def crear_contraseña_random(num):
    caracter = "hijklmnñopq"
    numero_entero = str(num)
    num = int(numero_entero[2])
    c1 = num - 2
    c2 = num
    c3 = num - 5
    contraseña = f"{caracter[c1]}{caracter[c2]}{caracter[c3]}{num*2}"
    return contraseña,num
    
password,num = crear_contraseña_random(312)

password,num = crear_contraseña_random(312)
print(f"Tu contraseña nueva es {password}")
print(f"El numero utilizado para la contraseña es {num}")
```