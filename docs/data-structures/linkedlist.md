---
sidebar_position: 2
---

# Linked List

Se utilizó una versión modificada de Linked List, la cual esta re-definida de la siguiente manera:

``` python
class filesList:
    head = None # primer nodo de la lista

class filesNode:
    nextNode = None # siguiente nodo de la lista
    fileName = None # nombre del archivo
    wordReps = 0 # cantidad de repeticiones
```

Esta estructura, utilizada en el campo files de la clase TrieNode, contiene la cantidad de repeticiones de cada palabra por archivo.

## Complejidad temporal
### Inserción
| Caso | Complejidad |
| ---- | :---------: |
| Promedio | `Θ(n)` |

### Búsqueda
| Caso | Complejidad |
| ---- | :---------: |
| Promedio | `Θ(n)` |
