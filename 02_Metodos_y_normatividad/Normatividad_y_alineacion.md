# Alineación Normativa y Metodológica: Estudio de Dose Dumping de Metformina ER

Este documento establece la correspondencia formal entre los requisitos de la legislación sanitaria mexicana, las especificaciones compendiales internacionales y los parámetros de desempeño analítico aplicados al proyecto de investigación.

---

## 1. Marco Normativo Aplicable

### 1.1 Regulación Nacional (NOM-177-SSA1-2013)
Establece los criterios metodológicos obligatorios para la realización de perfiles de disolución y la validación de métodos analíticos aplicados a pruebas de intercambiabilidad en territorio nacional[cite: 1]. 
* **Aplicación en el proyecto:** Rige el diseño de la validación cruzada y los criterios de aceptación matemática para dictaminar la similitud cinética entre las curvas de disolución[cite: 1].

### 1.2 Regulación Internacional y Compendial (USP / <711>)
La Farmacopea de los Estados Unidos (USP) dicta el estándar de oro para el control de calidad físico y la disolución de tabletas de Clorhidrato de Metformina de liberación prolongada (ER)[cite: 1].
* **Aplicación en el proyecto:** Alineación estricta con el capítulo general `<711>` de Disolución y la monografía específica del fármaco para fijar las condiciones mecánicas y térmicas de la prueba base (control)[cite: 1].

---

## 2. Parámetros Críticos del Método de Disolución (Alineación USP)

Se detallan las condiciones operativas oficiales extraídas de las especificaciones compendiales para el control analítico[cite: 1]:

| Parámetro Crítico | Especificación de Control | Soporte Normativo / Justificación | Estado |
| :--- | :--- | :--- | :--- |
| **Tipo de Aparato** | Aparato 2 (Paletas / Paddles)[cite: 1] | USP `<711>` / Monografía de Metformina ER[cite: 1] | **Definido** |
| **Velocidad de Agitación** | 100 rpm[cite: 1] | Monografía oficial de tabletas de Metformina ER[cite: 1] | **Definido** |
| **Temperatura del Baño** | 37 ± 0.5 °C[cite: 1] | Capítulo General USP `<711>`[cite: 1] | **Definido** |
| **Volumen del Medio** | 1000 mL[cite: 1] | Requisito de volumen volumétrico compendial[cite: 1] | **Definido** |
| **Medio Oficial (Control)** | Solución amortiguadora de fosfatos pH 6.8[cite: 1] | Medio biorrelevante oficial de la USP[cite: 1] | **Definido** |
| **Medio Modificado (Estrés)** | 80% Buffer Fosfatos pH 6.8 + 20% Sprite[cite: 1] | Surrogato analítico transparente para simular refresco de cola sin interferencia del colorante caramelo IV[cite: 1] | **Definido** |
| **Longitud de Onda (UV)** | 232 nm / 233 nm[cite: 1] | Máximo espectral de absorción de la Metformina en medio acuoso[cite: 1] | **Definido** |
| **Tiempos de Muestreo** | 1, 2, 3, 4, 6, 8 y 10 horas[cite: 1] | Ventana cinética extendida para evaluar la integridad de la matriz polimérica (HPMC)[cite: 1] | **Definido** |

---

## 3. Criterios de Aceptación para la Validación Analítica Cruzada (NOM-177)

Para validar el método espectrofotométrico UV-Vis en el medio modificado por el surrogato (Sprite), se implementan los límites de desempeño técnico mandatados por la NOM-177-SSA1-2013[cite: 1]:

### 3.1 Linealidad y Rango
* **Criterio de Aceptación:** Elaboración de una curva de calibración compuesta por un mínimo de 5 puntos de concentración[cite: 1].
* **Límite Estadístico:** El coeficiente de correlación lineal ($r$) obtenido mediante regresión por mínimos cuadrados debe ser $\ge 0.99$[cite: 1].

### 3.2 Precisión (Sistemas y Operación)
* **Criterio de Aceptación:** Evaluación de la repetibilidad y la precisión intermedia del sistema analítico[cite: 1].
* **Límite Estadístico:** El coeficiente de variación porcentual ($CV\%$) de las réplicas analizadas no debe exceder el $\le 3\%$[cite: 1].

### 3.3 Selectividad (Especificidad)
* **Criterio de Aceptación:** Demostración de que los componentes del medio de estrés no interfieren con el analito[cite: 1].
* **Límite Estadístico:** La lectura de los blancos (mezcla de solución amortiguadora y Sprite desgasificado) a la longitud de onda de detección debe demostrar una absorbancia nula o una ausencia total de señales interferentes a 232-233 nm[cite: 1].

### 3.4 Influencia del Filtro (Adsorción)
* **Criterio de Aceptación:** Cuantificación del porcentaje de retención o adherencia del principio activo al material de filtración[cite: 1].
* **Límite Estadístico:** La variación o diferencia absoluta entre las muestras filtradas y las muestras de referencia no filtradas (centrifugadas) debe ser $\le 2\%$[cite: 1].

### 3.5 Estabilidad de la Muestra
* **Criterio de Aceptación:** Evaluación de la degradación temporal del fármaco expuesto a las condiciones del ensayo[cite: 1].
* **Límite Estadístico:** La pérdida o degradación acumulada del analito disuelto en el medio modificado durante la ventana de tiempo del ensayo debe ser $\le 3\%$[cite: 1].

---

## 4. Criterios Estadísticos para la Comparación de Perfiles

El dictamen técnico final del fenómeno de *dose dumping* se ejecutará de acuerdo con los modelos matemáticos autorizados por la legislación mexicana[cite: 1]:

### 4.1 Factor de Similitud ($f_2$)
* **Equivalencia ($f_2 \ge 50$):** Si el valor resultante es igual o mayor a 50, se asume que la velocidad de liberación es similar, confirmando la hipótesis nula ($H_0$) de que la matriz polimérica resistió de forma íntegra el estrés fisicoquímico[cite: 1].
* **Dose Dumping ($f_2 < 50$):** Un valor inferior a 50 dictamina matemáticamente una alteración crítica y no equivalente en la cinética de liberación, demostrando la hipótesis de trabajo ($H_1$) y confirmando la presencia del fenómeno de *dose dumping* inducido por el medio carbonatado[cite: 1].

### 4.2 Restricciones de Variabilidad Cinética
Para que el cálculo del factor $f_2$ sea estadísticamente válido ante la NOM-177-SSA1-2013, la dispersión de los datos colectados debe cumplir las siguientes cotas de variabilidad[cite: 1]:
* **Primer punto de muestreo:** El coeficiente de variación ($CV\%$) de los porcentajes disueltos acumulados entre las unidades de prueba debe ser $\le 20\%$[cite: 1].
* **Tiempos subsecuentes:** A partir del segundo punto de muestreo y hasta la finalización del perfil, el coeficiente de variación ($CV\%$) máximo permitido es de $\le 10\%$[cite: 1].