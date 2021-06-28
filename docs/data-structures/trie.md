---
sidebar_position: 1
---

# Trie 

Como **estructura principal para el almacenamiento de datos** de la biblioteca virtual, se eligió la estructura Trie (o árbol n-ario).

La elección se fundamenta en base a la optimización del espacio requerido en memoria, en lo que Trie resulta una buena opción ya que permite minimizarlo.

Dadas las siguientes clases propias del árbol n-ario (Trie) vistas durante el cursado:

* **Trie**
* **TrieNode**

Se utilizó una modificación de un árbol n-ario (Trie) cuyo cambio es el siguiente:

* Se añadió a la clase **TrieNode** un campo extra, el cual se denomina 'files'.

Por lo que la clase TrieNode modificada queda de la siguiente manera:

``` python
class TrieNode:
    parent = None # nodo padre
    children = None # lista con nodos hijos
    key = None # caracter
    isEndOfWord = None # indicador fin de palabra
    files = None # campo nuevo
```

En el campo files agregado, se guardará una versión modificada de Linked List (explicada en el siguiente apartado).


## Complejidad temporal
### Inserción
| Caso | Complejidad | 
| ---- | :---------: |
| Peor | `O(m ǀΣǀ)` | 
| Promedio | `Θ(m)` |

### Búsqueda
| Caso | Complejidad |
| ---- | :---------: |
| Peor | `O(m ǀΣǀ)` |
| Promedio | `Θ(m)` |