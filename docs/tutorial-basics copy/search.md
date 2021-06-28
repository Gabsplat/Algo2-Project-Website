---
sidebar_position: 2
---

# Search

La función ***Search*** es la encargada de recuperar la información persistida por la función create, y devolver una lista de prioridades descendente con la cantidad de repeticiones de una palabra en los archivos de la biblioteca.

Uso:
```bash
python personal_library.py -search 'word'
```

## Proceso de búsqueda

El proceso de búsqueda es simple, ya que lo único que realiza es lo siguiente:
1. Se recupera los datos persistidos por pickle de la libreria
2. Luego, se busca en el Trie guardado la palabra
3. Si se encuentra, se procede a ordenar la lista en orden de prioridad descendente y se imprime en consola


## Complejidad temporal
La función tiene una complejidad en el peor caso de `O(m |Σ| + n)` siendo:
- `m`: tamaño de la palabra
- `|Σ|`: tamaño del diccionario
- `n`: cantidad de archivos en
