#ExercicesPython
Escribe un programa en Python que solicite al usuario ingresar una frase y luego cuente el número de palabras en esa frase. Una palabra se define como cualquier secuencia de caracteres separados por espacios en blanco. El programa debe imprimir el número total de palabras en la frase ingresada por el usuario.

Por ejemplo:
``` python
Ingrese una frase: "Python es un lenguaje de programación poderoso" 
Número de palabras: 6`
```

```python
def ContadorPalabras():
    frase = input("Escribe la frase que quieras que cuente las palabras: ")
    frase = frase.split(" ",)
    
    num_palabras = len(frase)
    print(f"Tu frase tiene {num_palabras} palabras.")
    
ContadorPalabras()
```
