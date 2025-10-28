# Factura Electrónica

Permite emitir una factura válida ante la DIAN (Colombia).

---

## 🧩 Endpoint
POST /api/factura/emitir


## 🧾 Ejemplo de solicitud

```json
{
  "nit": "900999888",
  "serie": "F001",
  "numero": 123,
  "monto": 250000,
  "cliente": {
    "nit": "1010101010",
    "razon_social": "Cliente Demo SAS"
  }
}
```

## 📘 Ejemplo de solicitud

```json
{
  "status": "OK",
  "mensaje": "Factura emitida correctamente",
  "cufe": "string_cufe"
}
```