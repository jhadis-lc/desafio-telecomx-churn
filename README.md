# 📌 Informe Final: Análisis de Churn en Telecom X

## 🔹 Introducción
Telecom X enfrenta una alta tasa de evasión de clientes. Este análisis busca identificar los factores que influyen en la cancelación de servicios, para apoyar al equipo de Data Science en la construcción de un modelo predictivo.

## 🔹 Limpieza y Tratamiento de Datos
- Se extrajeron datos desde una API en formato JSON.
- Se aplanaron estructuras anidadas con `pd.json_normalize()`.
- Se limpiaron valores nulos en `TotalCharges`.
- Se estandarizaron variables categóricas (ej: "Sí" → "Yes").
- Se creó la columna `Cuentas_Diarias` para análisis diarios.

## 🔹 Hallazgos Clave
- **Churn general**: ~26% de los clientes han cancelado.
- **Contrato mensual**: Muy alta tasa de churn.
- **Clientes nuevos**: Los primeros 12 meses son críticos.
- **Alto cargo mensual**: Asociado a mayor cancelación.
- **Sin pareja o dependientes**: Mayor riesgo de churn.
- **Facturación electrónica**: Más común entre quienes cancelan.

## 🔹 Recomendaciones
1. **Ofrecer descuentos en contratos anuales** para nuevos clientes.
2. **Programa de retención** en los primeros 6 meses.
3. **Personalizar ofertas** para clientes con alto `MonthlyCharges`.
4. **Mejorar soporte técnico** para usuarios de fibra óptica.
5. **Comunicación proactiva** con clientes solteros sin dependientes.
