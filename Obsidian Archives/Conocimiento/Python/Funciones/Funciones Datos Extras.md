
#### Función con Tres Parámetros y Clave Forzosa

En este bloque de código, se define la función `frase` que toma tres parámetros (`nombre`, `apellido`, y `adjetivo`). La función retorna una frase utilizando estos parámetros. Se utiliza una clave forzosa de argumentos al llamar a la función.

```python
def frase(nombre, apellido, adjetivo):     
	return f"Hola {nombre} {apellido}, eres un {adjetivo}"

frase_resultante = frase(nombre="Marti", apellido="Castaño", adjetivo="genio") print(frase_resultante)
```


#### Función con Clave y Argumento Opcional

En este bloque, se define la función `frase2` que toma tres parámetros (`nombre2`, `apellido2`, y `adjetivo2`). 

La novedad es que el parámetro `adjetivo2` tiene un valor predeterminado ("Tonto"), lo que lo convierte en opcional. Luego, se llama a la función sin proporcionar el tercer argumento opcional.

```python
def frase2(nombre2,apellido2,adjetivo2="Tonto"):
    return f"Hola {nombre2} {apellido2}, eres un {adjetivo2}"

frase_resultante2 = frase("Marti","Castaño","gilipolas")
print(frase_resultante2)
```
