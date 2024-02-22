#TiposDeDatosBasicos
Los datos compuestos como bien dice su nombre son tipos de datos generados en "paquetes" que se pueden asignar en diferentes tipos de conjuntos
### Listas
En este caso tenemos una lista, la lista sirve para poder modificar los datos.
```python 
list = ["Marti", "Pablo", True, 192.12]

list[3] = "Subnormal"

print(list[3])
```
### Tuplas
Las tuplas son como las **listas** pero con la diferencia que no se pueden modificar.
```python
tuplas = ("Marti", "Pablo", True, 192.12)
print(tuplas[3])
```
*En caso que queramos cambiar algo de la tupla nos marcara error.*
```python
tuplas[1] = "Marcos"
```
![[ErrorTuplas.png]]
### Set
Un set, y al igual que una **tupla**, no se puede modificar ni enseñar el interior, pero si el **conjunto**.
```python
conjunto = {"Marti", "Pablo", True, 192.12}
conjunto = {"jajajaj tus muertos pisoteados a caballo"}
```
### Diccionario
Un diccionario es como una lista pero en vez de definir las variables por números las **defines tu por nombres**.
```python
    "nombre" : "Marti Castaño", #0 nombre

    "clave" : "Pinturo", #1 clave

    "estoy enfadado" : False, #2 estoy enfadado

    "altura" : 1.23 #3 altura
```

### Items
El método `items()` en Python se utiliza para obtener una vista de tuplas que contiene todos los pares clave-valor en un diccionario. Cada tupla en esta vista representa un par clave-valor, donde el primer elemento de la tupla es la clave y el segundo elemento es el valor asociado a esa clave en el diccionario.

Por ejemplo, considera el siguiente diccionario:
```python
mi_diccionario = {'a': 1, 'b': 2, 'c': 3}
```
Si llamamos al método `items()` en este diccionario, obtendremos una vista de tuplas que contiene todos los pares clave-valor:
```python
print(mi_diccionario.items())
# Salida: dict_items([('a', 1), ('b', 2), ('c', 3)])
```
Esta vista se puede iterar usando un bucle `for`, y en cada iteración, obtendremos una tupla que representa un par clave-valor:
```python
for clave, valor in mi_diccionario.items():
    print(f"Clave: {clave}, Valor: {valor}")
```
En este bucle, `clave` y `valor` son variables que representan la clave y el valor respectivamente en cada par clave-valor del diccionario. Usando este método, podemos iterar fácilmente sobre todos los elementos de un diccionario y realizar operaciones en ellos.

En resumen, el método `items()` es útil cuando necesitamos trabajar con los pares clave-valor de un diccionario de una manera conveniente y eficiente.