![GET](https://img.shields.io/badge/v3/EjecutarConsulta-GET-brightgreen.svg)

---
En cuanto al consumo de la **API**, la información de autenticación (credenciales, claves o tokens)
será suministrada por un canal seguro e independiente, utilizando mecanismos temporales de
intercambio de información confidencial, tales como OneTimeSecret, PwPush o ZeroBin.

Estos servicios permiten compartir datos sensibles que solo pueden visualizarse una vez y que
posteriormente se eliminan de forma automática, garantizando la integridad y confidencialidad
de la información.

```bash
**server**
**key**
**token**
```

* **idCompania:** `6207` es un identificador del **middleware**
* Validar **ID_COMPAÑIA** en la sección *Datos estáticos* para el parámetro **IdCia**
* Validar **ID_BODEGA** en la sección *Datos estáticos* para el parámetro **IdBodega**
* Validar **ID_LISTA_PRECIO** en la sección *Datos estáticos* para el parámetro **IdPrecio**

---

## ⚙️ Endpoint: **ITEMPRECIOSPOS**
```bash
https://SERVER/v3/ejecutarconsulta?idCompania=6207&descripcion=ITEMPRECIOSPOS&parametros=IdCia={IdCia}|IdBodega={IdBodega}|IdPrecio={IdPrecio}
```

## 🧾 Request Headers
```bash
Key: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
Token: WSXWSXWSXWSXWSXWSXWSXWSXWSXWS
```

## 🔍 Query Parameters
```bash
idCompania: 6207
descripcion: ITEMPRECIOSPOS
parametros: IdCia={IdCia}|IdBodega={IdBodega}|IdPrecio={IdPrecio}
```

## 💻 Ejemplo Query Parameters
```bash
FechaInicio=20241201
FechaFin=20250101
IdCia=1
```

## 🔓 Curl
```bash
curl -X 'GET' \
  'http://SERVER/v3/EjecutarConsulta??idCompania=6207&descripcion=TERCEROS&parametros=FechaInicio%3D20241201%7CFechaFin%3D20250101%7CIdCia%3D1' \
  -H 'accept: */*' \
  -H 'Key: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX' \
  -H 'Token: WSXWSXWSXWSXWSXWSXWSXWSXWSXWS'
```

## ✅ Ejemplo de respuesta 200 OK

```json
{
  "codigo": 0,
  "mensaje": "transacción exitosa",
  "detalle": {
    "Table": [
      {
        "ID": "1234567        ",
        "TipoID": "C",
        "Nombre": "LUIS EDUARDO",
        "Apellidos": "PAEZ MARTINEZ",
        "RazonSocial": "PAEZ MARTINEZ LUIS EDUARDO",
        "Estado": "Activo",
        "Sucursal": "001 - PAEZ MARTINEZ LUIS EDUARDO",
        "CondicionPago": "CON - CONTADO",
        "Cupo": 0,
        "Cliente": "Si",
        "Proveedor": "No",
        "correo": "",
        "FechaCrecion": "20241213"
      },
      {
        "ID": "860098098",
        "TipoID": "N",
        "Nombre": "",
        "Apellidos": "",
        "RazonSocial": "JOSE BENJUMEA G. Y CIA LTDA",
        "Estado": "Activo",
        "Sucursal": "001 - JOSE BENJUMEA G. Y CIA LTDA",
        "CondicionPago": "CON - CONTADO",
        "Cupo": 0,
        "Cliente": "Si",
        "Proveedor": "No",
        "correo": "jose_benjumeag@yahoo.es",
        "FechaCrecion": "20241228"
      }
  }
}
```

## ⚠️ Ejemplo de error 400 Bad Request
```bash
{
  "status": 400,
  "mensaje": "Parámetros inválidos o faltantes: FechaInicio,FechaFin,IdCia"
}
```
---

**Explicacion** Response body:
```json
{
 "f_item": 112841, CODIGO ITEM
 "f_codigo_barra_principal": "7702155409211", CODIGO BARRAS
 "f_desc_item": "AMBIENTADOR SHICK GEL SENCILLO 80 GRS",
 "f_desc_corta": "AMBIENTADOR SHICK GE",
 "f_um": "UND ", UNIDAD MEDIDA
 "f_bodega": "TEX03",
 "f_desc_bodega": "BOD TEXANA, TIENDA",
 "f_ext_detalle_1": "520", CODIGO EXTENSION
 "f_desc_ext_detalle_1": "MANZACANE", NOMBRE EXTENSION
 "f_cant_existencia_actual": 25, EXISTENCIA KARDEX
 "f_precio_unit": 12000, PRECIO BRUTO
 "f_impto1": 19, VALOR IMPUESTO IVA
 "f_impto2": 0, VALOR IMPUESTO CONSUMO
 "f_impto4": 0, VALOR OTRO
 "f_impto3": 0, VALOR OTRO
 "f_tipo_inv": "IN3502E ", TIPO INVENTARIO
 "f_rowid_item": 8864, PKINTERNOS
 "f_rowid_item_ext": 13990, PKINTERNOS
 "f_01_GRP": "PRODUCTOS AUTOMOTRICES GRUPO PRODUCTO ",
 "f_01_LIN": "TBAS" LINEA PRODUCTO
 }
 ```