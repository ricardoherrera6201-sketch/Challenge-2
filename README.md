# Challenge Intermedio: Modelado Predictivo con Spark ML  
### Autor: Ricardo Antonio Herrera Lara  

## 1. Descripción del Proyecto
Este proyecto utiliza **Apache Spark ML** para entrenar un modelo de **clasificación binaria** que predice la calidad del vino usando el dataset *Wine Quality* del UCI Machine Learning Repository.

Se realiza en Google Colab y se evalúa usando métricas de Spark ML.

---

## 2. Objetivo
Aplicar técnicas de machine learning sobre una base de datos real utilizando el procesamiento distribuido de PySpark.

---

## 3. Dataset
- Fuente: **UCI Machine Learning Repository**  
- Observaciones: ~1599  
- Variables: 11 características químicas  
- Objetivo: *quality*  
- Conversión a clasificación binaria:
  - 1 = calidad ≥ 7  
  - 0 = calidad < 7  

---

## 4. Preparación de Datos
- Revisión de nulos  
- Conversión del objetivo a binario  
- Ensamble con `VectorAssembler`  
- División 70% entrenamiento / 30% prueba  

---

## 5. Modelo Utilizado
**Regresión Logística**  
Justificación:
- Es un modelo clásico para clasificación binaria  
- Buena interpretabilidad  
- Implementación nativa en Spark ML  

---

## 6. Resultados (ejemplo — reemplaza con los tuyos)
- **Accuracy:** 0.74  
- **AUC:** 0.78  

Interpretación: El modelo clasifica de forma aceptable, aunque puede mejorar debido al desbalance de clases.

---

## 7. Conclusiones
- Spark facilita el procesamiento de datos grandes.  
- La regresión logística funciona bien como baseline.  
- El modelo podría mejorar con Random Forest o tuning de hiperparámetros.

