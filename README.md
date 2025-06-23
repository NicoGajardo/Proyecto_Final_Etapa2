# Proyecto_Final_Etapa2
Pryecto Final - Curso de Machine Learning - DSI-2025/I

# Proyecto Final: Etapa 2  
### Desarrollo del Prototipo Computacional y Documentación Técnica  
**Autor:** Nicolás Gajardo Sepúlveda

## Descripción General

Este proyecto desarrolla un sistema de evaluación basado en modelos de aprendizaje automático para reducir el esfuerzo computacional requerido al ejecutar simulaciones hidráulicas en redes de distribución de agua (RDA). El enfoque se centra en la evaluación de configuraciones de diseño y operación de Estaciones de Bombeo (EB), mediante dos modelos:

- **Clasificación:** Estima la factibilidad de una solución (factible o no factible).
- **Regresión:** Predice las presiones de operación en función del caudal suministrado.

## Contenido del Notebook

1. **Carga de datos sintéticos**  
   - Datos generados a partir de simulaciones hidráulicas.
   - Variables como caudales (Q) para cada estación de bombeo en cada periodo (T), y parámetros de bombas a instalar (A, H₀, Qmax, Rmax).
   - Objetivo: presiones (H)
   - Etiquetas: factibilidad y costo total.

2. **Procesamiento de datos**  
   - Eliminación de columnas irrelevantes.
   - Separación de datos para modelos de clasificación y regresión.
   - Balanceo de clases mediante SMOTE.
   - Estandarización de variables.

3. **Análisis Exploratorio**  
   - Visualizaciones de correlación y comportamiento entre variables.
   - Gráficos de dispersión y mapas de calor.

4. **Entrenamiento de Modelos**  
   - Modelo de clasificación: `DecisionTreeClassifier`.
   - Modelo de regresión: `MLPRegressor` con múltiples salidas (MultiOutput).

5. **Evaluación de Resultados**  
   - Validación cruzada con métricas como precisión, recall, F1, MAE y R².
   - Comparación de resultados entre entrenamiento y validación.

---

## Requisitos

- Python ≥ 3.8
- scikit-learn
- pandas
- matplotlib
- seaborn
- imbalanced-learn
