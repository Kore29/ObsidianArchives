## Crear set Python

Los `set` en Python son un tipo que permite almacenar varios elementos y acceder a ellos de una forma muy **similar a las listas** pero con ciertas diferencias:

- Los elementos de un set son **único**, lo que significa que no puede haber elementos duplicados.
- Los set son **desordenados**, lo que significa que no mantienen el orden de cuando son declarados.
- Sus elementos deben ser **inmutables**.

Para entender mejor los `sets`, es necesario entender ciertos conceptos matemáticos como la **teoría de conjuntos**.

Para **crear** un set en Python se puede hacer con `set()` y pasando como entrada cualquier tipo iterable, como puede ser una lista. Se puede ver como a pesar de pasar elementos duplicados como dos `8` y en un orden determinado, al imprimir el set no conserva ese orden y los duplicados se han eliminado.

```python
s = set([5, 4, 6, 8, 8, 1])
print(s)       #{1, 4, 5, 6, 8}
print(type(s)) #<class 'set'>
```

Se puede hacer lo mismo haciendo uso de `{}` y sin usar la palabra `set()` como se muestra a continuación.

```python
s = {5, 4, 6, 8, 8, 1}
print(s)       #{1, 4, 5, 6, 8}
print(type(s)) #<class 'set'>
```

## Operaciones con sets

A diferencia de las listas, en los set no podemos modificar un elemento a través de su índice. Si lo intentamos, tendremos un `TypeError`.

```python
s = set([5, 6, 7, 8])
#s[0] = 3 #Error! TypeError
```

Los elementos de un `set` deben ser **inmutables**, por lo que un elemento de un `set` no puede ser ni un diccionario ni una lista. Si lo intentamos tendremos un `TypeError`

```python
lista = ["Perú", "Argentina"]
#s = set(["México", "España", lista]) #Error! TypeError
```

Los `sets` se pueden iterar de la misma forma que las listas.

```python
s = set([5, 6, 7, 8])
for ss in s:
    print(ss) #8, 5, 6, 7
```

Con la función `len()` podemos saber la longitud total del `set`. Como ya hemos indicado, los duplicados son eliminados.

```python
s = set([1, 2, 2, 3, 4])
print(len(s)) #4
```

También podemos saber si un elemento está presente en un set con el operador `in`. Se el valor existe en el set, se devolverá `True`.

```python
s = set(["Guitarra", "Bajo"])
print("Guitarra" in s) #True
```

Los `sets` tienen además diferentes funcionalidades, que se pueden aplicar en forma de operador o de método. Por ejemplo, el operador `|` nos permite realizar la **unión** de dos sets, lo que equivale a juntarlos. El equivalente es el método `union()` que vemos a continuación.

```python
s1 = set([1, 2, 3])
s2 = set([3, 4, 5])
print(s1 | s2) #{1, 2, 3, 4, 5}
```

## Métodos sets
#### `s.add(<elem>)`

El método `add()` permite añadir un elemento al `set`.

```python
l = set([1, 2])
l.add(3)
print(l) #{1, 2, 3}
```
#### `s.remove(<elem>)`

El método `remove()` elimina el elemento que se pasa como parámetro. Si no se encuentra, se lanza la excepción `KeyError`.

```python
s = set([1, 2])
s.remove(2)
print(s) #{1}
```
#### `s.discard(<elem>)`

El método `discard()` es muy parecido al `remove()`, borra el elemento que se pasa como parámetro, y si no se encuentra no hace nada.

```python
s = set([1, 2])
s.discard(3)
print(s) #{1, 2}
```
#### `s.pop()`

El método `pop()` elimina un elemento aleatorio del `set`.

```python
s = set([1, 2])
s.pop()
print(s) #{2}
```
#### `s.clear()`

El método `clear()` elimina todos los elementos de `set`.

```python
s = set([1, 2])
s.clear()
print(s) #set()
```

### Otros

Los `sets` cuentan con una gran cantidad de métodos que permiten realizar operaciones con dos o más, como la **unión** o la **intersección**.

Podemos calcular la **unión** entre dos sets usando el método `union()`. Esta operación representa la “mezcla” de ambos sets. Nótese que el método puede ser llamado con más parámetros de entrada, y su resultado será la unión de todos los sets.

```python
s1 = {1, 2, 3}
s2 = {3, 4, 5}
print(s1.union(s2)) #{1, 2, 3, 4, 5}
```

También podemos calcular la **intersección** entre dos o más set. Su resultado serán aquellos elementos que pertenecen a ambos sets.

```python
s1 = {1, 2, 3}
s2 = {3, 4, 5}
print(s1.intersection(s2)) #{3}
```

Los `set` en Python tiene gran cantidad de métodos, por lo que lo dejaremos para otro capítulo, pero aquí os dejamos con un listado de ellos:

- `s1.union(s2[, s3 ...])`
- `s1.intersection(s2[, s3 ...])`
- `s1.difference(s2[, s3 ...])`
- `s1.symmetric_difference(s2)`
- `s1.isdisjoint(s2)`
- `s1.issubset(s2)`
- `s1.issuperset(s2)`
- `s1.update(s2[, s3 ...])`
- `s1.intersection_update(s2[, s3 ...])`
- `s1.difference_update(s2[, s3 ...])`
- `s1.symmetric_difference_update(s2)`