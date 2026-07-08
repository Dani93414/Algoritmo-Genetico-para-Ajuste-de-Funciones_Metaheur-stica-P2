# Algoritmo Genético para Ajuste de Funciones — Metaheurística P2

Proyecto desarrollado para la asignatura de Metaheurística.  
Implementa un algoritmo genético en Python para ajustar una función a un conjunto de puntos mediante la optimización de sus coeficientes.

El objetivo es comparar distintas combinaciones de operadores genéticos y analizar su comportamiento mediante métricas y gráficas.

---

## Descripción

El algoritmo busca minimizar el error entre valores reales y valores predichos por una función de la forma:

```txt
f(x) = exp(a) + b·x + c·x² + d·x³ + e·x⁴ + g·x⁵ + h·x⁶ + i·x⁷
