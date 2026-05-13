# Plan de trabajo (borrador)

> Este plan es un punto de partida. Se ajusta con base en disponibilidad de equipo, insumos, tiempos de corrida y hallazgos.

## Objetivo del plan
Tener un camino claro desde la definición del método hasta el análisis y reporte, manteniendo trazabilidad (cambios y desviaciones).

## Fases e hitos

### Fase 1 — Definición (Semana 1)
- [ ] Definir condiciones de disolución (aparato, rpm, medio(s), volumen, temperatura, tiempos de muestreo).
- [ ] Definir técnica analítica (UV/HPLC) y esquema de calibración.
- [ ] Definir endpoints primarios/ secundarios.
- [ ] Definir definición operacional de “dose dumping”.

**Entregables**
- Método v0.1 en `02_Metodos_y_normatividad/`.
- Diccionario de datos v0.1.

### Fase 2 — Piloto y robustez práctica (Semanas 2–3)
- [ ] Corrida(s) piloto en condición control.
- [ ] Corrida(s) piloto en refresco.
- [ ] Ajustes menores documentados (control de cambios).
- [ ] Verificación de integridad de datos (formatos completos, cálculos reproducibles).

**Entregables**
- Registros piloto completos.
- Decisión sobre ajustes del método (v0.2).

### Fase 3 — Ejecución (Semanas 4–6)
- [ ] Corridas formales (definir número de unidades por condición y número de corridas).
- [ ] Captura de datos estandarizada.
- [ ] Gestión de desviaciones (si ocurre) y evaluación de impacto.

**Entregables**
- Dataset(s) final(es) (CSV) + registros.
- Desviaciones/CAPA documentadas (si aplica).

### Fase 4 — Análisis y reporte (Semanas 7–8)
- [ ] Limpieza/validación de datos.
- [ ] Comparación de perfiles (f2 y alternativas cuando no aplique).
- [ ] Modelado (p. ej. Weibull) y comparación.
- [ ] Redacción de reporte final.

**Entregables**
- `04_Analisis_bioestadistico/Interpretacion_y_reporte.md` (a crear).
- Reporte final en `06_Reportes/` (a crear).

## Riesgos y mitigaciones (ejemplos)
- **Insumos/equipo** no disponibles → reprogramación documentada.
- **Alta variabilidad** → revisar supuestos de f2, considerar alternativas.
- **Cambios de método** → control de cambios + impacto y comparabilidad.
- **Medio refresco**: burbujeo/CO₂/espuma → documentar manejo (desgasificación, control de temperatura, etc.).
