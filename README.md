# Sprint 3

El sistema ha crecido en volumen de datos y complejidad, por lo que ya no es 
viable trabajar únicamente con archivos CSV.

En este Sprint se profesionaliza la solución incorporando:

- Persistencia en base de datos relacional.
- Uso de ORM mediante SQLAlchemy.
- Control de versiones de datos.
- Preparación para búsquedas avanzadas.

Para ello es necesario migrar la información procesada a una base de datos 
estructurada.
# Urban Flow - Proyecto Integrador

## Sprint 3

### Objetivo
El objetivo principal de este sprint es migrar los datos de infracciones de 
tránsito a una base de datos relacional (SQLite) utilizando el ORM de 
SQLAlchemy, estructurar el versionado de datos binarios y del dataset procesado 
utilizando DVC, y configurar una base de datos vectorial (ChromaDB) con 
embeddings generados mediante OpenClip (ViT-B-32) para habilitar la búsqueda de 
vehículos mediante imágenes de patentes.

### Introducción y Contexto del Trabajo
El sistema de radares urbanos de la localidad de Vaalserberg ha crecido en 
complejidad y volumen. Para superar las limitaciones del almacenamiento en 
archivos planos (CSV), se ha diseñado y migrado la información a un esquema de 
base de datos relacional con relaciones consistentes de uno a muchos y uno a 
uno. Además, la evidencia visual (imágenes de patentes) se almacena y busca 
mediante vectores de similitud, sentando las bases para una identificación 
automatizada y precisa de vehículos sospechosos o infractores.

### Conclusión
La arquitectura híbrida implementada en este sprint, que combina una base de 
datos relacional (SQLite/SQLAlchemy) para consultas estructuradas y una base de 
datos vectorial (ChromaDB/OpenClip) para búsquedas basadas en similitud de 
imágenes, representa una solución óptima y profesional para sistemas modernos 
de tránsito inteligente. La separación de código y datos binarios a través de 
DVC garantiza la reproducibilidad y el correcto control de versiones en entornos 
colaborativos, asegurando la scalabilidad del sistema ante incrementos futuros 
en el volumen de datos.
