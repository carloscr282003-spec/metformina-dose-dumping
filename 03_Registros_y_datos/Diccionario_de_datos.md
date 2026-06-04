# Diccionario de datos

## Objetivo
Definir de manera inequívoca las variables/campos de los registros y datasets (CSV) para evitar ambigüedad y facilitar análisis reproducible.

## Convenciones
- Fechas: `YYYY-MM-DD`
- Hora: `HH:MM`
- Separador decimal: punto (`.`) en CSV (recomendado)
- Unidades: especificar siempre (mg/L, µg/mL, %, min, rpm, °C)
- `% de refresco v/v`: campo **obligatorio y editable** para corridas en refresco.
- λ (nm): mantener explícito como **POR DEFINIR** hasta cierre del criterio de método.

## Campos sugeridos (formato largo: una fila por lectura UV-VIS)

| Campo | Tipo | Unidad/Formato | Descripción | Reglas/Validación |
|---|---|---|---|---|
| run_id | texto | `RUN-YYYY-NNN` | Identificador de corrida | Único |
| lectura_id | texto | `READ-YYYY-NNN` | Identificador de lectura UV-VIS | Único por fila |
| fecha | fecha | `YYYY-MM-DD` | Fecha de lectura | No vacío |
| analyst | texto | libre | Analista | No vacío |
| equipo_uvvis_id | texto | libre | Equipo UV-VIS | No vacío |
| sample_id | texto | libre | ID de unidad/tableta | No vacío |
| product | texto | libre | Producto/formulación | Consistente |
| lot | texto | libre | Lote | Consistente |
| condition | texto | CONTROL / REFRESCO / etc. | Condición experimental | Catálogo |
| refresco_tipo | texto | Coca-Cola / otro | Tipo de refresco usado | Obligatorio si `condition=REFRESCO` |
| refresco_%_v/v | num | % v/v | Porcentaje de refresco en mezcla | Obligatorio si `condition=REFRESCO` |
| refresco_lote | texto | libre | Lote del refresco | Recomendado |
| refresco_fecha_apertura | fecha | `YYYY-MM-DD` | Fecha de apertura | Recomendado |
| refresco_desgasificado | texto | SI/NO | Estado de desgasificación | Obligatorio si `condition=REFRESCO` |
| refresco_obs | texto | libre | CO₂, espuma, olor, etc. | Opcional |
| medium | texto | libre | Medio (composición) | Documentado |
| apparatus | texto | USP 1/2/... | Aparato | Catálogo |
| rpm | num | rpm | Velocidad | Rango esperado |
| temperature_c | num | °C | Temperatura | Rango y tolerancia |
| volume_ml | num | mL | Volumen | Consistente |
| time_min | num | min | Tiempo de muestreo | Lista definida |
| lambda_nm | texto | nm / `POR DEFINIR` | Longitud de onda de lectura | Obligatorio |
| absorbancia | num | AU | Señal UV-VIS | >=0 |
| dilution_factor | num | adimensional | Factor de dilución | >0 |
| ecuacion_calibracion | texto | `Abs = m*C + b` | Ecuación aplicada | No vacío |
| concentration_calculada | num | mg/L o µg/mL | Concentración calculada | Según curva |
| percent_dissolved | num | % | % disuelto | 0–200 (según criterio) |
| reviewer | texto | iniciales | Quién revisó | Opcional/según QA |
| comments | texto | libre | Observaciones | Opcional |

## Catálogos
- `condition`: definir lista final.
- `product`: nomenclatura estable.
- `medium`: receta + código.
- `refresco_tipo`: iniciar con `Coca-Cola`.
- `lambda_nm`: usar `POR DEFINIR` hasta cierre formal del método.
