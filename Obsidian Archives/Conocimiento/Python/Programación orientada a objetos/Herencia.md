Digamos que tenemos 2 clases, una es el padre y el potro el hijo.
Para conservar los datos del padre al hijo se utiliza herencia, *un ejemplo:*
```python
# El padre
class Croquetas:
	def __init__(self,tamaño,textura)
		self.tamaño = tamaño
		self.textura = textura

# El hijo
class CroquetasJamon(Croquetas)
	def __init__(self,tamaño,textura,ingrediente)
		super().__init__(tamaño,textura)
		self.ingrediente = ingrediente
```

Te preguntaras, que coño ha pasado aquí? Es normal, ahora te lo explico
*La clase Croquetas tenia diversos atributos como el tamaño y la textura, nosotros hemos hecho una sub división y hemos añadido CroquetasJamon, y en esta clase hemos añadido un nuevo atributo llamado ingredientes, ahora bien, como se hace esto? Bien sencillo*

el super(). es para añadir los atributos que vas ha heredar de la clase padre.
Y debajo se añade como siempre el/los atributo/s nuevos, listo, ya lo tienes.