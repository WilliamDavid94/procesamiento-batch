# Procesamiento en Lote (Batch) - Análisis Saber Pro 11

Este repositorio contiene la implementación de la **Capa Batch** dentro de una arquitectura Lambda, desarrollada para la asignatura de Big Data en la UNAD. El objetivo es realizar un análisis histórico de los resultados de las pruebas Saber 11 utilizando **Apache Spark**.

## 📝 Descripción de la Solución
La solución automatiza la ingesta y el análisis de datos educativos provenientes del portal de Datos Abiertos de Colombia. Se enfoca en la eficiencia del procesamiento distribuido para transformar registros masivos en métricas de rendimiento departamental.

### Componentes Clave:
* **Fuente de Datos**: Consumo directo mediante la API de Socrata (SODA) de datos.gov.co.
* **Tecnología**: Desarrollo en Python utilizando la librería **PySpark**.
* **Limpieza y EDA**: 
    * Casting de tipos de datos de cadena a flotante para habilitar cálculos estadísticos.
    * Filtrado de registros para asegurar la integridad de los resultados.
    * Agrupamiento (Aggregation) para determinar el promedio global por ubicación geográfica.

## 🛠️ Instrucciones de Ejecución

### Requisitos Previos
1. Tener configurado un entorno de **Apache Spark** (probado en versión 3.5.x).
2. Contar con la librería `requests` para la gestión de la API.

### Pasos para correr el script:
1. Clona este repositorio:
   ```bash
  
