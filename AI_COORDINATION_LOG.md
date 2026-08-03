# 🤖 AI Coordination Log — GymTracker Personal

> **Protocolo para Asistentes de IA (Google Gemini, Anthropic Claude, OpenAI ChatGPT, DeepSeek, etc.):**
> Este documento sirve como registro de coordinación entre las diferentes Inteligencias Artificiales que colaboran en este proyecto.
> 
> **Instrucciones para cualquier IA que continúe este proyecto:**
> 1. **Leer este registro** antes de realizar cambios para conocer la estructura del proyecto y decisiones previas.
> 2. **No sobrescribir** `yayo-panel-salud-original.html` (se mantiene como archivo de referencia original).
> 3. **Registrar tu sesión** agregando una entrada al final de este archivo con la siguiente estructura:
>    - **Proveedor de IA**: (Google, Anthropic, OpenAI, DeepSeek, etc.)
>    - **Modelo Exacto & Configuración**: (ej. Gemini 3.6 Flash - Reasoning: High)
>    - **Fecha y Hora**: (Timestamp local o ISO)
>    - **Petición del Usuario**: (Resumen del prompt recibido)
>    - **Cambios Realizados**: (Archivos modificados/creados y decisiones técnicas)
>    - **Estado del Proyecto**: (Archivos actuales y punto de partida para la siguiente IA)

---

## 📜 Historial de Sesiones de IA

### 📌 Sesión 1 — Creación del Panel de Salud Base
- **Proveedor de IA**: Anthropic
- **Modelo**: Claude 3.5 / 3.7 Sonnet
- **Archivo Referencia**: `yayo-panel-salud-original.html`
- **Resumen**: Creación del HTML original del dashboard con métricas clave, composición corporal, historial de peso, comparativa de medidas, escenarios calóricos y macros objetivo.

---

### 📌 Sesión 2 — Estructura de Pestañas y Reordenamiento Cronológico Invertido
- **Proveedor de IA**: Google
- **Asistente**: Antigravity AI Coding Assistant
- **Modelo**: Gemini 3.6 Flash (Nivel de Razonamiento: High)
- **Fecha**: 27 de Julio, 2026 (22:28 UTC-6)
- **Petición del Usuario**: Pestañas de navegación, tablas invertidas (más recientes arriba) y creación de log de coordinación.

---

### 📌 Sesión 3 — Reorganización de Módulos y Gráficas de Espalda/Panza
- **Proveedor de IA**: Google
- **Asistente**: Antigravity AI Coding Assistant
- **Modelo**: Gemini 3.6 Flash (Nivel de Razonamiento: High)
- **Fecha**: 27 de Julio, 2026 (22:35 UTC-6)
- **Resumen**: Métricas clave al footer, composición corporal al header, gráficas para Espalda y Panza.

---

### 📌 Sesión 4 — Gráficas de Masa Magra/Grasa, Eje de Tiempos Vertical y Tooltips Hover Interactivos
- **Proveedor de IA**: Google
- **Asistente**: Antigravity AI Coding Assistant
- **Modelo**: Gemini 3.6 Flash (Nivel de Razonamiento: High)
- **Fecha**: 27 de Julio, 2026 (22:42 UTC-6)
- **Resumen**: Gráficas de Masa Magra y Masa Grasa en Historial de Peso y Composición Corporal, líneas punteadas verticales de tiempo (Sep '25 a Jul '26), tooltips interactivos hover en canvas.

---

### 📌 Sesión 5 — Optimización Responsiva para Móviles, Charts Combinados para Grupos y GitHub Pages
- **Proveedor de IA**: Google
- **Asistente**: Antigravity AI Coding Assistant
- **Modelo**: Gemini 3.6 Flash (Nivel de Razonamiento: High)
- **Fecha**: 27 de Julio, 2026 (22:54 UTC-6)
- **Resumen**: Optimización responsiva con eventos táctiles canvas y gráficos dual-series para Brazos, Hombros y Piernas.

---

### 📌 Sesión 6 — Integración de Escenarios Calóricos (Torso vs Piernas MET)
- **Proveedor de IA**: Google
- **Asistente**: Antigravity AI Coding Assistant
- **Modelo**: Gemini 3.6 Flash (Nivel de Razonamiento: High)
- **Fecha**: 31 de Julio, 2026 (20:20 UTC-6)
- **Resumen**: Adición inicial de escenarios calóricos diferenciados por grupo muscular.

---

