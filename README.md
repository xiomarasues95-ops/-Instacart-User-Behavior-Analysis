# 🛒 Análisis de Comportamiento de Usuarios — Instacart

> **Autor:** Xiomara Suescun Naizaque | Data Analyst Junior  
> **Herramientas:** Python · Pandas · Matplotlib  
> **Tipo de análisis:** Data Cleaning + Análisis Exploratorio (EDA)

---

## 📌 Contexto y Objetivo

Instacart es una plataforma de entrega de supermercado a domicilio. Este proyecto analiza el comportamiento de compra de sus usuarios a partir de más de **3 millones de registros**, con el objetivo de identificar patrones de consumo, productos más populares y frecuencias de recompra para apoyar decisiones estratégicas de negocio.

---

## 🗂️ Dataset

| Archivo | Descripción |
|--------|-------------|
| `instacart_orders.csv` | Pedidos realizados por usuario |
| `products.csv` | Catálogo de productos |
| `aisles.csv` | Categorías de pasillos |
| `departments.csv` | Departamentos de la tienda |
| `order_products.csv` | Productos por pedido (+3M registros) |

---

## 🔧 Metodología

**Paso 1 — Descripción de los datos**  
Carga y exploración inicial de los 5 datasets para entender su estructura y tipos de datos.

**Paso 2 — Preprocesamiento (Data Cleaning)**  
- Eliminación de **15 pedidos duplicados** (todos del miércoles a las 2:00 a.m.)  
- Tratamiento de **104 nombres de productos duplicados**  
- Valores ausentes en `product_name` reemplazados con `'Unknown'`  
- Valores ausentes en `add_to_cart_order` reemplazados con `999` (pedidos con más de 64 productos)

**Paso 3 — Análisis Exploratorio (EDA)**  
Visualizaciones y métricas para responder preguntas clave sobre comportamiento de usuarios, distribución de pedidos y tasas de recompra.

---

## 📊 Hallazgos Principales

### ⏰ Comportamiento por hora y día
- 📈 Mayor volumen de pedidos entre las **10:00 a.m. y 4:00 p.m.**
- 📉 Actividad mínima entre la **1:00 a.m. y 5:00 a.m.**
- 📅 **Domingo y lunes** concentran el mayor número de pedidos semanales
- 📅 **Jueves** registra el volumen más bajo de la semana

### 👥 Comportamiento de los clientes
- **55,357 clientes** realizaron únicamente 1 pedido — alta tasa de abandono tras la primera compra
- La mayoría compra entre **1 y 5 productos** por pedido
- El usuario con mayor fidelidad registra una **tasa de recompra del 93%**

### 🥦 Productos más populares
- 🍌 Las **bananas** son el producto más pedido y reordenado
- La mayoría del top 20 corresponde a **productos orgánicos**: fresas, espinacas baby, aguacate Hass
- Los **Chocolate Sandwich Cookies** tienen una tasa de recompra del **56%**
- La **cebolla amarilla orgánica** fue reordenada **1,246 veces**
- Top 3 primer artículo añadido al carrito: bananas · bolsa orgánica de bananas · leche entera orgánica

---

## 💡 Recomendaciones

1. **Retención de usuarios** — Campañas de reactivación para los +55,000 clientes con un solo pedido
2. **Reabastecimiento prioritario** — Garantizar inventario de bananas y productos orgánicos los domingos y lunes
3. **Optimización horaria** — Concentrar notificaciones y promociones entre las 10:00 a.m. y 4:00 p.m.
4. **Programa de fidelización** — Beneficios especiales para clientes con tasa de recompra superior al 80%
5. **Expansión orgánica** — Ampliar el catálogo orgánico y crear secciones destacadas en la app

---

## ✅ Conclusión

El análisis revela que los usuarios de Instacart prefieren comprar en la primera mitad del día y los primeros días de la semana, con una marcada preferencia por productos orgánicos frescos. La alta tasa de clientes con un solo pedido representa el principal reto de retención, mientras que la lealtad hacia productos específicos ofrece una oportunidad estratégica para fortalecer el catálogo y las campañas de marketing.

---

## 📁 Estructura del Proyecto