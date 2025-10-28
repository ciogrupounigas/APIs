# Factura Electrónica

Permite emitir una factura válida ante SUNAT.

---

## 🔧 Endpoint
POST /api/factura/emitir

bash
Copiar código

## 🧾 Ejemplo de solicitud
```json
{
  "ruc": "20100066603",
  "serie": "F001",
  "numero": 123,
  "monto": 150.50,
  "cliente": {
    "ruc": "10454545454",
    "razon_social": "Cliente Demo SAC"
  }
}
📘 Respuesta exitosa
json
Copiar código
{
  "status": "OK",
  "mensaje": "Factura emitida correctamente",
  "cdr": "string_base64"
}
