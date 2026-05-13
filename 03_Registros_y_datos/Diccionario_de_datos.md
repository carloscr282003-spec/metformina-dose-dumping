# Diccionario de datos

## Objetivo
Definir de manera inequívoca las variables/campos de los registros y datasets (CSV) para evitar ambigüedad y facilitar análisis reproducible.

## Convenciones
- Fechas: `YYYY-MM-DD`
- Hora: `HH:MM`
- Separador decimal: punto (`.`) en CSV (recomendado)
- Unidades: especificar siempre (mg/L, µg/mL, %, min, rpm, °C)

## Campos sugeridos (disolución)

| Campo | Tipo | Unidad/Formato | Descripción | Reglas/Validación |
|---|---|---|---|---|
| run_id | texto | `RUN-YYYY-NNN` | Identificador de corrida | Único |
| sample_id | texto | libre | ID de unidad/tableta | No vacío |
| product | texto | libre | Producto/formulación | Consistente |
| lot | texto | libre | Lote | Consistente |
| condition | texto | CONTROL / REFRESCO / etc. | Condición experimental | Catálogo |
| medium | texto | libre | Medio (composición) | Documentado |
| apparatus | texto | USP 1/2/... | Aparato | Catálogo |
| rpm | num | rpm | Velocidad | Rango esperado |
| temperature_c | num | °C | Temperatura | Rango y tolerancia |
| volume_ml | num | mL | Volumen | Consistente |
| time_min | num | min | Tiempo de muestreo | Lista definida |
| raw_signal | num | AU/area | Absorbancia o área HPLC | >=0 |
| concentration | num | mg/L o µg/mL | Concentración calculada | Según curva |
| percent_dissolved | num | % | % disuelto | 0–200 (según criterio) |
| analyst | texto | iniciales | Quién ejecutó | No vacío |
| reviewer | texto | iniciales | Quién revisó | Opcional/según QA |
| comments | texto | libre | Observaciones | Opcional |

## Catálogos
- `condition`: definir lista final.
- `product`: nomenclatura estable.
- `medium`: receta + código.
