Sprint 1


                Objetivo:

                El objetivo principal de este proyecto es aplicar los conocimientos adquiridos en para el versionado de código, la organización, limpieza del código y la utilización de pandas.


                Introducción y Contexto del problema:

                La localidad llamada Vaalserberg de Bélgica se encuentra en la zona fronteriza y limita con los paises de Países Bajos y Alemania. Esta localidad cuenta con un sistema de radares urbanos para la detección de infracciones por exceso de velocidad. Los registros históricos provienen de sistemas heredados, el cuál presenta errores de formato, faltante de datos generando registros inconsistentes en el nuevo sistema.
                Debemos analizar y depurar los datos de viejo sistema para obtener información relevante sobre las infracciones y de está forma en el futuro poder incorporar los datos al nuevo sistema sin inconsistencias.
                
### Conclusión del Análisis de Datos (Sprint 1)

A partir de la depuración del dataset de radares del sistema heredado de Vaalserberg, se concluye lo siguiente:

1. **Inconsistencias Temporales:** Se detectó una severa degradación en los metadatos de tiempo. Un 26.01% de los registros carecían de una fecha válida (procesados como `1932-01-01`) y un 19.39% no poseían una hora rastreable (procesados como `00:00`).
2. **Pérdida de Integridad:** La eliminación masiva de más de 2400 filas por falta de variables clave (patente o velocidad) indica que el sistema físico fallaba constantemente al reconocer los vehículos.
3. **Depuración Efectiva:** El cálculo del exceso de velocidad aplicando un 5% de tolerancia permitió limpiar falsos positivos y conservar únicamente las infracciones válidas.
4. **Impacto Final:** El dataset `interim/speeding_fines.csv` se encuentra estandarizado y homogeneizado. Sin embargo, para la migración final al nuevo sistema, se recomienda aislar aquellas multas con fechas y horas imputadas por defecto, ya que carecen de validez legal.
