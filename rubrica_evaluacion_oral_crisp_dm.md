# Evaluacion oral y activa por grupos

## Fases de CRISP-DM

**Fases evaluadas:**

1. Entendimiento del negocio.
2. Entendimiento de los datos mediante el Analisis Exploratorio de Datos (EDA).

Esta actividad evalua la capacidad del grupo para explicar su proyecto, justificar sus decisiones y demostrar con codigo como obtuvo sus resultados.

---

## 1. Condiciones de la presentacion

- La actividad se realiza **por grupos**.
- Cada grupo debe contar con **minimo dos expositores**.
- Cada grupo dispone de **un maximo de 3 minutos**.
- La presentacion debe tener **como maximo 2 diapositivas**.
- Todos los integrantes deben participar en el desarrollo del proyecto. La exposicion oral debe ser realizada, como minimo, por dos integrantes.
- La presentacion debe ser clara, concreta y centrada en los resultados mas importantes.
- No se debe leer de manera extensa el contenido de las diapositivas.

---

## 2. Contenido obligatorio de la presentacion

### Diapositiva 1: Entendimiento del negocio

El grupo debe presentar:

1. **Objetivo de negocio del proyecto**
   - Explicar que problema de negocio, social o de investigacion se desea resolver.
   - Indicar que decision o accion se espera apoyar con el analisis.

2. **Metrica principal**
   - Escribir el nombre de la metrica.
   - Explicar que mide y por que es importante para el proyecto.
   - Indicar la unidad de medida.

3. **Definicion y calculo de la metrica**
   - Presentar la formula, procedimiento o codigo utilizado.
   - Explicar que variables intervienen en su calculo.
   - Mostrar el valor obtenido para el conjunto de datos.

4. **Mejora tentativa de la metrica (opcional)**
   - Proponer un valor objetivo o una mejora esperada.
   - Justificar brevemente por que ese valor seria razonable.

> La propuesta de mejora es opcional y no debe inventarse como un resultado observado. Debe presentarse como una meta o escenario futuro.

### Diapositiva 2: Entendimiento de los datos y EDA

El grupo debe responder, usando su propio conjunto de datos, las siguientes cinco preguntas:

1. **¿Que datos tengo?**
   - Indicar el nombre o fuente del conjunto de datos.
   - Mostrar el numero de registros, variables y tipos de datos principales.

2. **¿Hay datos faltantes?**
   - Indicar si existen valores faltantes.
   - Identificar las variables afectadas y su cantidad.
   - Explicar que tratamiento se aplico o por que no fue necesario.

3. **¿Existen valores atipicos?**
   - Indicar si se encontraron valores atipicos.
   - Mostrar el metodo o grafico utilizado para identificarlos.
   - Explicar si son errores, casos validos o situaciones que requieren revision.

4. **¿Como se distribuyen los datos?**
   - Mostrar al menos una distribucion relevante mediante un histograma, grafico de densidad, barras u otra visualizacion adecuada.
   - Describir brevemente la forma, concentracion o comportamiento observado.

5. **¿Que relaciones existen entre variables?**
   - Presentar una relacion relevante mediante un grafico de dispersion, tabla de correlacion, mapa de calor u otra tecnica apropiada.
   - Explicar que relacion se observa y cuales son sus limitaciones.

6. **Hallazgo interesante**
   - Presentar un descubrimiento relevante, inesperado o util para el objetivo del proyecto.
   - Explicar por que el hallazgo puede ser importante para el negocio o el analisis.

---

## 3. Entregable en la plataforma

Cada grupo debe entregar un archivo **Jupyter Notebook (`.ipynb`)** que demuestre mediante codigo como se obtuvieron los resultados de la presentacion.

El notebook debe incluir, como minimo:

- Carga del conjunto de datos.
- Descripcion de la fuente y de la unidad de analisis.
- Exploracion inicial con cantidad de registros, variables y tipos de datos.
- Calculo de la metrica principal.
- Codigo para revisar datos faltantes.
- Codigo o procedimiento para revisar duplicados, inconsistencias y valores atipicos.
- Graficos o calculos que permitan analizar las distribuciones.
- Analisis de relaciones entre variables.
- Evidencia del hallazgo interesante.
- Interpretacion escrita de los resultados.
- Codigo ejecutado y salidas visibles.

