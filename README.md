# 🧩 API - Combustibles Unigas | ERP SIESA  
![version](https://img.shields.io/badge/Versión-1.26.10.28-blue.svg)  
![estado](https://img.shields.io/badge/Estado-Estable-brightgreen.svg)  
![ERP](https://img.shields.io/badge/ERP-SIESA-orange.svg)

---

## 📘 Descripción General  

La **API de Combustibles Unigas** proporciona acceso a los **maestros de configuración corporativos** utilizados por las distintas **unidades de negocio** de la organización.  

Su propósito es **unificar y homologar** las estructuras de datos con el **ERP SIESA**, garantizando coherencia, trazabilidad e integración fluida entre sistemas.  

Mediante **consultas y conectores dinámicos**, permite una **integración automatizada**, optimizando procesos, reduciendo duplicidades y centralizando la información maestra.  

---

## ⚙️ Funcionalidad  

Ofrece un conjunto integral de servicios para la **gestión y consulta dinámica de maestros corporativos**, facilitando la interoperabilidad con el **ERP SIESA** y sistemas externos.

### 🔹 Principales funcionalidades  

- **Consultas dinámicas** de terceros con filtros flexibles.  
- Obtención de **maestros**:
  - Compañías  
  - Unidades de negocio  
  - Bodegas  
  - Centros de operación  
  - Unidades de medida  
  - Ítems  
- **Cuentas por Cobrar (CxC)**:
  - Detalle de movimientos por cliente  
  - Consolidado general de saldos  
- **Cuentas por Pagar (CxP)**:
  - Detalle de facturas y documentos asociados  
  - Consolidado general de obligaciones  
- **Creación dinámica de terceros (POST)**  
- **Gestión comercial**:
  - Remisiones  
  - Ventas de contado  
  - Facturación electrónica  
- **Servidor de pruebas** para validación antes de producción  

---

## 🔗 Integración y Pruebas  

Los endpoints están disponibles en el **servidor de pruebas** para validar consultas y conectores antes del paso a producción.  

| Entorno | Ruta Base |
|----------|------------|
| 🧪 **QA / Pruebas** | `/ConnektaQA` |
| 🚀 **Producción** | `/Core` |

---

### 💻 Ejemplo `curl`

```bash
curl -X 'GET' \
  'http://SERVER/v3/CONSULTA_CONECTOR?PARAMETROS' \
  -H 'accept: */*' \
  -H 'Key: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX' \
  -H 'Token: WSXWSXWSXWSXWSXWSXWSXWSXWSXWSXWSXWsdSXQ'
```

### 🔍 Ejemplo de Endpoint
![GET](https://img.shields.io/badge/GET-brightgreen.svg) 
```bash
GET http://SERVER/v3/CONSULTA_CONECTOR?PARAMETROS
```

![POST](https://img.shields.io/badge/POST-orange.svg) 
```bash
POST http://SERVER/v3/CONSULTA_CONECTOR?PARAMETROS
```