# ListasEnlazadasNodeJS

Scaffolding de referencia para migrar la logica de `SinglyLinkedList` y `DoublyLinkedList` desde Java hacia Node.js.

## Objetivo

- Mantener la misma idea de responsabilidades por clase.
- Replicar metodos y comportamiento del proyecto Java.
- Tener ejemplos base para que estudiantes completen o extiendan.

## Estructura

```text
src/
  index.js
  challenges/
    linkedListChallenges.js
  structures/
    simple/
      SimpleNode.js
      SinglyLinkedList.js
    doubly/
      DoublyNode.js
      DoublyLinkedList.js
  examples/
    simpleListExample.js
    doublyListExample.js
    migrationGuideExample.js
```

## Ejecutar

```bash
npm install
npm run demo
```

## Mapa Java -> Node.js

- `addFirst(T value)` -> `addFirst(value)`
- `addLast(T value)` -> `addLast(value)`
- `removeFirst()` -> `removeFirst()`
- `removeLast()` -> `removeLast()`
- `countOccurrences(T value)` -> `countOccurrences(value)`
- `reverseInPlace()` -> `reverseInPlace()`
- `removeDuplicates()` -> `removeDuplicates()`

## Retos pendientes para estudiantes

En este scaffold, igual que en Java, los metodos de reto quedan con `TODO` y
`throw new Error(...)` para que el estudiante los implemente:

- `SinglyLinkedList.countOccurrences(value)`
- `SinglyLinkedList.clean()`
- `SinglyLinkedList.reverseInPlace()`
- `SinglyLinkedList.removeDuplicates()`
- `DoublyLinkedList.countOccurrences(value)`
- `DoublyLinkedList.clean()`
- `DoublyLinkedList.reverseInPlace()`
- `DoublyLinkedList.removeDuplicates()`

Puedes ejecutar `src/challenges/linkedListChallenges.js` desde `src/index.js` para
ver qué está pendiente y cuál es el resultado esperado por cada reto.

## Recomendacion didactica

1. Comparar archivo Java vs Node metodo por metodo.
2. Implementar primero operaciones basicas.
3. Validar invariantes: `head`, `tail`, `size`.
4. Resolver retos avanzados sin estructuras auxiliares.
