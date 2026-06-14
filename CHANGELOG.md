
## Sprint 3 - Ejercicio 01
- Clonado del repositorio del TP2
- Cambio a rama Sprint_3 (creada desde Sprint_2)
- Descarga de datasets Sprint 1 y Sprint 2
- Verificación de acceso a todos los datasets

## Sprint 3 - Ejercicio 02
- Inicialización de DVC con remote local /content/remote_dvc
- Migración de imágenes raw a DVC
- Migración de CSV procesado a DVC
- Push de datos al remote DVC

## Sprint 3 - Ejercicio 03
- Diseño del modelo lógico de entidades (Vehiculo, Multa, Radar, Evidencia)
- Definición de relaciones entre entidades
- Uso de dataclasses para la estructura del modelo

## Sprint 3 - Ejercicio 04
- Implementación de función procesar_fila_csv()
- Mapeo de fila CSV a clases Vehiculo, Radar, Evidencia y Multa
- Conversión de tipos: fecha (date), hora (time), velocidad (int)
- Manejo de evidencia opcional (solo si hay imagen)
- Vinculación de relaciones inversas

## Sprint 3 - Ejercicio 05
- Diseño del modelo relacional con SQLAlchemy ORM
- Creación de modelos VehiculoORM, RadarORM, EvidenciaORM y MultaORM
- Configuración de relaciones, claves primarias y foráneas
- Implementación de métodos __repr__ y soporte para type hints en SQLAlchemy 2.0

## Sprint 3 - Ejercicio 06
- Creación de base de datos SQLite (transito.db) con SQLAlchemy
- Creación automática de tablas desde los modelos ORM
- Migración de datos desde CSV a la base de datos
- Implementación de cachés para evitar duplicados (vehículos y radares)
- Manejo de relaciones: vehículo-multa, radar-multa, multa-evidencia
- Validación de registros insertados (conteo y consistencia)

## Sprint 3 - Ejercicio 07
Se realizaron las siguientes consultas a la base de datos:
- Top 10 patentes con mayor cantidad de multas.
- Top 10 de multas que no poseen evidencia asociada.
- Radares con mayor volumen de infracciones.
- Top 10 patentes más reincidentes entre 2020-01-01 y 2020-12-31
- Estadísticas de Evidencia.

## Sprint 3 - Ejercicio 08
- Creación de la base de datos vectorial 'patente_vectorial' con ChromaDB.
- Configuración del modelo base OpenClip para generación de embeddings.
- Extracción de IDs de vehículos y rutas de imágenes de la base de datos 
  relacional 'transito.db'.
- Generación de embeddings para imágenes asociadas a multas con evidencia.
- Almacenamiento de embeddings, metadatos (ID de vehículo y ruta original de 
  imagen) y IDs de imagen en la colección 'patente_vectorial'.

## Sprint 3 - Ejercicio 9
- Creación de la función buscar_patente_imagen que recibe como parámetro una 
  imagen y retorna todos los datos del vehículo.
