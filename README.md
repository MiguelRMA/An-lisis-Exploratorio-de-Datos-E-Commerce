# 🛒 E-Commerce Customer Behavior — Análisis Exploratorio (EDA)

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Estado-Completado-green?style=for-the-badge)

## 📌 Descripción del Proyecto
Este proyecto aborda el Análisis Exploratorio de Datos (EDA) sobre un conjunto de datos de comportamiento de clientes en comercio electrónico. El objetivo principal es limpiar, transformar y preparar los datos para análisis analíticos y predictivos posteriores, garantizando la integridad de los datos y la ausencia de **fuga de información (Data Leakage)**.

---

## 🔑 Hallazgos y Decisiones Clave del EDA

1. **Eliminación de Fuga de Datos (Data Leakage):**
   - Se removieron variables *post-hoc* como `Tiempo_entrega` y `Valoracion_cliente` para evitar que influyan indebidamente en modelos predictivos en tiempo real.
2. **Tratamiento de Valores Atípicos (Outliers):**
   - Utilizando el **Rango Intercuartílico (IQR)** en variables monetarias (`Precio_unitario`, `Descuento` y `Monto_Total`), la muestra se redujo de **17,049** a **11,558** registros limpios.
3. **Ingeniería de Características:**
   - Se consolidó la variable `Monto_Bruto` para analizar el valor real del carrito de compra antes de la aplicación de descuentos.

---

## 🛠️ Tecnologías y Librerías Utilizadas
* **Python** (Lógica principal de tratamiento de datos)
* **Pandas** (Limpieza, filtrado e ingeniería de características)
* **NumPy** (Operaciones numéricas y cálculo de coeficientes)

---

## 🚀 Cómo Ejecutar el Proyecto

1. Clona este repositorio:
   ```bash
   git clone [https://github.com/tu-usuario/ecommerce-eda-customer-behavior.git](https://github.com/tu-usuario/ecommerce-eda-customer-behavior.git)
   ```
2. Instala las dependencias necesarias:
   ```bash
   pip install pandas numpy
   ```
3. Ejecuta el script principal o abre el Jupyter Notebook asociado.