### Recomendacion de organizacion del notebook

1. Titulo, integrantes y objetivo de negocio.
2. Importacion de librerias.
3. Carga y descripcion de los datos.
4. Limpieza o preparacion, si corresponde.
5. Definicion y calculo de la metrica principal.
6. Respuestas a las cinco preguntas del EDA.
7. Hallazgo interesante.
8. Conclusiones.

> El notebook no debe contener solamente codigo. Cada resultado debe estar acompanado por una explicacion breve y relacionada con el objetivo del proyecto.

---

## 4. Rúbrica de evaluacion

La evaluacion se realiza sobre una escala de 0 a 100 puntos. La columna que mejor describa el desempeño del grupo determina el nivel alcanzado. Los pesos se distribuyen de la siguiente manera:

- **Entendimiento del negocio:** 25% dividido entre 3 criterios, aproximadamente 8.33% por criterio.
- **Entendimiento de los datos:** 25% dividido entre 6 criterios, aproximadamente 4.17% por criterio.
- **Notebook y reproducibilidad:** 25%.
- **Presentacion oral y cumplimiento del formato:** 25%.

Los valores decimales se muestran redondeados; cada bloque suma exactamente 25%.

| Criterio | Peso | Inicial (0-50 puntos) | Basico (51-74 puntos) | Autonomo (75-89 puntos) | Estrategico (90-94 puntos) | Excelencia (95-100 puntos) |
|---|---|---|---|---|---|---|
| **Objetivo de negocio** | 8.33% | No presenta el objetivo o lo confunde con una tarea tecnica. No se identifica el problema que se desea resolver. | Presenta un objetivo general, pero es poco claro, amplio o no se relaciona bien con los datos. | Explica un objetivo claro y relacionado con una necesidad concreta del proyecto. | Formula un objetivo medible, pertinente y conectado con una decision o accion. | Presenta un objetivo preciso, medible y relevante, con una justificacion solida de su valor para el negocio. |
| **Metrica principal** | 8.33% | No presenta una metrica o presenta un indicador que no corresponde al objetivo. | Menciona una metrica, pero no explica claramente que mide o por que la eligio. | Define una metrica coherente y explica su importancia para el proyecto. | Relaciona la metrica con el objetivo, la decision y la interpretacion de resultados. | Justifica rigurosamente la metrica, sus ventajas, sus limitaciones y su utilidad para evaluar mejora. |
| **Definicion y calculo de la metrica** | 8.33% | No muestra la formula, el procedimiento ni el resultado. | Muestra un calculo incompleto, poco claro o con errores menores de interpretacion. | Explica las variables, el procedimiento y el valor obtenido de forma comprensible. | Presenta el calculo correctamente, con unidad de medida y evidencia reproducible en el notebook. | Demuestra dominio del calculo, valida el resultado, interpreta sus limites y propone una lectura critica. |
| **Datos disponibles y calidad inicial** | 4.17% | No describe el conjunto de datos ni su fuente. | Menciona los datos, pero omite registros, variables, tipos o unidad de analisis. | Describe la fuente, la unidad de analisis, el numero de registros y las variables principales. | Relaciona la estructura y calidad de los datos con el objetivo de negocio. | Ofrece una caracterizacion completa, critica y bien sustentada de la pertinencia y calidad de los datos. |
| **Datos faltantes y tratamiento** | 4.17% | No revisa los datos faltantes o presenta conclusiones sin evidencia. | Detecta algunos faltantes, pero no cuantifica ni explica el tratamiento aplicado. | Identifica las variables afectadas, cuantifica los faltantes y explica la decision tomada. | Justifica el tratamiento con base en el contexto y analiza su posible impacto. | Compara alternativas, demuestra el tratamiento mediante codigo y evalua sus consecuencias sobre la metrica. |
| **Valores atipicos, duplicados e inconsistencias** | 4.17% | No realiza ninguna comprobacion o interpreta los resultados de manera incorrecta. | Realiza una revision parcial sin explicar el metodo ni las decisiones tomadas. | Utiliza un metodo adecuado y explica si los casos deben conservarse, corregirse o revisarse. | Contrasta la evidencia estadistica con el contexto del proyecto antes de tomar decisiones. | Presenta un analisis riguroso, reproducible y critico, distinguiendo errores de observaciones validas. |
| **Distribuciones de los datos** | 4.17% | No presenta distribuciones o los graficos son ilegibles o irrelevantes. | Presenta un grafico, pero la descripcion es superficial o no responde al objetivo. | Muestra una distribucion relevante y describe sus caracteristicas principales. | Interpreta forma, concentracion, dispersion o asimetria y relaciona el resultado con el proyecto. | Selecciona visualizaciones apropiadas, compara patrones y extrae conclusiones profundas y prudentes. |
| **Relaciones entre variables** | 4.17% | No analiza relaciones o afirma relaciones sin evidencia. | Presenta una relacion, pero no explica el grafico o confunde correlacion con causalidad. | Utiliza un grafico o medida adecuada y describe la relacion observada. | Interpreta la fuerza, direccion y limitaciones de la relacion con datos de respaldo. | Analiza relaciones relevantes, evita conclusiones causales indebidas y propone implicaciones para el negocio. |
| **Hallazgo interesante** | 4.17% | No presenta un hallazgo o presenta una observacion desconectada de los datos. | Presenta un hallazgo poco claro, sin evidencia suficiente o sin interpretacion. | Presenta un hallazgo respaldado por un calculo o visualizacion y explica su importancia. | Relaciona el hallazgo con el objetivo de negocio y reconoce sus limitaciones. | Presenta un hallazgo original, relevante, bien demostrado y capaz de generar una pregunta o accion posterior. |
| **Notebook y reproducibilidad** | 25% | El archivo no se entrega, no ejecuta o no permite verificar los resultados. | Entrega un notebook incompleto, con codigo desordenado o salidas faltantes. | El notebook contiene codigo ejecutable, resultados visibles y explicaciones basicas. | El notebook esta organizado, documentado y permite reproducir la metrica y el EDA presentado. | El notebook es claro, completo y reproducible; el codigo, las visualizaciones y las conclusiones se conectan de forma rigurosa. |
| **Presentacion oral y cumplimiento del formato** | 25% | Excede el tiempo, no cumple el minimo de expositores o utiliza mas de dos diapositivas. La explicacion es confusa. | Cumple parcialmente el formato, pero presenta lectura excesiva, poca coordinacion o falta de claridad. | Cumple el tiempo, participa el minimo de dos expositores y comunica los resultados principales con claridad. | La exposicion es fluida, sintetica, bien distribuida entre expositores y respeta completamente el formato. | La presentacion es precisa, segura y convincente; administra el tiempo con excelencia y responde con solvencia las preguntas. |

---

## 5. Lista de verificacion antes de exponer

### Presentacion

- [ ] Hay al menos dos expositores.
- [ ] La exposicion dura como maximo 3 minutos.
- [ ] Se utilizan como maximo 2 diapositivas.
- [ ] Se presenta el objetivo de negocio.
- [ ] Se define y calcula la metrica principal.
- [ ] Se indica la unidad de medida de la metrica.
- [ ] La mejora tentativa, si se incluye, esta identificada como propuesta.
- [ ] Se responden las cinco preguntas del EDA.
- [ ] Se presenta un hallazgo interesante.

### Notebook

- [ ] El archivo tiene extension `.ipynb`.
- [ ] El codigo esta ejecutado y sus resultados son visibles.
- [ ] La metrica puede reproducirse desde el codigo.
- [ ] Los analisis de faltantes, atipicos, distribuciones y relaciones tienen evidencia.
- [ ] Las conclusiones estan escritas y se relacionan con los resultados.
- [ ] El notebook coincide con lo expuesto en las diapositivas.
