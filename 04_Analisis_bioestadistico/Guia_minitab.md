# Guía Minitab — Análisis de perfiles de disolución (borrador)

## Objetivo
Dar un flujo reproducible para describir, comparar y (si aplica) modelar perfiles de disolución.

## 1) Importación y formato de datos
- Mantén datos en formato largo: `condition`, `unit_id`, `time_min`, `%dissolved`.
- Importar CSV: **File > Open Worksheet**.

## 2) Descriptivos por tiempo y condición
- **Stat > Basic Statistics > Display Descriptive Statistics**
  - Variables: `%dissolved`
  - By variables: `condition`, `time_min`

## 3) Gráficos
- Perfil promedio:
  - **Graph > Line Plot**
  - “Mean” por `time_min` agrupado por `condition`.

## 4) Comparación de perfiles (ideas)
Dependiendo de tu diseño y supuestos, se puede:
- comparar en tiempos específicos,
- usar enfoque de medidas repetidas (si se modela por unidad),
- o calcular métricas-resumen (MDT/AUC) por unidad y comparar entre condiciones.

> Nota: Minitab no siempre tiene f2 directo como función; se puede calcular con columnas (Calc) o fuera en Excel.

## 5) Modelado
- Ajuste no lineal (si procede): **Stat > Regression > Nonlinear Regression**
  - Definir modelo (p. ej. Weibull) y estimar parámetros.

## Pendientes
- Confirmar modelo(s) objetivo.
- Confirmar si el análisis primario será f2 u otro.
