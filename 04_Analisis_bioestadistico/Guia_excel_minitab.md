# Guía bioestadística (Excel y Minitab)

## 1) Validación previa de datos
- Confirmar tipo de variable (continua/categórica).
- Revisar faltantes, duplicados, rangos y outliers.
- Verificar estructura por condición, tiempo y unidad.

## 2) Datos mínimos requeridos
- Equipo y condiciones de disolución.
- Tiempos de muestreo.
- Técnica analítica y conversión señal→concentración.
- n por condición y número de condiciones.
- Definición operacional de dose dumping.
- Comparación primaria (f2/modelo/% a t/MDT).

## 3) f2 en Excel (perfil promedio)
Si R_t = referencia en tiempo t y T_t = prueba en tiempo t:

\[
f_2 = 50 \cdot \log_{10}\left(\frac{100}{\sqrt{1 + \frac{1}{n}\sum_{t=1}^{n}(R_t-T_t)^2}}\right)
\]

### Estructura sugerida
- Columna A: Tiempo
- Columna B: R_t
- Columna C: T_t
- Columna D: (R_t-T_t)^2  
  `=POWER(B2-C2,2)`

### Fórmula Excel (ejemplo)
Suponiendo datos en filas 2:9 (n = número de tiempos):
- Forma equivalente con promedio de cuadrados:  
  `=50*LOG10(100/SQRT(1+AVERAGE(D2:D9)))`
- Forma explícita con suma y n:  
  `=50*LOG10(100/SQRT(1+(SUM(D2:D9)/COUNT(D2:D9))))`

### Interpretación base
- **f2 ≥ 50**: perfiles similares.
- **f2 < 50**: perfiles no similares.

> Confirmar criterios formales aplicables en USP/FEUM para el caso específico.

## 4) Flujo en Minitab (resumen)
1. Cargar datos en columnas: `Condicion`, `Tiempo`, `%Liberado`.
2. `Stat > Basic Statistics > Display Descriptive Statistics`.
3. `Graph > Boxplot` y/o `Graph > Individual Value Plot` para outliers.
4. Si aplica comparación por tiempo: `Stat > ANOVA > One-Way` (o no paramétrica si no se cumplen supuestos).
5. Documentar supuestos, resultado y conclusión trazable.

## 5) Redacción sugerida de resultado
“Bajo las condiciones evaluadas, el análisis [método] mostró [resultado]. Con base en [criterio], se concluye [interpretación], sujeto a verificación normativa [por confirmar/confirmado].”
