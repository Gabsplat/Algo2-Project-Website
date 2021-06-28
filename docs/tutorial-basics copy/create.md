---
sidebar_position: 1
---

# Create

La función ***Create*** es la encargada de separar y guardar palabras en todos los archivos de la biblioteca virtual, para luego persistir esa información y así poder usarla para la función search.

Uso:
```bash
python personal_library.py -create 'path'
```

## Inserción de palabras en Trie

El proceso de inserción de palabras es el siguiente:
1. Primero se busca el último caractér de la palabra en el Trie
2. Se cambia el campo `isEndOfWord` por True (ya que es el final de la palabra)
3. En el caso de que no exista nada en el campo `files`, se cambia por una Linked List modificada
4. Una vez se tenga la lista, se procede a insertar el nombre del archivo y sumar una repetición

<img src="https://i.imgur.com/YM8SPCe.gif"/>  


## Complejidad temporal
La función tiene una complejidad promedio de `Θ(t*n*m)` siendo:
- `t`: cantidad de archivos
- `n`: cantidad de líneas en un archivo
- `m`: cantidad de caracteres por línea
