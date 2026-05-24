# Sprint 2

## Objetivo:
Desarrollar un sistema que determine qué multas tienen evidencia visual válida.

## Introducción y Contexto del sprint de trabajo:
Los radares urbanos generan registros administrativos de multas de forma
automática y las cámaras asociadas registran la evidencia visual que acompaña y
valida la infracción.
Sin embargo:
- No todas las multas tienen una imagen asociada.
- No todas las imágenes corresponden a una infracción.
- Puede haber errores de detección.

El objetivo actual es determinar qué multas tienen evidencia visual válida.

## Versionado de imágenes:
Las imágenes se versionan directamente con Git según indicación del profesor.

## Conclusión del Análisis de Datos (Sprint 2)

**Problema detectado:** Existe una falta de **integridad referencial directa** (una clave foránea o ID único) que vincule las imágenes físicas generadas por los radares de Vaalserberg con los registros tabulares del sistema.
Depender del Reconocimiento Óptico de Caracteres (OCR) para cruzar datos de texto con imágenes (Data Matching) es una mala práctica de diseño a largo plazo porque:
1. Es propenso a errores por ruido visual, iluminación o desgaste de las patentes.
2. Requiere un alto poder de cómputo (ineficiente).
3. Nunca garantiza el 100% de efectividad (generando imágenes "huérfanas" sin match).

**Solución ideal:** En un diseño de base de datos robusto, la cámara debería inyectar el ID unívoco de la infracción en los metadatos de la imagen (EXIF) desde el momento exacto de la captura, o guardar la ruta de la imagen en la misma transacción SQL que genera la multa.
