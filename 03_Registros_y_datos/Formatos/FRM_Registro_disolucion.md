# FRM — Registro de disolución

**Código:** FRM-DIS-001  
**Versión:** v0.1  
**Fecha:** 2026-05-13  

> Formato para capturar datos de corridas de disolución con trazabilidad y control mínimo de integridad de datos.

## 1) Identificación de la corrida

| Campo | Valor |
|---|---|
| Run ID | RUN-YYYY-NNN |
| Fecha | YYYY-MM-DD |
| Lugar/Lab |  |
| Equipo (ID) |  |
| Aparato |  |
| Paletas/canastillas (ID) |  |
| Analista |  |
| Revisor |  |

## 2) Condición experimental

| Campo | Valor |
|---|---|
| Producto/Formulación |  |
| Lote |  |
| Condición | CONTROL / REFRESCO / OTRO |
| Medio (receta/código) |  |
| Volumen (mL) |  |
| Temperatura objetivo (°C) |  |
| Tolerancia (°C) |  |
| RPM objetivo |  |
| Tolerancia (rpm) |  |
| Tiempos de muestreo (min) |  |
| ¿Medio desgasificado? (S/N) |  |
| Observaciones (CO₂/espuma/pH) |  |

## 3) Cuantificación (UV/HPLC)

| Campo | Valor |
|---|---|
| Técnica | UV / HPLC |
| Equipo (ID) |  |
| Método (referencia) |  |
| Longitud de onda / Columna |  |
| Curva de calibración (ID) |  |
| Ecuación (si aplica) |  |

## 4) Datos crudos y cálculo (tabla principal)

> Completar una tabla por unidad/tableta. Duplicar el bloque según número de unidades.

### Unidad: ____  (Sample ID: ____)

| Tiempo (min) | Señal cruda (Abs/Área) | Conc. | % Disuelto | Notas |
|---:|---:|---:|---:|---|
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

## 5) Controles de integridad de datos (checklist)
- [ ] Todos los campos obligatorios completos.
- [ ] Run ID y Sample ID consistentes con etiquetas físicas.
- [ ] Unidades y fórmulas verificadas.
- [ ] No hay sobrescrituras sin justificación (si se corrigió algo, documentar en “Notas”).
- [ ] Revisión realizada.

## 6) Firmas

| Rol | Nombre/Iniciales | Firma | Fecha |
|---|---|---|---|
| Analista |  |  |  |
| Revisor |  |  |  |
