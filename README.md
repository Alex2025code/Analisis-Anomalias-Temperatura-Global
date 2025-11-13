# 🌍 Análisis de Anomalías de Temperatura Global (NASA GISTEMP, 1880–2025)

## 📘 Descripción general

Este proyecto analiza la evolución de las **anomalías de temperatura global** desde 1880 hasta 2025, utilizando datos del **Global Land–Ocean Temperature Index** del [NASA Goddard Institute for Space Studies (GISS)](https://data.giss.nasa.gov/gistemp/).

El objetivo principal es **visualizar, interpretar y modelar** la tendencia del calentamiento global a lo largo del tiempo, combinando análisis exploratorio de datos (EDA) y técnicas básicas de *Machine Learning* (regresión lineal).

---

## 🧭 Contexto del dataset

El dataset recopila anomalías de temperatura promedio mensuales y anuales, medidas en grados Celsius (°C), respecto al promedio base **1950–1980**.

- **Valores positivos (+)** → años más cálidos que el promedio base  
- **Valores negativos (–)** → años más fríos que el promedio base

**Fuente:**  
> NASA Goddard Institute for Space Studies (GISS), *Global Land-Ocean Temperature Index (GISTEMP)*  
> [https://data.giss.nasa.gov/gistemp/](https://data.giss.nasa.gov/gistemp/)

---

## ⚙️ Contenido del proyecto

El análisis se desarrolló en un entorno **Jupyter Notebook (Python)** e incluye las siguientes etapas:

### 1️⃣ Importación y descripción de datos
- Carga del dataset original NASA GISTEMP.  
- Descripción de las variables principales y verificación del formato temporal.

### 2️⃣ Análisis exploratorio de datos (EDA)
Incluye visualizaciones y análisis de tendencia:

- Evolución del promedio anual de anomalías (1880–2025).  
- Promedio por década.  
- Distribución de anomalías anuales y estacionales.  
- Correlaciones entre estaciones del año.  
- Comparación de patrones térmicos entre periodos históricos.

**🧩 Conclusión EDA:**  
El análisis visual confirma una **tendencia sostenida de calentamiento global**, especialmente acentuada desde 1980.  
Todas las estaciones muestran aumentos coherentes, con inviernos siendo los más afectados.

### 3️⃣ Etapa de Machine Learning
- Modelo de **Regresión Lineal Simple**, donde la variable predictora es el **año** y la variable respuesta es la **anomalía anual (J-D)**.  
- Evaluación mediante métricas:  
  - **R² = 0.815**  
  - **RMSE = 0.143 °C**  
- Interpretación y proyección de tendencia hasta 2050.

**📊 Conclusión ML:**  
El modelo logra explicar más del **80% de la variabilidad** de las anomalías, confirmando un **patrón de calentamiento sostenido y no aleatorio**.

---

## 📈 Principales resultados

- El calentamiento global se intensifica a partir de **1980**, con anomalías que superan **+1.0 °C** en las últimas décadas.  
- Alta **correlación entre estaciones (r > 0.9)**, reflejando un calentamiento uniforme a nivel global.  

- La **proyección lineal** estima un aumento adicional de **≈ 0.21 °C hacia 2050**, aunque la aceleración reciente podría superar esta estimación.

---

## 🧩 Requisitos técnicos

**Lenguaje:** Python 3.10+  
**Entorno recomendado:** VS Code o Jupyter Notebook  

**Librerías principales:**
```bash
pandas
numpy
matplotlib
seaborn
scikit-learn

## 🧠 Reflexión Final

Los resultados evidencian que el calentamiento global no es una fluctuación temporal, sino una tendencia persistente y acelerada.  
Cada año la Tierra se calienta un poco más, y las proyecciones indican que este proceso continuará a menos que se tomen medidas significativas para mitigar las emisiones.  
El futuro climático dependerá de las acciones que se adopten hoy.

### ✍️ Autor

**Alexis Ortiz D.**  
Proyecto académico de análisis climático con fines educativos y de divulgación científica.  
Basado en datos abiertos de la **NASA Goddard Institute for Space Studies (GISS)**.