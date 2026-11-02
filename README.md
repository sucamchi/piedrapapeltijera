# Piedra, Papel o Tijera

![Python](https://img.shields.io/badge/Python-3-3776AB?logo=python&logoColor=white)
![Sin dependencias](https://img.shields.io/badge/dependencias-ninguna-brightgreen)

El clásico juego de piedra, papel o tijera contra el ordenador, en la
terminal. Escribes tu jugada, el ordenador elige la suya al azar y el
marcador se va actualizando ronda a ronda hasta que decides salir.

## Cómo jugar

```bash
python3 rock-paper-scissors.py
```

```
Enter your choice (rock, paper, scissors) or 'quit' to exit: rock
computer chose: scissors
You win!
User: 1 Computer: 0
Enter your choice (rock, paper, scissors) or 'quit' to exit: paper
It's a tie!
User: 1 Computer: 0
Enter your choice (rock, paper, scissors) or 'quit' to exit: quit
```

El juego está en inglés: escribe `rock`, `paper` o `scissors` (da igual si
es en mayúsculas o minúsculas) y `quit` para terminar. Cualquier otra
palabra se rechaza y se vuelve a preguntar.

## Reglas

| Tú | Ordenador | Resultado |
|----|-----------|-----------|
| piedra | tijera | ganas |
| papel | piedra | ganas |
| tijera | papel | ganas |
| piedra | papel | gana el ordenador |
| papel | tijera | gana el ordenador |
| tijera | piedra | gana el ordenador |
| lo mismo | lo mismo | empate |

## Lo que aprendí

- Un bucle `while True` que solo termina con `break`, el patrón típico de
  los juegos por turnos
- Leer la entrada del usuario con `input()` y normalizarla con `.lower()`
- Elegir al azar con `random.choice()`
- Combinar condiciones con `and` / `or` para codificar las reglas
- Guardar el estado (el marcador) en variables que sobreviven entre rondas
- Validar la entrada y volver a preguntar en vez de fallar
