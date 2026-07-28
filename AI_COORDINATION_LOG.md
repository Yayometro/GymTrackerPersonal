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
- **Petición del Usuario**:
  1. Mantener intacto el archivo `yayo-panel-salud-original.html` como referencia.
  2. Mantener fija en la parte superior la información del peso actual (**98.3 kg**), la barra de recorrido (Máximo 101.5 kg → Actual 98.3 kg → Meta 80 kg), las tarjetas de **Métricas Clave** y la gráfica canvas de **Tendencia de Peso**.
  3. Crear un sistema de 4 pestañas:
     - **🔥 Calorías por Escenario**: Pestaña principal y abierta por defecto (Estándar).
     - **⚖️ Historial de Peso**: Tabla con los registros de peso.
     - **🧬 Composición Corporal**: Tarjetas de masa magra/grasa + Tabla comparativa de medidas.
     - **📏 Historial Completo de Medidas**: Tabla completa de 14 entradas con scroll horizontal.
  4. **Inversión Cronológica de Tablas**:
     - *Historial de Peso*: Registros más nuevos (Julio 2026) arriba, más antiguos (Septiembre 2025) abajo.
     - *Comparativa de Medidas*: Columna más reciente (Julio 25 '26) a la izquierda, más antiguas hacia la derecha.
     - *Historial Completo de Medidas*: Entradas más recientes arriba, más antiguas abajo.
  5. Mantener persistente en el footer las tarjetas/chips de **Macros Objetivo** y los métodos de cálculo.
  6. Crear este documento de coordinación (`AI_COORDINATION_LOG.md`).
  7. Conectar y subir el proyecto al repositorio de GitHub: `https://github.com/Yayometro/GymTrackerPersonal.git`.

---

### 📌 Sesión 3 — Reorganización de Módulos y Gráficas de Espalda/Panza
- **Proveedor de IA**: Google
- **Asistente**: Antigravity AI Coding Assistant
- **Modelo**: Gemini 3.6 Flash (Nivel de Razonamiento: High)
- **Fecha**: 27 de Julio, 2026 (22:35 UTC-6)
- **Resumen**: Métricas clave movidas al footer arriba de macros. Composición corporal movida al header persistente. Agregadas gráficas canvas para Espalda y Panza en el Historial de Medidas.

---

### 📌 Sesión 4 — Gráficas Específicas de Masa Magra/Grasa, Eje de Tiempos Vertical y Tooltips Hover Interactivos
- **Proveedor de IA**: Google
- **Asistente**: Antigravity AI Coding Assistant
- **Modelo**: Gemini 3.6 Flash (Nivel de Razonamiento: High)
- **Fecha**: 27 de Julio, 2026 (22:42 UTC-6)
- **Petición del Usuario**:
  1. **Gráfico Dedicado de Masa Magra en Composición Corporal**: Agregar un gráfico específico para visualizar la evolución de la Masa Magra (kg) con base en la fórmula de la Naval USA (69.8 kg → 74.5 kg → 73.0 kg actual).
  2. **Gráficos en Historial de Peso**: Agregar dos gráficos interactivos:
     - 🏋️‍♂️ **Evolución de Masa Magra (kg)**
     - 📉 **Evolución de Masa Grasa (kg)**
  3. **Líneas Verticales de Tiempo (Eje X)**: Dibujar líneas de cuadrícula discontinuas verticales que muestren hitos de tiempo explícitos (Sep '25, Oct '25, Dic '25, Ene '26, Abr '26, Jul '26) en todas las 6 gráficas del sitio.
  4. **Tooltips Interactivos al pasar el Cursor (Hover)**: Implementar detección de mouse por proximidad en canvas (`bindCanvasHover`) para mostrar un tooltip flotante con fecha, valor exacto y etiqueta de hito al pasar el cursor.
  5. Sincronizar en GitHub.

---

## 📌 Estado Actual del Repositorio para la Siguiente IA
- **Entorno**: HTML5 / CSS3 Vanilla / JS Vanilla / HTML5 Canvas (6 gráficas interactivas con tooltips y líneas guía).
- **Punto de Entrada**: `index.html`
- **Gráficas Disponibles**:
  1. `wtCanvas` (Peso total en header persistente)
  2. `leanWeightCanvas` (Masa Magra en Historial de Peso)
  3. `fatWeightCanvas` (Masa Grasa en Historial de Peso)
  4. `compLeanCanvas` (Masa Magra dedicada en Composición Corporal)
  5. `backCanvas` (Espalda + Pecho en Historial Completo de Medidas)
  6. `waistCanvas` (Panza / Ombligo en Historial Completo de Medidas)
- **Fórmula de % Grasa**: Naval USA para hombres:
  $$\% \text{Grasa} = 86.010 \times \log_{10}(\text{cintura} - \text{cuello}) - 70.041 \times \log_{10}(\text{altura}) + 36.76$$
- **Repositorio Remoto**: `https://github.com/Yayometro/GymTrackerPersonal.git`
