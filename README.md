# 🧩 API - Combustibles Unigas | ERP SIESA
# Ver. 1.26.10.28

## 📘 Descripción General

Esta API proporciona acceso a los **maestros de configuración** utilizados por las distintas **unidades de negocio** y **verticales** de la organización.  
Su propósito es **unificar y homologar** las estructuras de datos con el **ERP corporativo**, garantizando coherencia y trazabilidad en la información.

A través de **consultas y conectores dinámicos**, la API permite una **integración automatizada y flexible** entre sistemas, optimizando los procesos de sincronización, reduciendo duplicidades y asegurando una **gestión centralizada** de los parámetros maestros.

---

## ⚙️ Funcionalidad

La API ofrece un conjunto integral de servicios orientados a la **gestión y consulta dinámica de maestros corporativos** y operaciones transversales del sistema **ERP**, facilitando la interoperabilidad con el **ERP SIESA** y otros sistemas externos.

### 🔹 Principales funcionalidades

- **Consultas dinámicas de terceros**, permitiendo la búsqueda y filtrado flexible de entidades externas.  
- Obtención de **maestros**:
  - Compañías  
  - Unidades de negocio  
  - Bodegas  
  - Centros de operación  
  - Unidades de medida  
  - Ítems  
- Consultas de **Cuentas por Cobrar (CxC)**:
  - Detalle de movimientos por cliente  
  - Consolidado general de saldos  
- Consultas de **Cuentas por Pagar (CxP)**:
  - Detalle de facturas y documentos asociados  
  - Consolidado general de obligaciones  
- **Creación dinámica de terceros (POST)**  
- **Gestión comercial**:
  - Remisiones de venta  
  - Ventas de contado  
  - Facturación electrónica  
- **Servidor de pruebas** para validación de flujos y conectores antes de pasar a producción  

---

### 🔗 Integración y Pruebas

Los endpoints están disponibles en el servidor de pruebas, donde se pueden ejecutar consultas y validar los conectores dinámicos antes de su implementación definitiva en producción.

### Servidor de pruebas:
```html
/ConnektaQA
```

### Servidor de producción:
```html
/Core
```

### Curl
```html
curl -X 'GET' \
  'http://SERVER/v3/CONSULTA_CONECTOR?PARAMETROS' \
  -H 'accept: */*' \
  -H 'Key: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX' \
  -H 'Token: WSXWSXWSXWSXWSXWSXWSXWSXWSXWSXWSXWsdSXQ'
```

### Request URL
```html
http://SERVER/v3/CONSULTA_CONECTOR?PARAMETROS'
```

### Response Headers
```html
 content-length: 436 
 content-type: application/json; charset=utf-8 
 date: Wed,29 Oct 2025 00:35:07 GMT 
 server: Microsoft-IIS/10.0 
 x-powered-by: ASP.NET 
```

---
## 🧠 Ejemplos de Respuesta

### ✅ 200 - Aceptado
```json
{
  "status": 200,
  "message": "Consulta procesada correctamente",
  "data": [
    {
      "codigo": "B001",
      "descripcion": "Bodega Principal Bogotá",
      "estado": "Activo"
    }
  ]
}
```

---

### 🕓 200 - Pendiente
```json
{
  "status": 200,
  "message": "Solicitud recibida, en proceso de sincronización con ERP",
  "job_id": "SYNC-984512",
  "timestamp": "2025-10-28T15:32:45Z"
}
```

---

### ❌ 400 - Bad Request
```json
{
  "status": 400,
  "error": "Parámetros inválidos o faltantes",
  "detalle": "El campo 'unidad_negocio' es obligatorio para esta consulta."
}
```

---

### ❌ 401 - Bad Request
```json
{
  "status": 401,
  "error": "No tiene autorización",
  "detalle": "No tiene autorización"
}
```

---

### ❌ 404 - Bad Request
```json
{
  "status": 404,
  "error": "Recurso de destino no existe",
  "detalle": "Recurso de destino no existe"
}
```

---

### ❌ 500 - Bad Request
```json
{
  "status": 500,
  "error": "Error interno en el servidor",
  "detalle": "Error interno en el servidor"
}
```