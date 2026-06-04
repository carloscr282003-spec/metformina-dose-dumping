# Validación de método de control de calidad 064-172

> Documento de trabajo editable basado en la fuente PDF `Validacion_metodos_control_calidad-064-172.pdf`.
>
> Este archivo desarrolla la estructura de validación por parámetros y deja plantillas listas para completar con datos reales del estudio.

## 1. Objetivo

Desarrollar y documentar la validación del método de control de calidad 064-172 mediante una estructura técnica que permita:

- evaluar el desempeño del método,
- definir criterios de aceptación,
- registrar resultados de forma trazable,
- identificar desviaciones y acciones correctivas,
- conservar evidencia de cumplimiento.

## 2. Alcance

Aplica al método de control de calidad 064-172 descrito en la documentación fuente, para su evaluación, registro, revisión y aprobación interna.

> **Nota:** cuando el dato exacto no esté presente en la fuente PDF, este documento usa una plantilla conservadora editable.

## 3. Responsabilidades

- **Analista:** ejecutar pruebas, registrar datos y reportar observaciones.
- **Revisor técnico:** verificar cálculos, consistencia y cumplimiento.
- **Aprobador:** autorizar el cierre de la validación.
- **Aseguramiento de calidad:** revisar trazabilidad, integridad y formatos.

## 4. Información mínima que debes tener antes de empezar

- Código y nombre exacto del método.
- Versión del procedimiento o documento base.
- Matriz o producto a evaluar.
- Instrumento/equipo utilizado.
- Reactivos, estándares, patrones o materiales de referencia.
- Lote, pureza y vigencia de estándares.
- Número de réplicas y niveles de concentración.
- Criterios de aceptación definidos.
- Formato oficial de registro.
- Fecha, responsable y estado de calibración de equipos.

## 5. Parámetros de validación

### 5.1 Especificidad / selectividad

**Definición:** capacidad del método para medir el analito sin interferencias de matriz, impurezas, degradantes o excipientes.

**Propósito:** demostrar que la señal observada corresponde al analito objetivo.

**Cómo se evalúa:**
- blanco,
- estándar,
- muestra,
- muestra fortificada,
- placebo o matriz sin analito,
- si aplica, muestras degradadas.

**Datos requeridos:**
- señal del blanco,
- tiempo de retención o respuesta del analito,
- respuesta de posibles interferentes,
- cromatogramas, espectros o lecturas comparativas.

**Criterio de aceptación:**
- ausencia de interferencias significativas en la región del analito,
- respuesta del analito claramente diferenciable,
- cumplimiento del criterio definido por el método.

**Formato de registro asociado:**
| Fecha | Muestra | Blanco | Respuesta analito | Interferencia | Observación | Cumple |
|---|---|---:|---:|---:|---|---|

### 5.2 Linealidad

**Definición:** capacidad del método para obtener resultados directamente proporcionales a la concentración dentro de un rango determinado.

**Propósito:** confirmar que el método responde de manera proporcional.

**Cómo se evalúa:**
- preparar al menos 5 niveles de concentración,
- analizar cada nivel según el procedimiento,
- construir curva de calibración.

**Datos requeridos:**
- concentración nominal,
- respuesta instrumental,
- ecuación de regresión,
- coeficiente de correlación,
- pendiente e intercepto.

**Criterio de aceptación:**
- coeficiente de correlación dentro del valor definido,
- residuals aceptables,
- comportamiento lineal en el rango establecido.

**Formato de registro asociado:**
| Nivel | Conc. nominal | Respuesta | Conc. calculada | Residual | Observación |
|---|---:|---:|---:|---:|---|

### 5.3 Rango

**Definición:** intervalo entre la concentración mínima y máxima para el cual el método demuestra precisión, exactitud y linealidad aceptables.

**Propósito:** establecer los límites de uso del método.

**Cómo se evalúa:**
- revisar desempeño en niveles bajo, medio y alto,
- comprobar que cumple en todo el intervalo.

**Datos requeridos:**
- nivel mínimo,
- nivel medio,
- nivel máximo,
- resultados de exactitud y precisión por nivel.

**Criterio de aceptación:**
- cumplimiento en todo el intervalo propuesto.

**Formato de registro asociado:**
| Nivel | Concentración | Resultado | %Error | Cumple |
|---|---:|---:|---:|---|

### 5.4 Precisión

**Definición:** grado de concordancia entre resultados obtenidos bajo condiciones repetidas.

**Propósito:** demostrar reproducibilidad interna del método.

**Cómo se evalúa:**
- repetir análisis en una misma corrida,
- repetir en diferentes días, analistas o equipos si aplica.

**Datos requeridos:**
- resultados individuales,
- media,
- desviación estándar,
- %RSD.

**Criterio de aceptación:**
- %RSD menor o igual al límite definido.

**Formato de registro asociado:**
| Réplica | Resultado | Desviación | Observación |
|---|---:|---:|---|

### 5.5 Exactitud

**Definición:** grado de cercanía entre el resultado obtenido y el valor verdadero o de referencia.

**Propósito:** comprobar recuperación del analito.

**Cómo se evalúa:**
- muestras fortificadas a distintos niveles,
- comparación contra valor teórico.

**Datos requeridos:**
- valor agregado,
- valor recuperado,
- porcentaje de recuperación.

