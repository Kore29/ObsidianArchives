#FuncionesYModularidad
#### Que es Lamda?

La palabra clave `lambda` en Python se utiliza para crear funciones anónimas, también conocidas como funciones lambda. Estas son funciones pequeñas y temporales que se pueden definir de manera concisa en una sola línea de código. La sintaxis básica de una función lambda es:

```python
lambda argumentos: expresion
```

- `lambda`: Es la palabra clave que indica que estás creando una función lambda.
- `argumentos`: Son los parámetros de la función. Puedes tener cero o más argumentos, pero la sintaxis más común es tener uno o más separados por comas.
- `expresion`: Es la expresión que se evalúa y devuelve como resultado de la función.

```python
multiplicar_por_dos = lambda x: x * 2
def multiplicar_por_dos(x): return x * 2
```
#### Que es Filter?

La función `filter` en Python se utiliza para filtrar elementos de una secuencia (como una lista) según una función dada. La función `filter` devuelve un objeto de tipo `filter`, que es iterable y contiene solo los elementos de la secuencia que cumplen con la condición especificada en la función.

La sintaxis básica de la función `filter` es la siguiente:

```python
filter(función, secuencia)
```

- `función`: Es la función que se aplica a cada elemento de la secuencia. Solo se incluyen en el resultado aquellos elementos para los cuales la función devuelve `True`.
- `secuencia`: Es la secuencia de elementos que se desea filtrar.

```python
# Definir una función para verificar si un número es par
def es_par(numero):
    return numero % 2 == 0

# Lista de números
numeros = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
# Usar filter para obtener solo los números pares
numeros_pares = filter(es_par, numeros)
# Convertir el resultado a una lista
lista_pares = list(numeros_pares)

print(lista_pares)
```

En este ejemplo, la función `es_par` se aplica a cada elemento de la lista `numeros`. La función `filter` filtra solo los números pares, y el resultado se convierte en una lista que se imprime al final.

Es importante mencionar que también se puede utilizar una función lambda en lugar de definir una función por separado, como se mostró en uno de tus ejemplos anteriores:

```python
# Usar filter con una función lambda para obtener solo los números pares
numeros_pares = filter(lambda numero: numero % 2 == 0, numeros)
```

Esto logra el mismo resultado que el ejemplo anterior utilizando una función lambda en lugar de una función definida con `def`.

#### Funciones Datos Compuestos

Tanto las listas como las tuplas son tipos de datos en Python que se utilizan para almacenar colecciones ordenadas de elementos

- *Funciones generales*
``len() Devuelve el número de elementos (pares clave-valor) en el diccionario.

``dict() Constructor de diccionarios. Puede crear un diccionario vacío o convertir otros tipos de datos en diccionarios.

``sorted() Devuelve una lista de las claves del diccionario ordenadas.
