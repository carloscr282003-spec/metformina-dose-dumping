# Guía Excel — Análisis de perfiles de disolución (UV-VIS)

> Esta guía se completará conforme definamos: tiempos, n por condición, λ UV-VIS y métricas finales.

## 0) Estructura recomendada del archivo Excel
- Hoja `raw_data`: datos en formato “largo” (una fila por muestra-tiempo).
- Hoja `calc`: cálculos intermedios (% disuelto, promedios, SD, etc.).
- Hoja `f2`: cálculo de similitud (si aplica).
- Hoja `%TMD`: cálculo de porcentaje respecto a dosis teórica marcada.
- Hoja `plots`: gráficos.
- Hoja `report`: tabla final para reporte.

## 1) Preparar datos (formato largo)
Columnas mínimas:
- condition (CONTROL/REFRESCO)
- refresco_tipo (iniciar con Coca-Cola)
- refresco_%_v/v (**obligatorio, editable**)
- unit_id (1..n)
- time_min
- lambda_nm (`POR DEFINIR` hasta decisión formal)
- percent_dissolved

## 2) Resumen por condición y tiempo
Objetivo: obtener **promedio** y **SD** por condición en cada tiempo.

### Ejemplo de fórmulas (Excel en inglés; si tu Excel está en español, lo ajustamos)
- Promedio en tiempo t (filtrando por condición):
  - `=AVERAGEIFS(percent_range, condition_range, "CONTROL", time_range, t)`
- Desviación estándar (si tienes Excel 365 con FILTER):
  - `=STDEV.S(FILTER(percent_range, (condition_range="CONTROL")*(time_range=t)))`

> Alternativa: usar Tablas dinámicas (Pivot) para media y SD.

## 3) Cálculo de f2 (Similarity factor) — esquema
> f2 suele calcularse usando medias en cada tiempo (excluyendo t=0) y con 3–4+ puntos comunes. Se debe validar aplicabilidad y supuestos.

Definición:

- Sea `Rt` = % disuelto medio del **referente/control** en el tiempo t
- Sea `Tt` = % disuelto medio del **test/refresco** en el tiempo t
- n = número de tiempos usados

\[
 f_2 = 50 \cdot \log_{10}\left(100 \cdot \left[1 + \frac{1}{n}\sum_{t=1}^{n}(R_t - T_t)^2\right]^{-0.5}\right)
\]

### Implementación en Excel (plantilla)
Supón:
- En `B2:Bn` están `Rt`
- En `C2:Cn` están `Tt`

1) Diferencia: `D2 = B2-C2`
2) Cuadrado: `E2 = D2^2`
3) Promedio de cuadrados: `MSE = AVERAGE(E2:En)`
4) f2:
- `=50*LOG10((1+MSE)^(-0.5)*100)`

## 4) Interpretación (borrador)
- f2 cercano a 100: perfiles muy similares.
- f2 más bajo: mayor diferencia.

> Nota: la interpretación final debe alinearse a criterio aceptado por tu protocolo y a aplicabilidad (variabilidad, puntos, etc.).

## 4.1) Endpoint adicional: %TMD
Definición de trabajo (ajustable en protocolo):

\[
 \%TMD = \frac{\text{cantidad liberada o cuantificada}}{\text{dosis teórica marcada}} \times 100
\]

En Excel (ejemplo):
- `=cantidad_liberada_mg/dosis_teorica_mg*100`

## 5) Gráficos
- Curva % disuelto vs tiempo por condición.
- Barras de error (SD) por tiempo.

## Pendientes para cerrar esta guía
- Confirmar tiempos de muestreo.
- Confirmar criterio y aplicabilidad de f2 vs alternativas.
- Definir qué se reportará como primario.
