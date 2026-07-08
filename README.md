# Algoritmo Genético para Ajuste de Funciones — Metaheurística P2

Proyecto desarrollado para la asignatura de **Metaheurística**.

Este proyecto implementa un algoritmo genético en Python para ajustar una función a un conjunto de puntos mediante la optimización de sus coeficientes.

El objetivo es comparar distintas combinaciones de operadores genéticos y analizar su comportamiento mediante métricas y gráficas.

---

## Descripción

El algoritmo busca minimizar el error entre valores reales y valores predichos por una función de la forma:

```txt
f(x) = exp(a) + b·x + c·x² + d·x³ + e·x⁴ + g·x⁵ + h·x⁶ + i·x⁷
```

Cada individuo representa un conjunto de coeficientes:

```txt
[a, b, c, d, e, g, h, i]
```

La calidad de cada individuo se evalúa mediante el **error cuadrático medio** entre los valores reales y los valores predichos.

---

## Funcionalidades

* Generación de población inicial aleatoria.
* Evaluación de individuos mediante error cuadrático medio.
* Selección de padres mediante diferentes estrategias.
* Cruce de individuos con varios operadores.
* Mutación adaptativa.
* Elitismo para conservar la mejor solución.
* Ejecución de múltiples pruebas.
* Comparación de combinaciones de operadores.
* Generación automática de gráficas.
* Análisis de convergencia y rendimiento.

---

## Operadores implementados

### Selección

* Torneo binario.
* Ruleta.
* Muestreo estocástico universal.
* Emparejamiento variado inverso.

### Cruce

* Cruce uniforme.
* Cruce por un punto.
* Cruce BLX-alpha.
* Cruce aritmético simple.

### Mutación

* Mutación gaussiana.
* Mutación por intercambio.
* Mutación uniforme.

---

## Estructura del proyecto

```txt
Metaheur-stica-P2/
├── main.py
├── algoritmo.py
├── graficas.py
├── operadores/
│   ├── seleccion.py
│   ├── cruce.py
│   └── mutacion.py
└── resultados/
```

---

## Tecnologías utilizadas

* Python
* NumPy
* Matplotlib
* Seaborn

---

## Ejecución

Instala las dependencias principales:

```bash
pip install numpy matplotlib seaborn
```

Ejecuta el programa:

```bash
python main.py
```

El programa mostrará un menú para elegir entre:

* combinación manual de operadores,
* combinación predefinida.

---

## Resultados generados

Los resultados se guardan automáticamente en la carpeta:

```txt
resultados/
```

Para cada combinación se generan gráficas como:

* distribución del fitness final,
* tiempo de ejecución,
* evolución del tamaño de población,
* número de cruces y mutaciones,
* comparación entre valores reales y predichos,
* fitness frente a tamaño de población,
* generaciones hasta convergencia,
* mejor fitness y error medio por generación.

---

## Objetivo académico

El proyecto permite estudiar cómo afectan los operadores genéticos al rendimiento de un algoritmo evolutivo, analizando:

* calidad de la solución,
* velocidad de convergencia,
* estabilidad entre ejecuciones,
* impacto del tamaño de población,
* comportamiento de la mutación adaptativa.

---

## Estado del proyecto

Proyecto académico funcional para experimentación con algoritmos genéticos y comparación de operadores metaheurísticos.

---

## Autores

* Daniel Grande Rubio — [@Dani93414](https://github.com/Dani93414)
* Carlos de la Torre Frías — [@CarlosDT191](https://github.com/CarlosDT191)
* Manuel Eddy Ruiz Rivera — [@i12rurim](https://github.com/i12rurim)