**Criterio de aceptación:**
- recuperación dentro del rango definido.

**Formato de registro asociado:**
| Nivel | Agregado | Recuperado | %Recuperación | Cumple |
|---|---:|---:|---:|---|

### 5.6 Límite de detección (LOD)

**Definición:** menor cantidad detectable del analito, aunque no necesariamente cuantificable con precisión.

**Propósito:** establecer capacidad de detección del método.

**Cómo se evalúa:**
- por relación señal/ruido,
- por desviación estándar de respuesta,
- o por criterio definido en el protocolo.

**Datos requeridos:**
- señal de blanco,
- señal mínima detectable,
- cálculo aplicado.

**Criterio de aceptación:**
- según el criterio validado en el protocolo.

**Formato de registro asociado:**
| Ensayo | Señal | Ruido | S/N | LOD calculado |
|---|---:|---:|---:|---:|

### 5.7 Límite de cuantificación (LOQ)

**Definición:** menor cantidad del analito que puede cuantificarse con precisión y exactitud aceptables.

**Propósito:** asegurar cuantificación confiable en bajas concentraciones.

**Cómo se evalúa:**
- usando relación señal/ruido,
- usando precisión y exactitud en baja concentración.

**Datos requeridos:**
- señal,
- ruido,
- recuperación,
- %RSD.

**Criterio de aceptación:**
- cumplimiento del valor mínimo definido.

**Formato de registro asociado:**
| Ensayo | Señal | Ruido | S/N | %RSD | %Recuperación | LOQ |
|---|---:|---:|---:|---:|---:|---:|

### 5.8 Robustez

**Definición:** capacidad del método para mantenerse fiable ante cambios pequeños y deliberados en parámetros operativos.

**Propósito:** identificar parámetros críticos del método.

**Cómo se evalúa:**
- variar flujo, pH, temperatura, tiempo, volumen, longitud de onda u otra variable relevante.

**Datos requeridos:**
- condición nominal,
- condición modificada,
- resultado comparativo,
- impacto observado.

**Criterio de aceptación:**
- sin cambios significativos en el desempeño.

**Formato de registro asociado:**
| Parámetro | Condición nominal | Condición alterada | Resultado | Diferencia | Cumple |
|---|---|---|---:|---:|---|

### 5.9 Estabilidad de muestras y soluciones

**Definición:** capacidad de conservar la integridad del analito durante el tiempo de análisis y almacenamiento.

**Propósito:** asegurar que los resultados no se alteren por degradación.

**Cómo se evalúa:**
- medir en tiempo inicial,
- medir a intervalos definidos,
- comparar contra referencia.

**Datos requeridos:**
- hora de preparación,
- hora de análisis,
- condición de almacenamiento,
- diferencia respecto al inicial.

**Criterio de aceptación:**
- variación dentro del límite definido.

**Formato de registro asociado:**
| Tiempo | Condición | Resultado | Diferencia % | Cumple |
|---|---|---|---:|---|

## 6. Señalizaciones críticas

- **⚠ No iniciar** sin verificar vigencia de estándares.
- **⚠ No validar** si los equipos no están calibrados o verificados.
- **⚠ Registrar** cualquier desviación desde el inicio.
- **⚠ No mezclar** datos de corridas distintas sin trazabilidad.
- **⚠ Conservar** cromatogramas, hojas de cálculo y cálculos.

## 7. Checklist de ejecución

### Antes de iniciar
- [ ] Método y versión confirmados
- [ ] Equipos calibrados/verificados
- [ ] Reactivos vigentes
- [ ] Estándares identificados
- [ ] Formatos preparados
- [ ] Criterios de aceptación definidos

### Durante el ensayo
- [ ] Condiciones de trabajo registradas
- [ ] Identificación de muestras correcta
- [ ] Réplicas suficientes
- [ ] Observaciones anotadas
- [ ] Desviaciones documentadas

### Después del ensayo
- [ ] Cálculos revisados
- [ ] Resultados comparados con criterios
- [ ] Gráficas/soportes archivados
- [ ] Conclusión redactada
- [ ] Aprobación obtenida

## 8. Formato general de registro

| Fecha | Método | Parámetro | Muestra | Resultado | Criterio | Cumple | Responsable | Observaciones |
|---|---|---|---|---:|---|---|---|---|

## 9. Tratamiento de resultados

- Reportar resultados individuales y promedios.
- Calcular desviación estándar y %RSD cuando aplique.
- Comparar cada parámetro contra su criterio de aceptación.
- Documentar cualquier exclusión o repetición justificada.

## 10. Desviaciones

Toda desviación debe incluir:
- descripción,
- fecha,
- impacto,
- acción inmediata,
- evaluación de impacto en la validación,
- cierre y aprobación.

## 11. Conclusión

La validación del método 064-172 solo debe considerarse concluida cuando todos los parámetros aplicables cumplan con sus criterios de aceptación y la documentación soporte esté completa.

## 12. Archivo de trabajo sugerido

- `README.md` — guía rápida de uso.
- `validacion_metodo_control_calidad_064_172.md` — documento principal.
- `formatos_registro.md` — tablas y plantillas.
- `checklist_validacion.md` — lista de verificación.
- `datos_requeridos.md` — datos mínimos a reunir.
