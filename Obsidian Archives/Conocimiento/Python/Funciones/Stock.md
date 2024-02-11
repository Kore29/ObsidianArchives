*Los Stocks son Funciones ya hechas que vienen con Python y nos facilita mucho mas el código*

Para empezar las tuplas y listas serian una función, función que se encarga de almacenar información como variables o otras listas
```python
numeros = [4,7,1,42]
```

La función `max` sirve para encontrar sobre una lista o tupla el numero (determinado por int) mas alto
```python
numero_mas_alto = max(numeros)
print(numero_mas_alto)
```

En este caso, como hay una función max, también hay una función que se llama `min` y es para encontrar el numero mas pequeño
```python
numero_mas_bajo = min(numeros)
print(numero_mas_bajo)
```

También hay una función donde se suman todos los valores numéricos, se llama `sum`.
```python
suma_total = sum(numeros)
print(suma_total)
```

Para redondear al decimal que tu quieras, tenemos una función llamada `round`, donde se le tienen que asignar dos valores, uno con el numero y otro con el numero de decimales.
```python
numero_round = round(12.34512,2)
print(numero_round)
## 12.34
```

La función `bool()` sirve para tomar un argumento y devolverte `True` si el argumento es considerado verdadero, o `False` si el argumento es considerado falso.
```python
resultado_bool = bool([9,12,True])
print(resultado_bool)
```

La función `all()` en Python se utiliza para determinar si todos los elementos en un iterable son evaluados como verdaderos.
```python
resultado_all = all(["hola",True,[344,23]])
print(resultado_all)
```