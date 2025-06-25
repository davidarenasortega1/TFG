# Trabajo Fin de Grado:

Este repositorio contiene el código y análisis correspondientes al Trabajo Fin de Grado (TFG), centrado en el modelado y predicción de series temporales mediante técnicas estadísticas y de machine learning, con énfasis en la descomposición espectral (FFT), modelos ARIMA/SARIMA y métodos de ensamblado.

## 🎯 Objetivo

El objetivo principal de este trabajo es evaluar la capacidad predictiva de diferentes enfoques para series temporales, incluyendo:

- Modelos clásicos como AR, MA, ARIMA y SARIMA.
- Modelos basados en descomposición de Fourier.
- Modelos ETS (Exponential Smoothing).
- Técnicas de ensamblado para combinación de predicciones.

## 🧪 Metodología

El flujo de trabajo se divide en las siguientes etapas:

1. **Simulación de series**:
   - Generación de series sintéticas usando modelos AR(1) y MA(1).
   - Señales periódicas simuladas con suma de senoidales y ruido.

2. **Descomposición y análisis espectral**:
   - Aplicación de Transformada Rápida de Fourier (FFT) para descomposición en componentes frecuenciales.
   - Selección de las frecuencias dominantes con mayor energía.

3. **Modelado clásico**:
   - Ajuste de modelos ARIMA y SARIMA a series simuladas y reales.
   - Evaluación de residuos y supuestos (estacionariedad, autocorrelación, etc.).

4. **Modelado exponencial (ETS)**:
   - Aplicación de modelos ETS a distintas series.
   - Evaluación de ajuste y predicción.

5. **Evaluación de errores**:
   - Cálculo de métricas como MAPE (Mean Absolute Percentage Error) y MedAPE (Mediana del Error Porcentual Absoluto).
   - Filtrado de outliers para obtener métricas robustas.

6. **Métodos de ensamblado**:
   - Combinación de predicciones de distintos modelos mediante media y mediana.
   - Comparación entre modelos individuales y ensamblados.

## 📊 Resultados

Algunos hallazgos clave del trabajo:

- Los modelos basados en descomposición de Fourier ofrecen buena capacidad de predicción en señales periódicas con ruido.
- El ensamblado de modelos (media y mediana) mejora la estabilidad de las predicciones, reduciendo sensibilidad a errores extremos.
- El modelo ETS proporciona predicciones sólidas especialmente en datos suavizados o con componentes estacionales.
- Las métricas MAPE y MedAPE fueron utilizadas extensivamente para evaluar precisión y robustez de las predicciones.

## 🧰 Tecnologías y paquetes usados

- Lenguaje: **R**
- Paquetes: `forecast`, `TTR`, `stats`, `ggplot2`, `RColorBrewer`, `CVXR`
- Métodos implementados:
  - Modelos ARIMA, SARIMA
  - Modelos ETS
  - FFT y regresión sobre componentes frecuenciales
  - Regularización: Ridge, Lasso y L∞ con `CVXR`

## 📁 Estructura del código

El archivo `tfg.Rmd` contiene tanto la generación de datos como el análisis y visualización. Incluye:

- Simulación de datos sintéticos
- Análisis de Fourier
- Ajuste de múltiples modelos
- Comparación de predicciones
- Cálculo de errores

## 📎 Nota final

Este trabajo combina elementos clásicos de análisis de series temporales con enfoques modernos de ensamblado y optimización, ofreciendo un enfoque práctico a la predicción robusta en entornos con ruido.



