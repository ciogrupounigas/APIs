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

📘 Respuesta exitosa
```json
{
  "status": "OK",
  "mensaje": "Factura emitida correctamente",
  "cufe": "string_cufe"
}

⬅️ Volver al inicio

yaml


---

# ⚙️ Activar GitHub Pages

1. En tu repositorio, ve a **Settings → Pages**.  
2. En **Source**, elegí:  
   - **Branch:** `main`  
   - **Folder:** `/ (root)`  
3. Guardá.

👉 Tu documentación estará en:  
`https://github.dev/ciogrupounigas/APIs/`

---

# 🧠 Qué logramos con esta configuración

✅ Página principal (`README.md`) con descripción general.  
✅ Sidebar **a la derecha** con enlaces jerárquicos.  
✅ **Modo oscuro predeterminado** con opción de tema claro.  
✅ Todo funcionando **desde la raíz del repositorio**, sin `/docs`.  
✅ Compatible 100% con **GitHub Pages**.  

---

¿Querés que el nombre “APIs Combustibles Unigas SAS | Nirvana” se vea en un **header fijo arriba** (como un logo + título central) para hacerlo más institucional?  
Puedo agregarte esa versión del código con un header elegante y responsive.
