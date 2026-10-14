# Otelo: búsqueda adversaria y aprendizaje automático

Proyecto realizado durante el curso 2025-2026 para la asignatura **Inteligencia Artificial**, en el que se desarrolla un agente capaz de jugar al juego de estrategia Otelo.

## Descripción

El proyecto estudia la aplicación de técnicas de inteligencia artificial a la toma de decisiones en juegos. El agente combina el algoritmo **Monte Carlo Tree Search (MCTS)** con la estrategia **Upper Confidence Bounds for Trees (UCT)** para explorar el árbol de jugadas y seleccionar movimientos prometedores.

Además, se genera información mediante partidas automáticas y se entrena una red neuronal convolucional para evaluar posiciones del tablero. Esta evaluación puede integrarse en la búsqueda para mejorar el comportamiento del agente frente a las simulaciones aleatorias.

## Tecnologías empleadas

- **Python** como lenguaje de programación.
- **NumPy** para la representación y manipulación de los tableros.
- **Pandas** para la lectura y el tratamiento de los datos de entrenamiento.
- **Keras y TensorFlow** para la creación, entrenamiento y carga de la red neuronal.
- **scikit-learn** para la división de los datos en conjuntos de entrenamiento y validación.
- **MCTS-UCT** como algoritmo de búsqueda adversaria.

## Estructura del proyecto

El proyecto se organiza en dos bloques principales:

- `docs`: documentación del proyecto en formato Word (`.docx`) y LaTeX (`.tex`).
- `src`: código fuente de la implementación.

Dentro de `src` se incluyen el motor del juego, el agente MCTS-UCT, la generación y lectura de datos y el entrenamiento del modelo neuronal.

## Autores

- Nuno José del Pino Escalante
- Javier Gutiérrez Pastor

## Instrucciones

Desde la carpeta src, se podrán ejecutar los archivos de la siguiente manera:

    Jugar al juego: python -m game.play_match
    Generar partidas para obtener datos: python -m game.game_generator
    Leer datos generados: python -m data.results_reader
    Generar modelo a partir de datos de entrenamiento: python -m agent.model.model

Nota: Si no se hace desde la carpeta src es muy probable que los scripts no se ejecutan correctamente.
