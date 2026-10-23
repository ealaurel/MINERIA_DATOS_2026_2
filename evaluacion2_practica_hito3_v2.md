# Evaluación del hito 3 - Parte 2: evaluacion procesual en notebook (paralelo 1)

## Propósito y duración

Esta evaluación práctica individual revisa la construcción, evaluación e interpretación de modelos de clasificación y regresión del hito 3.

- **Duración total:** 40 minutos.
- **Preguntas:** 4 ejercicios prácticos, con aproximadamente 10 minutos para cada uno.
- **Entregable:** un solo notebook Jupyter (`.ipynb`) individual.
- **Datos:** utilizar los archivos disponibles en la carpeta `data/` del repositorio. Cada ejercicio indica el dataset.
- **Puntaje:** 100 puntos, 25 por pregunta.

## Reglas de trabajo y entrega

- El trabajo es **individual**. Al inicio del notebook, cada estudiante debe escribir su nombre completo y el paralelo. No formen grupos.
- Respondan cada pregunta dentro del notebook: copien el enunciado en una celda Markdown, desarrollen el código, muestren las salidas y escriban una respuesta e interpretación en otra celda Markdown.
- Comenten cada línea de código ejecutable, en la misma línea o inmediatamente antes, indicando qué hace y por qué se necesita. Las líneas vacías y las que solo contienen comentarios no requieren explicación adicional.
- Ejecuten las celdas y dejen visibles sus salidas. El notebook debe correr en orden desde el inicio; no se aceptan resultados sin código que los reproduzca.
- Se permite usar IA como apoyo para programar. Cada estudiante debe revisar y adaptar el código, indicar brevemente en una celda final qué herramienta utilizó y para qué, y poder explicar y justificar cada línea y decisión. El uso de IA no reemplaza la comprensión del trabajo.
- No inventen resultados. Interpreten los valores que efectivamente obtuvieron y señalen limitaciones cuando corresponda.

## Estructura sugerida del notebook

1. **Identificación:** nombre completo y paralelo.
2. **Pregunta 1:** enunciado, código comentado, salidas e interpretación.
3. **Pregunta 2:** enunciado, código comentado, salidas e interpretación.
4. **Pregunta 3:** enunciado, código comentado, salidas e interpretación.
5. **Pregunta 4:** enunciado, código comentado, salidas e interpretación.
6. **Uso de IA:** herramienta utilizada y tareas para las que se usó; si no se utilizó, indíquenlo.

## Preguntas prácticas

### 1. Clasificación con regresión logística en `ifood.csv` - 10 minutos

Utilicen `data/ifood.csv`. La variable objetivo es `Response`.

1. Seleccionen `Teenhome` y `Recency` como variables explicativas, y `Response` como variable objetivo. Muestren las dimensiones de las variables seleccionadas.
2. Dividan los datos en entrenamiento (80 %) y prueba (20 %), usando `random_state=777` y `stratify=y` para conservar la proporción de clases.
3. Ajusten una regresión logística con el conjunto de entrenamiento y predigan las clases del conjunto de prueba.
4. Muestren la exactitud y la matriz de confusión. En Markdown, expliquen qué representa la exactitud y qué tipo de error refleja cada una de las dos clases de la matriz.

### 2. Clasificación con árbol de decisión en `ifood.csv` - 10 minutos

Utilicen `data/ifood.csv` con `Response` como variable objetivo y `Kidhome` y `Recency` como variables explicativas.

1. Dividan los datos en entrenamiento (80 %) y prueba (20 %), usando `random_state=888` y `stratify=y`.
2. Ajusten un `DecisionTreeClassifier` con `max_depth=3` y `random_state=888`, utilizando únicamente el conjunto de entrenamiento.
3. Grafiquen el árbol con nombres de variables y clases legibles, y muestren la exactitud y la matriz de confusión para el conjunto de prueba.
4. Muestren la importancia de cada variable. En Markdown, describan una ruta de decisión del árbol y nombren la variable con mayor importancia. Aclaren por qué la importancia no demuestra causalidad.

### 3. Regresión con árbol de decisión en `insurance.csv` - 10 minutos

Utilicen `data/insurance.csv` para estimar `charges` a partir de `age`, `bmi` y `children`.

1. Dividan los datos en entrenamiento (80 %) y prueba (20 %), usando `random_state=888`.
2. Ajusten un `DecisionTreeRegressor` con `max_depth=3` y `random_state=888`, solo con los datos de entrenamiento.
3. Predigan `charges` para el conjunto de prueba y calculen RMSE y R².
4. Grafiquen el árbol con nombres de variables. En Markdown, interpreten una de sus reglas de división y expliquen qué indican RMSE y R² sobre las predicciones, sin afirmar causalidad.

### 4. Regresión lineal con OLS en `insurance.csv` - 10 minutos

Utilicen `data/insurance.csv` para estimar `charges` a partir de `age`, `bmi` y `children`.

1. Dividan los datos en entrenamiento (80 %) y prueba (20 %), usando `random_state=888`.
2. Añadan el intercepto y ajusten un modelo OLS con el conjunto de entrenamiento únicamente.
3. Predigan `charges` para el conjunto de prueba y calculen RMSE y R².
4. En Markdown, expliquen qué mide cada métrica e interpreten el signo de uno de los coeficientes estimados. Indiquen por qué el R² por sí solo no basta para decidir si el modelo es adecuado y no presenten una asociación como causalidad.

## Rúbrica de evaluación

Califiquen cada pregunta sobre 25 puntos. La calificación total es la suma sobre 100.

| Criterio | Puntaje | Evidencia esperada |
|---|---:|---|
| Pregunta 1: regresión logística | 25 | Variables y objetivo correctos; partición reproducible y estratificada; modelo ajustado con entrenamiento; predicción, métricas e interpretación correcta de la matriz de confusión. |
| Pregunta 2: árbol de clasificación | 25 | Partición correcta; árbol ajustado con los parámetros solicitados; visualización legible; exactitud, matriz de confusión e importancias correctas; interpretación prudente de una ruta y de las variables. |
| Pregunta 3: árbol de regresión | 25 | Partición correcta; árbol ajustado solo con entrenamiento y con la profundidad solicitada; visualización legible; RMSE, R² e interpretación razonable de una regla de división y de las métricas. |
| Pregunta 4: regresión lineal | 25 | Partición correcta; OLS ajustado solo con entrenamiento; predicciones y métricas correctas; interpretación razonable de un coeficiente y de las limitaciones. |

En las cuatro preguntas se considera la claridad de la respuesta, los comentarios línea por línea, la ejecución reproducible y la capacidad individual para justificar el código, incluso si recibió apoyo de IA.
