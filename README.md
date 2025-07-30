# 📊 TelecomX – Análisis de Evasión de Clientes (Churn)

## 🧠 Descripción

Este proyecto forma parte del challenge **TelecomX** de Alura Latam. El objetivo es analizar el comportamiento de los clientes de una empresa de telecomunicaciones para entender las causas de evasión (**Churn**) y proponer soluciones estratégicas basadas en datos.

Se utilizó Python en Google Colab junto con bibliotecas como Pandas, Seaborn y Plotly para procesar los datos, realizar limpieza, visualizaciones y extraer insights clave.

---

## 📁 Estructura del Proyecto

├── TelecomX_Data.json # Dataset principal (formato JSON)
├── TelecomX_Challenge.ipynb # Notebook con el análisis completo
├── README.md # Este archivo descriptivo


---

## 🚀 Tecnologías y Herramientas

- Python 3
- Pandas
- Seaborn y Matplotlib
- Plotly Express
- Google Colab

---

## 🧹 Limpieza y Preprocesamiento

- Carga del dataset desde archivo JSON
- Expansión de columnas anidadas (`customer`, `phone`, `internet`, `account`)
- Conversión de tipos (`Charges.Total` a numérico)
- Normalización de texto (minúsculas y sin espacios)
- Eliminación y tratamiento de valores faltantes
- Creación de nuevas variables:
  - `Cuentas_Diarias` (cargos mensuales / 30)
  - `Servicios_Contratados` (suma de servicios activos)
  - `tenure_group` (antigüedad categorizada)

---

## 📊 Análisis Exploratorio (EDA)

- Distribución de `Churn` (clientes que se quedan vs. se van)
- Relación entre `Churn` y variables como:
  - Tipo de contrato
  - Tiempo como cliente (`tenure`)
  - Monto facturado (`Charges.Monthly`, `Charges.Total`)
  - Tipo de servicio de internet y método de pago
  - Cantidad de servicios contratados
- Gráficos de barras, violín, cajas y mapas de calor de correlación

---

## 🔍 Insights Relevantes

- Clientes con **menos de 12 meses** de antigüedad son más propensos a abandonar el servicio.
- **Contratos mensuales** tienen tasas de churn significativamente más altas que contratos anuales o bianuales.
- Clientes con **más servicios contratados** tienen mayor retención.
- **Altos cargos mensuales** no necesariamente implican mayor evasión, pero sí mayor dispersión.

---

## 🧭 Recomendaciones Estratégicas

1. **Segmentar y fidelizar a nuevos clientes** (primeros 12 meses).
2. **Fomentar contratos anuales** mediante promociones.
3. **Incentivar la contratación de múltiples servicios** (TV, seguridad, soporte).
4. Analizar los métodos de pago con mayor churn para mejorar la experiencia.
5. Desarrollar un **modelo predictivo de churn** para prevenir cancelaciones futuras.

---

## 🛠 Cómo ejecutar este proyecto

1. Clona el repositorio o descarga los archivos.
2. Abre el archivo `TelecomX_Challenge.ipynb` en Google Colab o Jupyter Notebook.
3. Carga el archivo `TelecomX_Data.json` en el entorno.
4. Ejecuta las celdas del notebook para ver todo el análisis paso a paso.

---

## 📌 Notas finales

Este proyecto representa una fase de **análisis exploratorio**. Como paso siguiente se puede:
- Entrenar modelos de machine learning (Logistic Regression, Random Forest, etc.)
- Implementar dashboards con Streamlit o Power BI
- Aplicar soluciones de retención personalizadas con los insights obtenidos

---

> Desarrollado por Marlon Miranda – Participante del programa ONE – Oracle + Alura Latam 🚀
