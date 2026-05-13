# Normatividad y alineación (USP / NOM / FEUM)

> Objetivo: mapear requisitos aplicables → evidencia dentro del repositorio.

## Alcance
Este documento no reemplaza las normas. Sirve para **trazabilidad**: qué requisito estamos atendiendo y dónde está la evidencia (registros/análisis/método).

## Principios de trabajo
- No inventar requisitos: si un punto requiere confirmación, marcar como **POR CONFIRMAR**.
- Mantener evidencia verificable: formatos, registros, control de cambios, análisis reproducible.

## Mapa de alineación (plantilla)

| Fuente (USP/NOM/FEUM) | Sección/Capítulo | Requisito/expectativa (resumen) | Cómo lo cumplo en el proyecto | Evidencia en el repo (ruta) | Estado (OK/POR CONFIRMAR) |
|---|---|---|---|---|---|
| USP | POR DEFINIR | Control documental y trazabilidad | Versionado del método + log de cambios + registros firmados | `02_Metodos_y_normatividad/Control_de_versiones_del_metodo.md`, `01_Planificacion/Reprogramacion_y_cambios.md`, `03_Registros_y_datos/Formatos/` | POR CONFIRMAR |
| FEUM | POR DEFINIR | Condiciones de disolución y criterios | Método documentado y condiciones controladas | `02_Metodos_y_normatividad/Metodos_disolucion.md` (a crear) | POR CONFIRMAR |
| NOM | POR DEFINIR | Buenas prácticas / integridad de datos (según aplique a tu contexto) | Formatos con revisión, control de datos, manejo de desviaciones | `03_Registros_y_datos/Formatos/`, `05_Calidad_desviaciones_CAPA/` | POR CONFIRMAR |

## Próximos pasos para completar
1) Especificar exactamente qué NOM(s) aplican (número y tema) y su relación con tu institución/lab.
2) Identificar capítulos USP relevantes (p. ej. disolución, validación, análisis) y FEUM aplicable.
3) Convertir “POR DEFINIR” en referencias concretas.

## Evidencia mínima esperada (checklist)
- [ ] Método documentado (condiciones completas) y versionado.
- [ ] Registros de preparación de medios / verificación de equipo.
- [ ] Registros de corrida (datos crudos + cálculos).
- [ ] Diccionario de datos.
- [ ] Log de cambios y reprogramación.
- [ ] Registro de desviaciones y CAPA (si aplica).
- [ ] Análisis reproducible (Excel/Minitab) + interpretación.
