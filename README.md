# 🚲🌦️ Ecobici Weather ETL & Analytics (Databricks)

## 🧠 Descripción del proyecto

Este proyecto implementa una arquitectura **end-to-end de Data Engineering** utilizando Databricks, integrando datos de movilidad urbana (Ecobici 🚲) con información climática 🌦️ para analizar cómo las condiciones ambientales impactan el comportamiento de los usuarios.

**Ecobici** es un programa de la **Ciudad de México 🇲🇽** que permite a los ciudadanos utilizar bicicletas compartidas como medio de transporte urbano, promoviendo la movilidad sostenible y reduciendo el uso de vehículos motorizados.

A través de un pipeline ETL basado en **PySpark** y la arquitectura **Medallion (Bronze 🥉, Silver 🥈, Gold 🥇)**, se construye un modelo analítico que permite visualizar patrones relevantes de uso y generar insights accionables.

---

## 🎯 Impacto del análisis

- 🌧️ La lluvia reduce significativamente el uso del sistema Ecobici  
- 🌡️ Existe un rango óptimo de temperatura donde la demanda es mayor  
- 👥 El comportamiento es consistente entre distintos tipos de usuarios  
- 📉 Condiciones climáticas adversas impactan directamente la movilidad urbana  

👉 Aplicaciones:
- planeación operativa  
- estrategias de movilidad urbana  
- promoción del uso del sistema  

---

## 🏗️ Arquitectura del proyecto

### 🧩 Enfoque Medallion

El pipeline sigue la arquitectura:

- 🥉 **Bronze** → datos crudos  
- 🥈 **Silver** → datos limpios e integrados  
- 🥇 **Gold** → datos agregados para análisis  

### 🔄 Flujo de datos

1. 📥 Ingesta de datos Ecobici (dataset)  
2. 🌐 Consumo de API de clima  
3. 🔧 Transformaciones en PySpark  
4. 🔗 Integración por fecha  
5. 📊 Generación de datasets analíticos  
6. 📈 Visualización en Databricks  

### 🧱 Componentes clave

- 🧠 Databricks (Free Edition)  
- 🔥 PySpark  
- 🐍 Python  
- 🗄️ Delta Lake  
- 🌐 API REST (clima)  
- 📊 Visualización en Databricks  
- ⚙️ GitHub Actions (CI/CD)  

---

## 📊 Visualización (BI)

Se construyeron visualizaciones para analizar:

- 🌧️ impacto de lluvia en viajes  
- 🌡️ impacto de temperatura  
- 👥 comportamiento por tipo de usuario  

Tipos de gráficas:

- Scatter plots  
- Line charts  
- comparativos por segmentos  

---

## 🧪 Evidencia de ejecución

Para validar el correcto funcionamiento del pipeline se incluyen evidencias de:

- ✅ ejecución de notebooks (ingestión, transformación y agregación)  
- ✅ creación de tablas en capa GOLD  
- ✅ visualizaciones generadas en Databricks  
- ✅ resultados de queries  

📸 Las evidencias se encuentran en:

👉 `/evidencias`

Incluyen:

- capturas de ejecución  
- resultados de tablas  
- dashboards  

---

## ⚙️ CI/CD 🚀

El proyecto incluye automatización mediante GitHub Actions:

- 🔄 ejecución simulada del pipeline  
- 🧪 validación de procesos  
- 🚀 promoción DEV → PROD  

Archivo: .github/workflows/deploy.yml


---

## 📁 Estructura del repositorio

### 📂 `.github/workflows` ⚙️
Configuración de CI/CD:

- `deploy.yml` → pipeline automatizado de despliegue  

---

### 📂 `PrepAmb` 🧱
Preparación del entorno:

- configuración inicial  
- setup de variables  
- condiciones necesarias para ejecutar el ETL  

---

### 📂 `certificaciones` 🏅 
Evidencias de formación:

- certificaciones Databricks  
- cursos  


---

### 📂 `dashboard` 📊
Elementos de visualización:

- dashboards  
- configuraciones visuales  
- resultados analíticos  

---

### 📂 `datasets` 📦
Datos fuente:

- dataset Ecobici  
- archivos base de ingestión  

---

### 📂 `evidencias` 🧪
Validación del proyecto:

- ejecución de notebooks  
- resultados  
- visualizaciones  

---

### 📂 `proceso` 🔄
Lógica del pipeline ETL:

- ingestión (bronze)  
- transformación (silver)  
- agregación (gold)  

👉 Núcleo del proyecto en PySpark  

---

### 📂 `reversion` 🔁
Control y recuperación:

- mecanismos de rollback  
- control de cambios  

---

### 📂 `seguridad` 🔐
Gobierno y acceso:

- configuración de permisos  
- credenciales  
- seguridad del entorno  

---

### 📄 `README.md`
Documento principal del proyecto  

---

## 🧠 Conclusiones

El análisis confirma patrones claros en el comportamiento de los usuarios:

- 🌧️ La lluvia reduce significativamente los viajes  
- 🌡️ Los usuarios prefieren temperaturas moderadas  
- ❄️☀️ Condiciones extremas disminuyen la demanda  
- 👥 El comportamiento es consistente entre grupos  

👉 En resumen:

Las personas prefieren utilizar Ecobici cuando las condiciones climáticas son favorables, evitando lluvia y temperaturas extremas.

---

## 🚀 Conclusión general

Este proyecto demuestra la implementación completa de un pipeline moderno de datos, integrando múltiples fuentes y generando valor analítico real.

Refleja capacidades en:

- arquitectura de datos  
- integración de fuentes  
- análisis de información  
- automatización de procesos  

---

## 👤 Autor

**Gerardo Rodríguez**  
🔗 https://www.linkedin.com/in/roager/
