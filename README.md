# Optimización de Hiperparámetros - Random Forest

Este repositorio contiene el desarrollo de un taller práctico de **optimización de hiperparámetros** utilizando el algoritmo **Random Forest Classifier** con validación cruzada.

## Dataset

Se utilizó el conjunto de datos `datos_filtrados.csv`, que contiene registros de ciberseguridad, incluyendo:

- Número de usuarios afectados.
- Tiempo de resolución del incidente.
- Año.
- Pérdida financiera (en millones de dólares).

Se creó una variable categórica llamada `High_Loss`, que clasifica si la pérdida financiera fue alta o baja en función de la mediana del conjunto.

## ⚙Técnicas aplicadas

- **GridSearchCV** con validación cruzada (5 folds).
- **RandomizedSearchCV** con 25 iteraciones.
- Evaluación del modelo con matriz de confusión, precisión, recall y f1-score.

## Resultados

- Mejores hiperparámetros (`RandomizedSearchCV`):
  - `n_estimators`: 250
  - `max_depth`: None
  - `min_samples_split`: 10
  - `max_features`: log2
- Precisión del modelo final: **~51%**

## Archivos

- `taller_optimizacion_rf.ipynb`: Notebook con el desarrollo completo del taller.
- `modelo_random_forest_optimo.pkl`: Modelo entrenado y optimizado.
- `LICENSE`: Licencia MIT.

## 🔗 Licencia

Este proyecto se distribuye bajo la [Licencia MIT](LICENSE).
