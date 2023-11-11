## Reporte de Resultados Clasificación Marea Roja
### Análisis Exploratorio de Datos
Dentro de la exploración de los datos se encontraron los siguientes patrones de interés:

*Las distribuciones de las variables en los días de análisis positivos y negativos siguen aproximadamente la misma distribución con las siguientes particularidades:*
* En las variables de temperatura la distribución de los positivos esta corrida hacia el lado derecho lo que confirma la suposición de una influencia de las altas temperaturas a la aparición de marea roja.
* En las variables de radiación solar se observa una interesante distribución donde en existe un pico amesetado de positivos en el rango de la mediana de la distribución y su consecuente baja de negativos lo que puede indicar que ese rango de radiación afecta particularmente al fenómeno.
* Las variables de viento no parecen afectar al fenómeno.
[![Figura1](Distribucion "Figura1")](http://reports/figures/Figura1.png "Figura1")

### Modelos de Clasificación
#### Regresión Logística
* La precisión del modelo con una validación cruzada fue: Media de precisión 0.88, desviación estándar 0.04.
* La precisión de entrenamiento fue de 0.865, la precisión de prueba fue de 0.895 mientras que la precisión del set completo de datos fue 0.874
* La matriz de confusión del set de prueba refleja una buena identificación de positivos con una tasa de falsos positivos un poco alta.

#### Regresión Logística
* La precisión del modelo con una validación cruzada fue: Media de precisión 0.87, desviación estándar 0.04.
* La precisión de entrenamiento fue de 96,3%, la precisión de prueba fue de 90,5% mientras que la precisión del set completo de datos fue de 94,5%
* La matriz de confusión del set de prueba refleja una identificación de positivos un poco menos eficiente, pero con una tasa de falsos positivos menor.

#### Conclusiones Finales
+ Es posible determinar con un grado de precisión aceptable la aparición de marea roja en base a variables meteorológicas.
+ El modelo de Regresión Logística es mejor para identificar los positivos, pero con una alta tasa de falsos positivos mientras que el de máquina de soporte vectorial tiene menor detección de positivos pero mayor precisión global.
+ Se recomienda explorar el rendimiento de otros algoritmos de aprendizaje automático.
+ Queda explorar el comportamiento del modelo agregando datos oceanográficos (temperatura del agua, salinidad, saturación de oxígeno, etc.)

