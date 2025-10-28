# 🧩 API - Maestros de Configuración | Sistema NSX

## 📘 Descripción General

Esta API permite obtener los **maestros de configuración** utilizados por el sistema **NSX** para consolidar información y homologar las tablas de datos con el ERP corporativo.  
Su objetivo principal es facilitar la **integración dinámica** entre sistemas mediante **consultas y conectores automáticos**, optimizando los procesos de sincronización y evitando duplicidades en la definición de parámetros maestros.

---

## ⚙️ Funcionalidad

- Obtener catálogos maestros (sucursales, productos, clientes, tipos de documento, etc.).
- Centralizar configuraciones compartidas por los distintos módulos del sistema NSX.
- Permitir consultas dinámicas parametrizadas según el tipo de maestro requerido.
- Servir como **base de referencia para los conectores automáticos** hacia el ERP y otros sistemas.

---

## 🌐 Endpoint

```http
GET /api/nsx/config/maestros
```

```ruby
https://api.unigas.com.co/nsx/config/maestros

```
---

## 🧾 Request Header
Encabezado	Tipo	Descripción	Obligatorio
Authorization	String	Token JWT para autenticación Bearer	✅ Sí
Content-Type	String	Tipo de contenido (application/json)	✅ Sí
x-api-key	String	Llave de acceso para validación de seguridad adicional	❌ No

Ejemplo:

```json
{
  "Authorization": "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...",
  "Content-Type": "application/json"
} 
```
