### *Tecnicatura Superior en Ciencia de Datos e Inteligencia Artificial.*
### *Politécnico Malvinas Argentinas.*

## Aprendizaje Automático
Autor: Visñuk Victor.
# **Clasificación Marea Roja**
*Utilizacion de las técnicas de aprendizaje automatico aprendidas a lo largo de la cursada en el campo de la marea roja a fines de predecir la aparicion de toxinas mediante clasificación.*

##### Entrega 1: Descripción y Formulación del ObjetivoEntrega 1: Descripción y Formulación del Objetivo

------------

Se conoce como marea roja a la proliferación de una o distintos tipos de organismos en diferentes cuerpos de agua que contienen diferentes tipos de toxinas que mediante el proceso de bioacumulación pueden afectar a los seres humanos. Se la denomina marea roja o hemotalasia debido al cambio de color que se percibe localmente en el agua derivado del aumento localizado de estos organismos.
“Estos fenómenos se inician, desarrollan y desaparecen debido a la interacción de factores biológicos intra e interespecíficos, oceanográficos y meteorológicos, procesos aun no totalmente conocidos en general” (Marea Roja en el Canal Beagle, Julio H. Vinuesa 1993).
Existen distintas especies con toxinas de distinto nivel de peligrosidad con síntomas que van desde diarreas y vómitos hasta toxinas de tipo paralizante que pueden llevar a la muerte por insuficiencia respiratoria.
Actualmente y desde hace muchos años se realizan estudios periódicos de monitoreo en distintos organismos particularmente cholga y mejillón en los cuales mediante un procedimiento se inyecta a ratones, existen datos tabulados según el tiempo que tarde en morir y los niveles de toxina.
Al ser estos moluscos habitantes del intermareal además de ser consumidos luego de la recolección y venta por personas dedicadas a la pesca pueden ser recolectados de sus bancos costeros por cualquier persona que sepa identificar sus zonas y épocas.
Esto hace que la detección temprana de este tipo de sucesos se vuelva crucial para evitar estas consecuencias, y en caso de poder predecirse un brote pueden tomarse medidas que eviten aun mas las consecuencias como adelantar la “cosecha” de los moluscos previo al brote.
Partimos con la hipótesis de que es posible determinar la presencia de toxinas mediante distintos datos meteorológicos (temperatura, viento, precipitaciones, presión, etc.) y oceanográficos (salinidad, mareas, temperatura del agua, etc.).

------------


**Las preguntas de investigación del proyecto son:**

-	¿Es posible integrar los datos provenientes de los análisis de monitoreo de marea roja con datos meteorológicos y oceanográficos de sus respectivas fechas?
-	¿Existe relación entre estos datos, meteorológicos y oceanográficos, respecto a la aparición de marea roja la ciudad de Ushuaia?
-	¿Es posible entrenar un algoritmo de aprendizaje supervisado utilizando como datos de entrenamiento los datos oceanográficos y meteorológicos y como target la aparición o no de marea roja?
-	¿Es posible realizar predicciones con este modelo utilizando datos nuevos con la precisión adecuada?

Todas estas englobadas en la pregunta clave del proyecto ¿Se puede clasificar mediante las diferentes variables predictoras, meteorológicas y oceanográficas, si en un determinado momento hay o no marea roja?

------------
**Las distintas etapas del proyecto son:**
-	Obtención de los datos: datos de los análisis de la presencia de toxinas en distintos moluscos, datos meteorológicos y oceanográficos de los mismos periodos.
-	Integración y limpieza de los datos provenientes de las distintas fuentes.
-	Análisis exploratorio de los datos en busca de comprender mejor los datos y encontrar patrones y preparación de los datos para el modelado.
-	Modelar los datos en los distintos algoritmos de clasificación que podemos utilizar y analizar sus resultados, en esta etapa también se optimizan los distintos modelos y culmina con la elección del modelo más eficiente.
-	Visualizar y comunicar los resultados del modelo.

Estas etapas si bien siguen un orden se retroalimentan y pueden retomarse o reiniciarse en base a las salidas de las otras etapas.

------------

### Organizacion del Repositorio
    
    ├── LICENSE
    ├── Makefile           <- Makefile con comandos como `make data` o `make train`
    ├── README.md          <- El README del nivel superior para desarrolladores o usuarios de este proyecto.
    ├── data
    │   ├── external       <- Datos de fuentes externas.
    │   ├── interim        <- Datos intermedios que han sido transformados.
    │   ├── processed      <- Datasets finales para el modelado.
    │   └── raw            <- Datos crudos internos.
    │
    ├── docs               <- Un proyecto Sphinx por defecto, vea sphinx-doc.org para mas detalles.
    │
    ├── models             <- Modelos entrenados, predicciones o resumenes de modelos.
    │
    ├── notebooks          <- Jupyter notebooks. La convencion para            		nombrarlos es un
    │                                    numero (para ordenarlos) seguido de las iniciales del creador y una descripcion corta 
    │                                   demilitada por "-" por ejemplo `1.0-jqp-exploracion-inicial-datos`.
    │
    ├── references         <- Diccionario de datos, manuales y otro material explicativo.
    │
    ├── reports            <- Analisis generado como HTML, PDF, LaTeX, etc.
    │   └── figures        <- Graficos y figuras generadas para ser usadas en reportes.
    │
    ├── requirements.txt   <- El archivo de requerimientos para reproducir el ambiente de analisis por ejemplo
    │                         generado con `pip freeze > requirements.txt`
    │
    ├── setup.py           <- hace el proyecto instalable mediante pip  (pip install -e .) asi src puede ser importado. can be imported
    ├── src                <- Codigo fuente usado en este proyecto.
    │   ├── __init__.py    <- Hace a src un modulo de Python
    │   │
    │   ├── data           <- Scripts para descargar o generar los datos.
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts para transformar los datos crudos en features para el modelado.
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts para entrenar modelos y luego hacer predicciones.
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts para crear visualizaciones orientadas a la exploracion de datos o a los resultados.
    │       └── visualize.py
    │
    └── tox.ini            <- archvi tox con ajustes para ejecutar tox; vea tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
