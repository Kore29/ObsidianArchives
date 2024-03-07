#ControlDeFlujo 
### 1. Condicionales.
#### 1.1. `Condicional If
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

#### 1.2. `Condicional Elif
El condicional Elif sirve como condicional **EXTRA** de cualquier variable que tengamos que condicionar
```python
edad = 20
if edad >= 18:
	print("Eres mayor de edad")
# En este caso utilizaremos un Elif para mostrar otro condicional
elif edad >= 40
	print("Eres bastante mayor")
```
 
#### 1.3. `Condicional Else
El condicional Else es parecido al Elif, con la diferencia que se utiliza en vez de como único condicional como el contrario de los condicionales if y Elif que hayamos asignado
```python
edad = 20
if edad >= 18:
	print("Eres mayor de edad")
elif:
# Es decir, lo contrario de mayor de 18 es menor de 18
	print("No eres mayor de edad")
```

### 2. Operadores Para Condicionales.
#### 2.1. `Operadores de Comparación

```python
#Nos devolverá True o False en condiciones que pongamos en nuestras comparaciones
es_igual_que = 5 == 6         # False
es_distinto_de = 5 != 6       # True
mayor_que = 5 > 6             # False
menor_que = 5 < 6             # True
mayor_o_igual = 5 <= 6        # True
```

En resumen, estás utilizando los operadores de comparación para evaluar expresiones y determinar si son verdaderas o falsas. Las variables `es_igual_que`, `es_distinto_de`, `mayor_que`, `menor_que`, y `mayor_o_igual` almacenan resultados de comparaciones. 
#### 2.2. `Cálculos Combinados

```python
a = 5
b = 10
c = 20
comparacion0 = a + b == c      # True, ya que 5 + 10 = 15, y 15 es igual a c (20)
comparacion1 = a + b < c       # True, ya que 5 + 10 = 15, y 15 es menor que c (20)
```

#### 2.3. `Comparación de Contraseñas

```python
contraseña_guardada = "Pan"
contraseña_escrita = "Papa"
print(contraseña_guardada == contraseña_escrita)  #False, las contraseñas no son iguales
```

Además, las variables `comparacion0` y `comparacion1` se utilizan para realizar cálculos combinados y evaluar expresiones más complejas. La última impresión compara dos contraseñas, y en este caso, devuelve `False` ya que las contraseñas son diferentes.
