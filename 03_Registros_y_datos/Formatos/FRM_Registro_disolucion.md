# FRM — Registro de disolución

**Código:** FRM-DIS-001
**Versión:** v0.2
**Fecha:** 2026-06-04

> Formato para capturar datos de corridas de disolución con trazabilidad, cuantificación UV-VIS e integridad de datos.

## 1) Identificación de la corrida

| Campo | Valor |
|---|---|
| Run ID | RUN-YYYY-NNN |
| Fecha | YYYY-MM-DD |
| Lugar/Lab |  |
| Equipo disolución (ID) |  |
| Aparato |  |
| Paletas/canastillas (ID) |  |
| Analista |  |
| Revisor |  |

## 2) Condición experimental y matriz refresco

| Campo | Valor |
|---|---|
| Producto/Formulación |  |
| Lote |  |
| Condición | CONTROL / REFRESCO / OTRO |
| Refresco tipo | Coca-Cola / otro |
| Refresco % v/v | **Obligatorio y editable** |
| Refresco lote |  |
| Refresco fecha apertura | YYYY-MM-DD |
| ¿Refresco desgasificado? (S/N) |  |
| Medio (receta/código) |  |
| Volumen (mL) |  |
| Temperatura objetivo (°C) |  |
| Tolerancia (°C) |  |
| RPM objetivo |  |
| Tolerancia (rpm) |  |
| Tiempos de muestreo (min) |  |
| Observaciones (CO₂/espuma/pH y otros) |  |

## 3) Cuantificación UV-VIS

| Campo | Valor |
|---|---|
| Técnica | UV-VIS |
| Equipo UV-VIS (ID) |  |
| Método (referencia) |  |
| Longitud de onda λ (nm) | **POR DEFINIR** |
| Curva de calibración (ID) |  |
| Ecuación de calibración | `Abs = m*C + b` |
| Criterios de aceptación aplicados |  |

## 4) Datos crudos y cálculo (formato largo: una fila por lectura)

| Lectura ID | Sample ID | Tiempo (min) | λ (nm) | Absorbancia | Dilución (DF) | Ecuación usada | Concentración calculada | % Disuelto | Notas |
|---|---|---:|---|---:|---:|---|---:|---:|---|
|  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |

## 5) Controles de integridad de datos (checklist)
- [ ] Todos los campos obligatorios completos.
- [ ] Run ID, Lectura ID y Sample ID consistentes con etiquetas físicas.
- [ ] `% refresco v/v` registrado (si condición REFRESCO).
- [ ] λ registrada (`POR DEFINIR` permitido solo en etapa previa a definición formal).
- [ ] Unidades y fórmulas verificadas.
- [ ] No hay sobrescrituras sin justificación (si se corrigió algo, documentar en “Notas”).
- [ ] Revisión realizada.

## 6) Firmas

| Rol | Nombre/Iniciales | Firma | Fecha |
|---|---|---|---|
| Analista |  |  |  |
| Revisor |  |  |  |
