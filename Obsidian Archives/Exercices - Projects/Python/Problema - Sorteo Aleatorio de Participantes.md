Problema: Eres el encargado de organizar un sorteo para un evento de tu universidad. Para hacerlo de manera justa y transparente, decides escribir un programa en Python que seleccione aleatoriamente a los ganadores entre los participantes inscritos. Cada participante tiene un número de identificación único, que va desde 1 hasta el número total de inscritos.

Escribe un programa en Python que realice lo siguiente:

1. Solicite al usuario ingresar el número total de participantes.
2. Genere aleatoriamente tres números de identificación de ganadores entre 1 y el número total de participantes.
3. Imprima los números de identificación de los tres ganadores.

Recuerda utilizar el módulo `random` de Python para generar los números aleatorios.
#### CODE

```python
import random

def sorteo():
    num_participantes = int(input("Ingrese el numero de participantes total: "))
    if num_participantes < 3:
        print("Se necesita un maximo de 3 personas para hacer el sorteo.")
        return

    ganadores = random.sample(range(1,num_participantes),3)
    for ganador in ganadores:
        print(ganador)

sorteo()
```

*Cosas a destacar*
```python
ganadores = random.sample(range(1,num_participantes),3)
```
- Utilizamos el asset `random` para extraer tres ganadores, utilizamos el `sample` que nos hace escoger un numero (o cualquier cosa) dentro de una variable o lista y cuantas veces lo queremos repetir, en este caso 3, pero pueden ser repetidas, para eso optamos por ponerle al `num_participantes + 1` para que si o si el numero este sumado y no se pueda repetir 

Si pusiésemos `print(ganadores)` el output seria `[1, 15, 13]` y para evitarnos eso y tenerlo mas limpio, ponemos un `for x in y` :
```python    
for ganador in ganadores:
        print(ganador)
```
![[Output For.png]]
