# 🎮 Simon Says: Motion Controlled Game via Inertial Sensors

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter Notebook](https://img.shields.io/badge/Made%20with-Jupyter-orange)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit_Learn-yellow)

Un juego interactivo de **"Simón Dice"** controlado por movimiento. Este proyecto utiliza un modelo de Machine Learning entrenado con datos de **sensores inerciales de un smartphone** (acelerómetro y giroscopio) para clasificar gestos del brazo y validar si el jugador siguió la secuencia correcta.


---

## 📖 Descripción del Proyecto

El objetivo de este proyecto es demostrar cómo los datos biométricos y de movimiento pueden ser utilizados para interfaces hombre-máquina (HMI). En lugar de usar botones o pantallas táctiles, el usuario interactúa con el juego realizando ejercicios físicos específicos.

El sistema captura la orientación y aceleración del dispositivo móvil, procesa estas señales para extraer características (features) y utiliza un modelo de clasificación para determinar qué movimiento se realizó.

## 🦾 Movimientos Reconocidos

El modelo ha sido entrenado para identificar 4 clases distintas de movimiento:

1.  **Rotación de Muñeca (Izquierda):** Giro de la mano sosteniendo el dispositivo hacia la izquierda.
2.  **Rotación de Muñeca (Derecha):** Giro de la mano hacia la derecha.
3.  **Levantamiento de Brazo:** Elevación vertical del brazo extendido.
4.  **Brazo a Hombro Opuesto:** Movimiento cruzado llevando la mano al hombro contrario.

## 📂 Estructura del Repositorio

El código está organizado en Notebooks de Jupyter para facilitar la visualización de datos y el entrenamiento:

```text
├── dataset_final_todas_caracteristicas.csv  # Dataset procesado con features extraídas
├── ExploratoryExtraccionCaracteristicas (1).ipynb # EDA y Extracción de Features (Media, Desv. Std, etc.)
├── modelTrainingSensadoFis.ipynb            # Entrenamiento y validación del modelo de ML
├── GameModelSimon1 (1).ipynb                # Lógica del juego "Simon Dice" e inferencia
└── README.md
