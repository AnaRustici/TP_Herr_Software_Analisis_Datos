Ejercicio 1: Creación del repositorio y armado de la estructura del proyecto.

Ejercicio 2: Se descargó el archivo, se mostraron las 5 primeras filas, se analizaron los tipos de datos y se contaron los valores nulos.

Ejercicio 3: Se normalizaron fechas, horas, ubicaciones y patentes, se eliminaron filas con valores vacíos y outliers, se calcularon los excesos de velocidad y se guardó el dataset en interim.

Ejercicio 4: Se definio la clase FineAnalyzer con metodos para ranking de patentes, ranking de horarios, exceso promedio de velocidad, exceso real promedio de velocidad y conteo de multas por ubicacion.

Ejercicio 5: Se generaron y exportaron graficos de barras, torta y lineas para el analisis exploratorio visual de las multas.

Ejercicio 6: Se calculo el porcentaje de infraccion que se produjeron en la fecha 1932-01-01 y el porcentaje en la hora 00:00.

Ejercicio 7: Se redacto la conclusion final sobre el estado del dataset y se anexo al archivo README.md.

Revision Final: Se revisaron todos los ejercicios y se realizaron pequeñas modificaciones siguiendo el enunciado del trabajo integrador.

Ejercicio 2: Se descargó el archivo, se mostraron las 5 primeras filas, se analizaron los tipos de datos y se contaron los valores nulos.

Ejercicio 3: Se normalizaron fechas, horas, ubicaciones y patentes, se eliminaron filas con valores vacíos y outliers, se calcularon los excesos de velocidad y se guardó el dataset en interim.

Ejercicio 4: Se definio la clase FineAnalyzer con metodos para ranking de patentes, ranking de horarios, exceso promedio de velocidad, exceso real promedio de velocidad y conteo de multas por ubicacion.

Ejercicio 5: Se generaron y exportaron graficos de barras, torta y lineas para el analisis exploratorio visual de las multas.

Ejercicio 6: Se calculo el porcentaje de infraccion que se produjeron en la fecha 1932-01-01 y el porcentaje en la hora 00:00.

Ejercicio 7: Se redacto la conclusion final sobre el estado del dataset y se anexo al archivo README.md.

Revision Final: Se revisaron todos los ejercicios y se realizaron pequeñas modificaciones siguiendo el enunciado del trabajo integrador.
## Sprint 2 - Ejercicio 01
- Clonado del repositorio del TP1
- Cambio a rama Sprint_2 (creada si no existe)
- Actualización de README para Sprint 2
- Descarga y descompresión de dataset de imágenes
- 106 imágenes almacenadas en urban_flow/data/raw/imgs/
- **Versionado de imágenes con Git (según indicación del profesor)**

## Sprint 2 - Ejercicio 02
- Listado de imágenes con nombre y tamaño en KB
- Clasificación en grupos plates (87) y completes (19)
- Construcción y guardado del diccionario group_images.json
- Función mostrar_imagenes en grilla 2x4

## Sprint 2 - Ejercicio 03
- Conversión a escala de grises de plates y completes.
- Suavizado (GaussianBlur) aplicado a ambos grupos.
- Detección de bordes (Canny) aplicado a ambos grupos.

## Sprint 2 - Ejercicio 04
- Extracción OCR optimizada para todo el set de imágenes.
- Implementación de algoritmo de coincidencia posicional (>= 80%).
- Cruce de datos visuales con el dataset de multas.
- Guardado del dataset final en la carpeta processed/.
