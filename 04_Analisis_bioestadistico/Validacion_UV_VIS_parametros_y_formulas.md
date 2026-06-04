# Documento madre — Validación UV-VIS: parámetros, captura y fórmulas

## Alcance
Guía maestra para planear, ejecutar y cerrar la validación de método UV-VIS en este proyecto.

## Fuentes
Referencias internas (sin citas textuales):
- `04_Analisis_bioestadistico/Validacion_metodos_control_calidad-006-017.pdf`
- `04_Analisis_bioestadistico/Validacion_metodos_control_calidad-018-040.pdf`
- `04_Analisis_bioestadistico/Validacion_metodos_control_calidad-042-063.pdf`
- `04_Analisis_bioestadistico/Validacion_metodos_control_calidad-064-172.pdf`
- `04_Analisis_bioestadistico/Validacion_metodos_control_calidad-174-199.pdf`

> Nota: esta guía estructura plantillas y cálculos compatibles con validación analítica. Ajustar criterios numéricos al protocolo aprobado.

## Parámetros de validación y captura en registros
| Parámetro | Qué se evalúa | Dónde se registra |
|---|---|---|
| Selectividad/especificidad | Interferencias de matriz/control/refresco | `01_Planificacion/Documentos_validacion_metodo/01_Ejecucion/FRM_Registro_lecturas_UV_VIS_validacion.md` |
| Linealidad y rango | Ajuste de curva en niveles definidos | `03_Registros_y_datos/Plantillas_csv/uvvis_lecturas_largo.csv` |
| Precisión | Variabilidad intra/inter | `03_Registros_y_datos/Plantillas_csv/validacion_uvvis_resumen_parametros.csv` |
| Exactitud (% recuperación) | Cercanía al valor esperado | `03_Registros_y_datos/Plantillas_csv/validacion_uvvis_resumen_parametros.csv` |
| LOD/LOQ | Sensibilidad del método | `03_Registros_y_datos/Plantillas_csv/validacion_uvvis_resumen_parametros.csv` |
| Robustez | Efecto de pequeños cambios | `01_Planificacion/Documentos_validacion_metodo/01_Ejecucion/BIT_Bitacora_validacion_UV_VIS.md` |
| Estabilidad | Comportamiento en tiempo/condición | `01_Planificacion/Documentos_validacion_metodo/01_Ejecucion/BIT_Bitacora_validacion_UV_VIS.md` |

## Fórmulas base y ejemplos plantilla

### 1) Curva de calibración
- Ecuación: `Abs = m*C + b`
- Despeje: `C = (Abs - b)/m`

Ejemplo:
- `Abs = 0.455`, `m = 0.012`, `b = 0.015`
- `C = (0.455 - 0.015)/0.012 = 36.67`

### 2) Corrección por dilución
- `C_original = C_calculada * DF`

Ejemplo:
- `C_calculada = 36.67`, `DF = 10`
- `C_original = 366.7`

### 3) Precisión (%RSD)
- `%RSD = (SD / promedio) * 100`

Ejemplo:
- promedio = 98.5, SD = 1.2
- `%RSD = 1.22%`

### 4) Exactitud (% recuperación)
- `%Recuperación = (C_encontrada / C_agregada) * 100`

Ejemplo:
- `C_encontrada = 49.2`, `C_agregada = 50.0`
- `%Recuperación = 98.4%`

### 5) LOD y LOQ (por pendiente)
- `LOD = 3.3 * (σ/m)`
- `LOQ = 10 * (σ/m)`

Ejemplo:
- `σ = 0.004`, `m = 0.012`
- `LOD = 1.10`
- `LOQ = 3.33`

### 6) f2 para comparación de perfiles
\[
 f_2 = 50 \cdot \log_{10}\left(\left[1 + \frac{1}{n}\sum_{t=1}^{n}(R_t - T_t)^2\right]^{-0.5} \cdot 100\right)
\]

### 7) %TMD (endpoint adicional)
\[
 \%TMD = \frac{\text{cantidad liberada o cuantificada}}{\text{dosis teórica marcada}} \times 100
\]

## Campos obligatorios de proyecto
- `refresco_tipo`: iniciar con `Coca-Cola`.
- `refresco_%_v/v`: obligatorio y editable por corrida.
- `lambda_nm`: registrar como `POR DEFINIR` hasta decisión formal documentada.
