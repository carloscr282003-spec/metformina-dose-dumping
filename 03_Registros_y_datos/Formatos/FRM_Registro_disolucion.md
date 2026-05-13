# FRM — Registro de disolución

## Encabezado
| Campo | Valor |
|---|---|
| Código de formato | FRM-DIS-001 |
| Versión | 0.1 |
| Fecha | AAAA-MM-DD |
| Analista | |
| Revisor QA | |

## Variables críticas y reglas
| Columna | Unidad | Rango esperado | Obligatorio | Regla de integridad |
|---|---|---|---|---|
| ID corrida | NA | Texto único | Sí | No duplicados |
| Condición (control/refresco) | NA | Catálogo | Sí | Debe existir en catálogo |
| Aparato disolución | NA | USP 1/2 (por confirmar) | Sí | Consistente por corrida |
| RPM | rpm | Según método | Sí | Numérico > 0 |
| Medio | NA | Según método | Sí | Catálogo |
| Volumen | mL | Según método | Sí | Numérico > 0 |
| Temperatura | °C | Según método | Sí | Registrar fuera de rango |
| Tiempo muestreo | min | Según plan | Sí | Catálogo de tiempos |
| Unidad # | NA | 1..n | Sí | Sin saltos no justificados |
| Señal analítica | AU o área | Según técnica | Sí | Numérico |
| Concentración calculada | mg/L | Según curva | Sí | Trazable a fórmula |
| % liberado | % | 0–100 (objetivo); >100 requiere investigación | Sí | Revisar outliers y sesgo analítico |
| Observaciones | NA | Texto | No | Justificar incidencias |

## Tabla de captura (copiar/pegar)
| ID corrida | Condición | Aparato | RPM | Medio | Volumen (mL) | Temp (°C) | Tiempo (min) | Unidad # | Señal | Concentración (mg/L) | % liberado | Observaciones |
|---|---|---|---:|---|---:|---:|---:|---:|---:|---:|---:|---|
|  |  |  |  |  |  |  |  |  |  |  |  |  |

## Revisión
| Revisión | Nombre | Fecha | Firma/Iniciales | Resultado |
|---|---|---|---|---|
| Analista | | | | Conforme / No conforme |
| Revisor QA | | | | Conforme / No conforme |
