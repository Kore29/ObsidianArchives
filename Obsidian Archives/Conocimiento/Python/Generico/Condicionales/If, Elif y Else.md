## Condicional If
El condicional **if** es una estructura de control en Python que permite que un bloque de código se ejecute solo si una **condición especificada** es verdadera

*La estructura básica de un condicional *if* es la siguiente:*
```python
if condición:
    # bloque de código que se ejecutará si la condición es verdadera
```

Si la condición es verdadera, el bloque de código dentro del condicional **if** se ejecutará. Si la condición es falsa, el bloque de código se omitirá y el programa continuará ejecutando el código después del condicional.

*Un ejemplo sencillo:*
```python
edad = 20

if edad >= 18:
    print("Eres mayor de edad")
```

## Condicional Elif
El condicional Elif sirve como condicional **EXTRA** de cualquier variable que tengamos que condicionar
```python
edad = 20
if edad >= 18:
	print("Eres mayor de edad")
# En este caso utilizaremos un Elif para mostrar otro condicional
elif edad >= 40
	print("Eres bastante mayor")
```
 
## Condicional Else
El condicional Else es parecido al Elif, con la diferencia que se utiliza en vez de como único condicional como el contrario de los condicionales if y Elif que hayamos asignado
```python
edad = 20
if edad >= 18:
	print("Eres mayor de edad")
elif:
# Es decir, lo contrario de mayor de 18 es menor de 18
	print("No eres mayor de edad")
```

