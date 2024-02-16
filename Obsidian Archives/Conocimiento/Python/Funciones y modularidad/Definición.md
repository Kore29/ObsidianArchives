### Que es una función?

una función es un bloque de código reutilizable que realiza una tarea específica. Las funciones permiten dividir un programa en partes más pequeñas y manejables, lo que facilita el desarrollo, la depuración y el mantenimiento del código.

Una función en Python se define mediante la palabra clave `def`, seguida del nombre de la función y paréntesis que pueden contener argumentos

```python
def nombre_de_la_funcion(argumento1, argumento2):
    # Cuerpo de la función
    # Realizar alguna tarea
    resultado = argumento1 + argumento2
    return resultado
```

En este ejemplo, **nombre_de_la_funcion** es el nombre de la función, y toma dos argumentos **argumento1** y **argumento2.** El cuerpo de la función realiza una tarea específica, en este caso, suma los dos argumentos y devuelve el resultado con la instrucción **return**.

```python
resultado_de_suma = nombre_de_la_funcion(5, 3) 
print(resultado_de_suma) # Esto imprimirá 8
```