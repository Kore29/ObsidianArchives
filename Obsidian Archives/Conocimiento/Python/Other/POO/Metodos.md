Los métodos son funciones, para no calentarse la cabeza, que puedes crear tu mismo, pero de vez en cuando para poo nos viene bien para asignarles "acciones" a estas clases.

Imagínate que tenemos una persona, y esa persona tiene unas cualidades, (tipo de ropa, altura, cultura, caracter...) Pero quiero que esa persona haga una acción, podemos crearla como un método. Aquí un ejemplo.

```python
class Persona:
	def __init__(self, altura, pais, caracter)
		self.altura = altura
		self.pais = pais
		self.caracter = caracter
	
	# Asignamos otro metodo (puede ser el que nosotros queramos)
	def presentacion(altura ,pais, caracter)
		print(f"hola, mido {self.altura} y soy de {self.pais}")
	
```

Ahora que entiendes un poco el concepto de los Métodos, te preguntaras que método es `_init_` y para que sirve `self`? no?

## Métodos Especiales

Ahora que entiendes un poco el concepto de los Métodos, te preguntaras que método es `_init_` y para que sirve `self`? no? El `_init_` es un constructor.

Pero Martí, ¿Qué es un constructor? (Explicación para tontos)

*Imagina que estás fabricando juguetes en una fábrica. Cada juguete es un objeto y tiene algunas características, como su color y tamaño. Para asegurarte de que cada juguete tenga las características correctas cuando se fabrica, usas una máquina especial llamada "constructor de juguetes". Esta máquina toma el color y el tamaño como entrada y crea un juguete con esas características.*

Tengamos como referencia que una clase es como esa máquina, y el "constructor de juguetes" es como el método `__init__()` en una clase. El método `__init__()` se utiliza para crear un objeto (juguete) y configurarlo con las características adecuadas (atributos).

```python
# Definimos una clase para representar juguetes
class Juguete:
    def __init__(self, color, tamano):
        self.color = color
        self.tamaño = tamano
```

En este código, `Juguete` es la clase que representa los juguetes. El método `__init__()` es como la máquina que crea los juguetes. Toma dos argumentos: `self` (que es una referencia al juguete que estamos creando) y los valores para `color` y `tamaño`. Luego, el método `__init__()` configura el juguete recién creado con el color y el tamaño proporcionados.

Ahora, cuando creamos un juguete, usamos la clase `Juguete` y el método `__init__()`:

```python
# Creamos un juguete rojo y pequeño
mi_juguete = Juguete("rojo", "pequeño")

# Podemos acceder a las características del juguete
print(mi_juguete.color)   # Imprime "rojo"
print(mi_juguete.tamaño)  # Imprime "pequeño"
```

Entonces, el método `__init__()` es como el proceso de construcción que asegura que cada objeto (en este caso, cada juguete) tenga las características adecuadas cuando se crea. Es una parte esencial de la programación orientada a objetos en Python.