### 📌 Sesión 7 — Corrección Basada en el 2024 Adult Compendium of Physical Activities
- **Proveedor de IA**: Google
- **Asistente**: Antigravity AI Coding Assistant
- **Modelo**: Gemini 3.6 Flash (Nivel de Razonamiento: High)
- **Fecha**: 31 de Julio, 2026 (20:28 UTC-6)
- **Petición del Usuario**: Actualización de los escenarios calóricos según la investigación corregida de Claude basada en las tablas oficiales del *2024 Adult Compendium of Physical Activities*.
- **Cambios Realizados**:
  1. **Valores Calóricos Corregidos**:
     - 💪 **Torso 1h30 (MET 5.0 · +770 kcal)**:
       - `#8a` Torso + sedentario: `3,118 kcal` (Maint) | `2,618 kcal` (Opt) | `2,368 kcal` (Agg)
       - `#8b` Torso + 10k pasos plano: `3,693 kcal` (Maint) | `3,193 kcal` (Opt) | `2,943 kcal` (Agg)
       - `#8c` Torso + 10k pasos 5% incl.: `3,973 kcal` (Maint) | `3,473 kcal` (Opt) | `3,223 kcal` (Agg)
     - 🦵 **Piernas 1h30 (MET 5.5 · +851 kcal)**:
       - `#9a` Piernas + sedentario: `3,199 kcal` (Maint) | `2,699 kcal` (Opt) | `2,449 kcal` (Agg)
       - `#9b` Piernas + 10k pasos plano: `3,774 kcal` (Maint) | `3,274 kcal` (Opt) | `3,024 kcal` (Agg)
       - `#9c` Piernas + 10k pasos 5% incl.: `4,054 kcal` (Maint) | `3,554 kcal` (Opt) | `3,304 kcal` (Agg)
  2. **Nota Informativa Realista en Infobox**:
     - Explicación de que la quema intra-workout difiere solo por `+81 kcal` debido a los mayores descansos en piernas, mientras que el beneficio clave radica en el **EPOC (afterburn)** post-ejercicio y la **respuesta hormonal** (Testosterona +16%, GH alta).
  3. **Sincronización Total y Despliegue**:
     - Actualizados `yayo-panel-salud-original.html`, `index.html`, `yayo-panel-salud-tabs.html` y `AI_COORDINATION_LOG.md`.
     - Git commit y push a la rama `main` de GitHub.

---

### 📌 Sesión 8 — Nueva Pestaña de Proyección de Bajada de Peso
- **Proveedor de IA**: Anthropic
- **Modelo**: Claude Sonnet 5
- **Fecha**: 3 de Agosto, 2026
- **Petición del Usuario**: Agregar una pestaña con la proyección de cuánto peso se podría bajar en 12 meses bajo tres escenarios de déficit calórico diario (−500, −700 y −800 kcal), basada en los datos ya existentes del panel (peso actual 98.3 kg, meta 80 kg).
- **Cambios Realizados**:
  1. **Nueva Pestaña `📉 Proyección de Bajada`** en `index.html` y `yayo-panel-salud-tabs.html`:
     - Tabla mes a mes (Mes 1 a Mes 12) con el peso proyectado para −500 kcal/día (seguro), −700 kcal/día y −800 kcal/día (agresivo).
     - Metodología: 1 kg de grasa ≈ 7,700 kcal, proyección lineal (sin ajustar por la reducción gradual del TDEE al bajar de peso).
     - Marca visual (`🎯 Meta alcanzada`) en el mes donde cada escenario llega a los 80 kg: ~mes 9.8 (−500), ~mes 6.6 (−700), ~mes 5.8 (−800).
     - Infobox con el ritmo semanal equivalente de cada escenario (0.45 / 0.64 / 0.73 kg/semana), todos por debajo del umbral de ~1%/semana asociado a mayor riesgo de pérdida muscular (Helms et al. 2014).
  2. **Sincronización**: Actualizados `index.html` y `yayo-panel-salud-tabs.html` (idénticos, sin tocar `yayo-panel-salud-original.html` por protocolo). JS `switchTab()` actualizado para incluir la pestaña `proyeccion`.
  3. **Impacto Estimado en Masa Magra**: 3 tarjetas (una por escenario) con rango de cambio de m&uacute;sculo esperado, basado en el perfil real del usuario (prote&iacute;na 200&ndash;300g/d&iacute;a, entrenamiento a fallo 2x/semana por grupo muscular) y en umbrales de investigaci&oacute;n (Garthe et al. 2011: 0.7%/sem vs 1.4%/sem de p&eacute;rdida de peso en atletas de fuerza):
     - &minus;500 kcal (0.46%/sem): Mantener &rarr; +1 kg
     - &minus;700 kcal (0.65%/sem): &minus;0.3 &rarr; +0.7 kg
     - &minus;800 kcal (0.74%/sem): &minus;1 &rarr; +0.3 kg
  4. Verificado visualmente en navegador antes de publicar.

---

## 📌 Estado Actual del Repositorio para la Siguiente IA
- **Entorno**: HTML5 / CSS3 Vanilla Responsive / JS Vanilla / 9 Gráficas HTML5 Canvas con Tooltips Táctiles y Dual-Series.
- **Punto de Entrada**: `index.html`
- **Pestañas**:
  1. `🔥 Calorías por Escenario` (Con escenarios corregidos según 2024 Compendium: Torso MET 5.0 [+770 kcal] vs Piernas MET 5.5 [+851 kcal])
  2. `⚖️ Historial de Peso` (Tablas + Charts Masa Magra & Masa Grasa)
  3. `🧬 Composición Corporal` (Masa Magra/Grasa + Chart Dedicado Magro + Comparativa)
  4. `📏 Historial Completo de Medidas` (Tabla 14 entradas + 5 Charts: Espalda, Panza, Brazos Izq/Der, Hombros Izq/Der, Piernas Izq/Der)
  5. `📉 Proyección de Bajada` (Proyección de peso a 12 meses para déficits de −500/−700/−800 kcal/día)
- **URL Pública GitHub Pages**: `https://yayometro.github.io/GymTrackerPersonal/`
- **Repositorio Remoto**: `https://github.com/Yayometro/GymTrackerPersonal.git`
