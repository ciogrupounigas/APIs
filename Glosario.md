# 📘 Glosario API REST

Este glosario reúne los términos técnicos más comunes utilizados en la documentación de las APIs del sistema.  
Sirve como referencia rápida para desarrolladores, analistas y personal técnico que interactúa con los servicios REST.

---

## 🧩 Conceptos Generales

| Término | Descripción |
|----------|-------------|
| **API (Application Programming Interface)** | Conjunto de reglas que permiten la comunicación entre sistemas de software. En este contexto, la API expone datos o funcionalidades del sistema mediante peticiones HTTP. |
| **REST (Representational State Transfer)** | Estilo de arquitectura que utiliza los métodos HTTP estándar (GET, POST, PUT, DELETE) para realizar operaciones sobre recursos. |
| **Endpoint** | URL específica a la que se realiza una solicitud para interactuar con un recurso o servicio dentro de la API. Ejemplo: `/api/v1/clientes`. |
| **Recurso** | Entidad o dato que puede ser accedido o manipulado a través de la API. Ejemplo: Cliente, Factura, Producto. |
| **JSON (JavaScript Object Notation)** | Formato estándar para el intercambio de datos estructurados entre cliente y servidor. |
| **HTTP (Hypertext Transfer Protocol)** | Protocolo utilizado para la comunicación entre el cliente y el servidor. |
| **Token** | Cadena generada para autenticar y autorizar solicitudes a la API. Generalmente se envía en el encabezado `Authorization`. |

---

## ⚙️ Métodos HTTP

| Método | Uso Principal | Ejemplo |
|---------|----------------|----------|
| **GET** | Consultar información o listar recursos. | `/api/v1/facturas` |
| **POST** | Crear un nuevo recurso. | `/api/v1/facturas` |
| **PUT** | Actualizar un recurso existente (reemplazo completo). | `/api/v1/facturas/123` |
| **PATCH** | Actualizar parcialmente un recurso. | `/api/v1/facturas/123` |
| **DELETE** | Eliminar un recurso. | `/api/v1/facturas/123` |

---

## 🔐 Autenticación y Seguridad

| Término | Descripción |
|----------|-------------|
| **Bearer Token** | Método de autenticación donde se envía un token de acceso en el encabezado `Authorization: Bearer <token>`. |
| **API Key** | Clave única asignada a un cliente o aplicación para acceder a la API. |
| **HTTPS** | Versión segura de HTTP que cifra las comunicaciones entre cliente y servidor. |
| **CORS (Cross-Origin Resource Sharing)** | Mecanismo que controla qué dominios pueden acceder a los recursos de la API. |

---

## 💬 Códigos de Respuesta HTTP

| Código | Estado | Descripción |
|---------|---------|-------------|
| **200 OK** | Éxito | La solicitud se procesó correctamente. |
| **201 Created** | Éxito | El recurso fue creado correctamente. |
| **202 Accepted** | En proceso | La solicitud fue recibida y está siendo procesada. |
| **400 Bad Request** | Error del cliente | La solicitud contiene errores de formato o parámetros inválidos. |
| **401 Unauthorized** | No autorizado | Falta autenticación o el token es inválido. |
| **403 Forbidden** | Prohibido | El usuario no tiene permisos para realizar esta acción. |
| **404 Not Found** | No encontrado | El recurso solicitado no existe. |
| **500 Internal Server Error** | Error del servidor | Ocurrió un error inesperado en el servidor. |

---

## 🧠 Ejemplo de Respuesta JSON

```json
{
  "status": 200,
  "message": "Solicitud procesada exitosamente",
  "data": {
    "id": 101,
    "nombre": "Juan Pérez",
    "email": "jperez@ejemplo.com"
  }
}
```

## 🧾 Ejemplo de Error JSON

```json
Copiar código
{
  "status": 400,
  "error": "BAD_REQUEST",
  "message": "El parámetro 'fecha' es obligatorio"
}
```

🧭 Convenciones de Nombres
Elemento	Convención	Ejemplo
Endpoints	minúsculas, separados por guiones medios	/api/v1/facturas-pendientes
Parámetros	camelCase	fechaInicio, fechaFin
Campos JSON	snake_case	"fecha_emision": "2025-10-29"

📅 Versionado
Las versiones de la API se indican en la URL siguiendo el formato v{número}.
Ejemplo:
https://api.combustiblesunigas.com/v1/facturas

---
© 2025 - Departamento TIC - Combustibles Unigas SAS