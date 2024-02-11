https://developer.mozilla.org/es/docs/Learn/Getting_started_with_the_web/HTML_basics#entonces_%C2%BFqu%C3%A9_es_html_en_realidad

El Lenguaje de Marcado de Hipertexto (HTML) es el código que se utiliza para estructurar y desplegar una página web y sus contenidos. Por ejemplo, sus contenidos podrían ser párrafos, una lista con viñetas, o imágenes y tablas de datos. Como lo sugiere el título, este artículo te dará una comprensión básica de HTML y cúal es su función.

HTML no es un lenguaje de programación; es un _lenguaje de marcado_ que define la estructura de tu contenido. HTML consiste en una serie de elementos que usarás para encerrar diferentes partes del contenido para que se vean o comporten de una determinada manera.

```html
Mi gato es muy gruñon
```

Si quieres especificar que se trata de un párrafo, podrías encerrar el texto con la etiqueta de párrafo [[<p/>]]

```html
<p>Mi gato es muy gruñon</p>
```


![[grumpy2.png]]

##### **Las partes principales del elemento son:**

1. **La etiqueta de apertura**: consiste en el nombre del elemento (en este caso, p), encerrado por **paréntesis angulares** (< >) de apertura y cierre. Establece dónde comienza o empieza a tener efecto el elemento —en este caso, dónde es el comienzo del párrafo—.

2. **La etiqueta de cierre**: es igual que la etiqueta de apertura, excepto que incluye una barra de cierre (/) antes del nombre de la etiqueta. Establece dónde termina el elemento —en este caso dónde termina el párrafo—.

3. **El contenido**: este es el contenido del elemento, que en este caso es sólo texto.

4. **El elemento**: la etiqueta de apertura, más la etiqueta de cierre, más el contenido equivale al elemento.

**Los elementos pueden también tener atributos, que se ven así:**

![[grumpy.png]]

Los atributos contienen información adicional acerca del elemento, la cual no quieres que aparezca en el contenido real del elemento. Aquí `class` es el _nombre_ del atributo y `editor-note` el _valor_ del atributo. En este caso, el atributo `class` permite darle al elemento un nombre identificativo, que se puede utilizar luego para apuntarle al elemento información de estilo y demás cosas.

##### Un atributo debe tener siempre:

1. Un espacio entre este y el nombre del elemento (o del atributo previo, si el elemento ya posee uno o más atributos). 
2. El nombre del atributo, seguido por un signo de igual (**=**).
3. Comillas de apertura y de cierre, encerrando el valor del atributo.

**Nota:** *el atributo con valores simples que no contengan espacios en blanco ASCII (o cualesquiera de los caracteres `"` `'` `` ` `` `=` `<` `>`) pueden permanecer sin entrecomillar, pero se recomienda entrecomillar todos los valores de atributo, ya que esto hace que el código sea más consistente y comprensible*

### Anidar elementos

Puedes también colocar elementos dentro de otros elementos —esto se llama **anidamiento**—. Si, por ejemplo, quieres resaltar una palabra del texto (en el ejemplo la palabra «muy»), podemos encerrarla en un elemento [[Strong]], que significa que dicha palabra se debe enfatizar:

```html
<p>Mi gato es <strong>muy</strong> gruñon.</p>
```

Debes asegurarte que los elementos estén correctamente anidados: en el ejemplo de abajo, creaste la etiqueta de apertura del elemento [`<p>`] primero, luego la del elemento [[Strong]], por lo tanto, debes cerrar esta etiqueta primero, y luego la de ``<p>``. Esto es incorrecto:

```html
<p>Mi gato es <strong>muy gruñon.</p></strong>
```

Los elementos deben abrirse y cerrarse ordenadamente, de forma tal que se encuentren claramente dentro o fuera el uno del otro. Si estos se encuentran solapados, el navegador web tratará de adivinar lo que intentas decirle, pero puede que obtengas resultados inesperados. Así que, ¡no lo hagas!