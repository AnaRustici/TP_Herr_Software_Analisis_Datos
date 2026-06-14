
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
