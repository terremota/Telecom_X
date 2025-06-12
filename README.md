
# 📊 Análisis de Evasión de Clientes - Telecom X

Este proyecto forma parte de un desafío de análisis de datos para la empresa **Telecom X**, que busca reducir su alta tasa de abandono de clientes (**churn**). A través de técnicas de limpieza, transformación y análisis exploratorio, se identifican los factores clave que influyen en el comportamiento de evasión de los usuarios.

---

## 🧾 Descripción del Proyecto

El objetivo principal es comprender por qué los clientes abandonan el servicio, a través del análisis de datos históricos proporcionados en formato JSON.

El flujo del proyecto incluye:
- Carga y aplanamiento de datos anidados.
- Limpieza e imputación de valores faltantes.
- Transformación de datos (nuevas variables, conversión de tipos).
- Análisis descriptivo y visualización.
- Identificación de patrones y propuesta de estrategias de retención.

---

## 🧠 Principales Herramientas y Librerías

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn` *(opcional para visualización avanzada)*
- `json_normalize` para estructuras anidadas

---

## 🗃️ Estructura del Proyecto

```
├── TelecomX_Data.json          # Archivo de datos original en JSON
├── analysis_telecom_x.ipynb    # Notebook con todo el proceso
├── preprocess.py               # Script de preprocesamiento (opcional)
└── README.md                   # Este archivo
```

---

## ⚙️ Pasos del Análisis

1. **Carga y exploración de los datos**
   - Lectura del JSON
   - Inspección de columnas y tipos

2. **Transformación**
   - Aplanamiento de columnas anidadas (`customer`, `account`)
   - Eliminación de columnas irrelevantes
   - Conversión de tipos y tratamiento de valores nulos o inconsistentes
   - Cálculo de nueva variable: `Cargo.Diario`

3. **Análisis exploratorio**
   - Estadísticas descriptivas de variables clave
   - Tablas cruzadas (Churn vs Contract, PaymentMethod, etc.)
   - Visualización con gráficos de barras

4. **Conclusiones**
   - Contratos mensuales y pagos electrónicos se asocian a mayor churn
   - La facturación electrónica podría estar ligada a una experiencia negativa
   - El género no es un factor determinante

---

## 📌 Hallazgos Clave

- Los contratos **mensuales** presentan una tasa de evasión del **41%**, en comparación con solo el **2.7%** en contratos de dos años.
- El método de pago **electronic check** está relacionado con una tasa de churn superior al **43%**.
- Usuarios que eligen la facturación electrónica presentan también una mayor tasa de abandono.

---

## 🎯 Recomendaciones Estratégicas

- Incentivar contratos de largo plazo con beneficios atractivos.
- Mejorar la experiencia de usuario en pagos electrónicos y facturación digital.
- Implementar programas de retención temprana basados en duración del contrato (`tenure`).

---

## 🚀 Próximos pasos

- Entrenamiento de modelos predictivos (logistic regression, decision trees, etc.)
- Segmentación avanzada de clientes por riesgo
- Dashboard interactivo con herramientas como Plotly o Dash

---

## 🤝 Autor

- **Tu Nombre** ([@tucuenta](https://github.com/tucuenta))  
- Desarrollador en formación | Apasionado por la ciencia de datos 📈

---

## 📄 Licencia

Este proyecto es parte de un desafío académico y no está asociado oficialmente con ninguna empresa real. Uso educativo.
