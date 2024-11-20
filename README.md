# Proyecto_ML

# Predicción Principales Causas de Muerte en Tierra del Fuego: Análisis de Datos y Modelos de Aprendizaje Automático

## Introducción
El objetivo principal de este proyecto es desarrollar un modelo de aprendizaje automático capaz de predecir la causa de muerte en la provincia de Tierra del Fuego. A través de este modelo, se busca identificar patrones y tendencias en la mortalidad que permitan comprender mejor los factores de riesgo asociados a cada causa de muerte.


## Contexto
Tierra del Fuego, al ser una provincia con características geográficas y socioeconómicas particulares, presenta un perfil de mortalidad que puede diferir de otras regiones de Argentina. Comprender las causas de muerte en esta región es fundamental por varias razones:
Salud Pública: Permite diseñar estrategias de prevención y promoción de la salud más focalizadas y efectivas.
Planificación de Servicios: Ayuda a optimizar la asignación de recursos en el sistema de salud.
Investigación: Contribuye al conocimiento científico sobre los factores que influyen en la mortalidad a nivel regional.
Política Pública: Informa la toma de decisiones en materia de salud y bienestar social.

##Preguntas de Investigación o Hipótesis
¿Cuáles son los principales factores de riesgo asociados a las principales causas de muerte en Tierra del Fuego? Esta pregunta busca identificar variables como edad, sexo, factores ambientales, etc, que están más fuertemente relacionadas con cada causa de muerte.
¿Es posible desarrollar un modelo de aprendizaje automático que prediga con precisión la causa de muerte en función de las variables disponibles? Esta pregunta evalúa la viabilidad de utilizar técnicas de aprendizaje automático para abordar este problema y la precisión que se puede alcanzar.
¿Qué algoritmos de aprendizaje automático son más adecuados para modelar la causa de muerte en este contexto particular? Esta pregunta busca identificar los modelos que mejor se ajustan a los datos y ofrecen mejores resultados predictivos.
Este proyecto busca utilizar el aprendizaje automático como herramienta para explorar las causas de mortalidad en Tierra del Fuego, identificar factores de riesgo y, en última instancia, contribuir a mejorar la salud de la población.


## Datos
Los datos utilizados son de IPIEC, con base en datos del Ministerio de Salud y Desarrollo Social. Secretaria de Gobierno de Salud. Dirección de Estadísticas e Información en Salud (DEIS).	


## Resultados
Al analizar las causas de muerte en Tierra del Fuego, observamos diferencias significativas entre hombres y mujeres, especialmente tras la pandemia de COVID-19.

Hombres: Se registró un pico en las muertes totales en 2020, seguido de una disminución gradual. Las enfermedades del sistema circulatorio, tumores malignos y enfermedades respiratorias mostraron un aumento constante.
Mujeres: Las muertes totales aumentaron año a año, con un mayor impacto en la población de 65 años o más. Las causas de muerte más comunes fueron similares a las de los hombres, pero con un mayor énfasis en enfermedades del sistema urinario y diabetes.
Modelado de Series de Tiempo

Se emplearon modelos SARIMA y árboles de decisión para predecir las causas de muerte.

SARIMA: Este modelo demostró un buen ajuste a los datos, con bajos valores de MSE y altos valores de R².
Árboles de decisión: Los árboles de decisión superaron al modelo SARIMA, especialmente cuando se redujo el número de variables de entrada, lo que sugiere que este modelo es más adecuado para capturar las relaciones no lineales presentes en los datos.

Conclusiones

Las causas de muerte en Tierra del Fuego presentan patrones diferenciados entre hombres y mujeres, especialmente tras la pandemia.
Los modelos de árboles de decisión demostraron ser más adecuados para predecir las causas de muerte en este conjunto de datos, en comparación con los modelos SARIMA.
La reducción del número de variables de entrada en los modelos de árboles de decisión mejoró significativamente su desempeño.


## Estructura del Proyecto
├── LICENSE            <- Licencia de código abierto si se elige una
├── Makefile           <- Makefile con comandos de conveniencia como `make data` o `make train`
├── README.md          <- README 
├── data
│   ├── external       <- Datos de fuentes de terceros.
│   ├── interim        <- Datos intermedios que han sido transformados.
│   ├── processed      <- Los conjuntos de datos finales y canónicos para modelado.
│   │   ├── dataset limpio.csv       <- Archivo csv limpio para el posterior modelo de machine learning.
│   └── raw           
│       
├── docs               <- Documentacion del proyecto
│
├── models             <- Modelos entrenados y serializados, predicciones de modelos o resúmenes de modelos
│
├── notebooks          <- Notebooks de Jupyter.
├── references         <- Diccionarios de datos, manuales y otros materiales explicativos.
│
├── reports            <- Análisis generado como HTML, PDF, LaTeX, etc.
│   └── figures        <- Gráficos y figuras generados para ser utilizados en informes

