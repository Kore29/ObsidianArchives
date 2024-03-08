#FuncionesYModularidad #Metodos
## Métodos en Python

### Métodos para Listas (`list`)

- `append()`: Agrega un elemento al final de la lista.
- `insert()`: Inserta un elemento en una posición específica de la lista.
- `remove()`: Elimina el primer elemento de la lista con el valor especificado.
- `sort()`: Ordena los elementos de la lista en su lugar.
- `sorted()`: Devuelve una nueva lista ordenada con los elementos de la lista.

### Métodos para Tuplas (`tuple`)

- `count()`: Devuelve el número de veces que aparece un elemento en la tupla.
```python
mi_tupla = (1, 2, 2, 3, 4)
apariciones = mi_tupla.count(2)
print(apariciones)  # Salida: 2
```

- `index()`: Devuelve el índice de la primera aparición de un elemento en la tupla.
```python
mi_tupla = (1, 2, 3, 4, 5)
indice = mi_tupla.index(4)
print(indice)  # Salida: 3
```

### Métodos para Diccionarios (`dict`)

- `len()`: Devuelve el número de elementos (pares clave-valor) en el diccionario.
```python
mi_diccionario = {"a": 1, "b": 2, "c": 3}
longitud = len(mi_diccionario)
print(longitud)  # Salida: 3
```

- `keys()`: Devuelve una lista de las claves del diccionario.
```python
mi_diccionario = {"a": 1, "b": 2, "c": 3}
claves = mi_diccionario.keys()
print(claves)  # Salida: dict_keys(['a', 'b', 'c'])
```

- `values()`: Devuelve una lista de los valores del diccionario.
```python
mi_diccionario = {"a": 1, "b": 2, "c": 3}
valores = mi_diccionario.values()
print(valores)  # Salida: dict_values([1, 2, 3])
```

- `items()`: Devuelve una lista de tuplas, donde cada tupla contiene una clave y su valor correspondiente.
```python
mi_diccionario = {"a": 1, "b": 2, "c": 3}
items = mi_diccionario.items()
print(items)  # Salida: dict_items([('a', 1), ('b', 2), ('c', 3)])
```

### Métodos para Cadenas de Texto (`str`)

- `upper()`: Devuelve una copia de la cadena con todos los caracteres en mayúsculas.
- `lower()`: Devuelve una copia de la cadena con todos los caracteres en minúsculas.

- `strip()`: Este método devuelve una nueva cadena sin los espacios en blanco iniciales o finales.
```python
cadena = " Hola Mundo " 
print(cadena.strip()) # Output: "Hola Mundo"
```

- `split()`: Divide la cadena en subcadenas utilizando el delimitador especificado y devuelve una lista.
```python
texto = "Hola mundo"
palabras = texto.split(' ')
print(palabras)  # Salida: ['Hola', 'mundo']
```

- `join()`:  (JUNTAR) Une los elementos de una lista en una cadena utilizando el separador especificado.
```python
palabras = ['Hola', 'mundo']
texto_unido = ' '.join(palabras)
print(texto_unido)  # Salida: Hola mundo
```

<<<<<<< Updated upstream:Conocimiento/Python/Funciones y modularidad/Stock.md
- `srip()`: Remover los laterales de espacio, el `lstrip` y `rstrip` sirven solo para eliminar uno de los dos lados
```python
txt = "     banana     "  
x = txt.lstrip()  
print("of all fruits", x, "is my favorite")
```

- `isdigit()`: Comprueba si la variable es texto
```python
txt = "50800"  
x = txt.isdigit()
print(x)
```

=======
- `replace()` Para (REMPLAZAR) un dato str por otro
```python
cadena_original = "Hola mundo"
nueva_cadena = cadena_original.replace("mundo", "amigo")
# Salida = Hola amigo
```
>>>>>>> Stashed changes:Obsidian Archives/Conocimiento/Python/Funciones y modularidad/Stock.md
### Métodos para Conjuntos (`set`)

- `add()`: Agrega un elemento al conjunto.
- `remove()`: Elimina un elemento específico del conjunto. Genera un error si el elemento no está presente.
- `discard()`: Elimina un elemento específico del conjunto, si está presente. No genera error si el elemento no está presente.
- `pop()`: Elimina y devuelve un elemento aleatorio del conjunto.

### Métodos para Archivos (`file`)

- `read()`: Lee y devuelve el contenido completo del archivo como una cadena.
- `write()`: Escribe el contenido especificado en el archivo.
- `seek()`: Cambia la posición del cursor de lectura/escritura dentro del archivo.
- `close()`: Cierra el archivo.

### Métodos para Números (`int`, `float`)

- `abs()`: Devuelve el valor absoluto del número.
- `round()`: Redondea el número al entero más cercano.
- `is_integer()`: Devuelve `True` si el número es un entero, `False` si no lo es.
- `conjugate()`: Devuelve el conjugado del número complejo.