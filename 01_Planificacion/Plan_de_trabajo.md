# Plan de trabajo (alineado a UV-VIS)

> Este plan es un punto de partida. Se ajusta con base en disponibilidad de equipo, insumos, tiempos de corrida y hallazgos.

## Objetivo del plan
Tener un camino claro desde la definición del método hasta el análisis y reporte, manteniendo trazabilidad (cambios y desviaciones).

## Flujo del proyecto
Planeación → Ejecución → Análisis → Conclusión
(con trazabilidad continua en control de cambios y desviaciones/CAPA)

## Fases e hitos

### Fase 1 — Planeación técnica (Semana 1)
- [ ] Definir condiciones de disolución (aparato, rpm, medio(s), volumen, temperatura, tiempos de muestreo).
- [ ] Confirmar técnica analítica principal: **UV-VIS**.
- [ ] Definir estrategia para seleccionar **λ (por definir)** y documentar decisión.
- [ ] Definir criterios de aceptación del método (linealidad, precisión, exactitud, LOD/LOQ, robustez, selectividad, estabilidad).
- [ ] Definir endpoints primarios/secundarios de análisis final (f2, %TMD y otros).
- [ ] Definir definición operacional de “dose dumping”.

**Entregables**
- Método v0.1 en `02_Metodos_y_normatividad/`.
- Diccionario de datos v0.2 (incluyendo campos de Coca-Cola y `% v/v` variable).
- Protocolo de validación UV-VIS en `01_Planificacion/Documentos_validacion_metodo/00_Planeacion/`.

### Fase 2 — Validación del método UV-VIS (Semanas 2–4)
- [ ] Ejecutar plan de validación (linealidad/rango, precisión, exactitud, selectividad, LOD/LOQ, robustez, estabilidad según aplique).
- [ ] Registrar datos crudos en formato largo (una fila por lectura UV-VIS).
- [ ] Documentar criterios cumplidos/no cumplidos y acciones.
- [ ] Emitir reporte de validación del método.

**Entregables**
- Registros de validación completos.
- Reporte de validación UV-VIS (apto/no apto y alcance).

### Fase 3 — Ejecución experimental de perfiles (Semanas 5–7)
- [ ] Corridas formales (definir número de unidades por condición y número de corridas).
- [ ] Captura de datos estandarizada en condición control y condición **Coca-Cola**.
- [ ] Registrar `% de Coca-Cola v/v` como campo obligatorio y editable por corrida.
- [ ] Gestión de desviaciones (si ocurre) y evaluación de impacto.

**Entregables**
- Dataset(s) final(es) (CSV) + registros.
- Desviaciones/CAPA documentadas (si aplica).

### Fase 4 — Análisis (Semanas 8–9)
- [ ] Limpieza/validación de datos.
- [ ] Comparación de perfiles (f2 y alternativas cuando no aplique).
- [ ] Cálculo y análisis de **%TMD** y otros endpoints definidos.
- [ ] Modelado (p. ej. Weibull) y comparación.

**Entregables**
- `04_Analisis_bioestadistico/Interpretacion_y_reporte.md` (a crear/actualizar).
- Reporte final en `06_Reportes/` (a crear).

### Fase 5 — Conclusión y cierre (Semana 10)
- [ ] Integrar conclusión técnica del método UV-VIS validado y su alcance.
- [ ] Integrar conclusión de perfiles y riesgo de dose dumping.
- [ ] Consolidar control de cambios y lecciones aprendidas.

## Riesgos y mitigaciones (ejemplos)
- **Insumos/equipo** no disponibles → reprogramación documentada.
- **Alta variabilidad** → revisar supuestos de f2, considerar alternativas.
- **Cambios de método** → control de cambios + impacto y comparabilidad.
- **Medio refresco**: burbujeo/CO₂/espuma → documentar manejo (desgasificación, control de temperatura, etc.).
- **λ aún no definida** → bloquear corridas formales hasta documentar decisión y criterios.
