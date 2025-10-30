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
* Validar **ID_BODEGAPOS** en la sección *Datos estáticos* para el parámetro **IdBodega**
* Validar **ID_LISTA_PRECIO** en la sección *Datos estáticos* para el parámetro **IdPrecio**
**FALTA AGREGAR TABLA BODEGAPOS DATOS ESTATICOS SQL VERIFICAR PROCEDIMIENTO ALMACENADO**
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
IdCia=1
IdBodega=8
IdPrecio=003
```

## 🔓 Curl
```bash
curl -X 'GET' \
  'http://SERVER/v3/EjecutarConsulta?idCompania=6207&descripcion=ITEMPRECIOSPOS&parametros=IdCia%3D1%7CIdBodega%3D8%7CIdPrecio%3D003' \
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
        "f_item": 13054,
        "f_codigo_barra_principal": "7705955103044",
        "f_desc_item": "ACEITE MOBIL SPECIAL HD 50 1/4-946ml",
        "f_desc_corta": "MOBIL  HD 50 1/4",
        "f_um": "CUA ",
        "f_bodega": "TEX03",
        "f_desc_bodega": "BOD TEXANA, TIENDA",
        "f_ext_detalle_1": null,
        "f_desc_ext_detalle_1": null,
        "f_cant_existencia_actual": 16,
        "f_precio_unit": 26000,
        "f_impto1": 0,
        "f_impto2": 0,
        "f_impto4": 0,
        "f_impto3": 0,
        "f_tipo_inv": "IN3502    ",
        "f_fecha_actualizacion": "2018-12-06T14:51:27",
        "f_rowid_item": 78,
        "f_rowid_item_ext": 79,
        "f_01_GRP": "PRODUCTOS AUTOMOTRICES                  ",
        "f_01_LIN": "LUBRICANTES"
      },
      {
        "f_item": 112841,
        "f_codigo_barra_principal": "7702155409211",
        "f_desc_item": "AMBIENTADOR SHICK GEL SENCILLO 80 GRS",
        "f_desc_corta": "AMBIENTADOR SHICK GE",
        "f_um": "UND ",
        "f_bodega": "TEX03",
        "f_desc_bodega": "BOD TEXANA, TIENDA",
        "f_ext_detalle_1": "520",
        "f_desc_ext_detalle_1": "MANZACANE",
        "f_cant_existencia_actual": 120,
        "f_precio_unit": 12000,
        "f_impto1": 19,
        "f_impto2": 0,
        "f_impto4": 0,
        "f_impto3": 0,
        "f_tipo_inv": "IN3502E   ",
        "f_fecha_actualizacion": "2019-07-25T10:51:55",
        "f_rowid_item": 8864,
        "f_rowid_item_ext": 13990,
        "f_01_GRP": "PRODUCTOS AUTOMOTRICES                  ",
        "f_01_LIN": "TBAS"
      }
    ],
    "Table1": [
      {
        "tipo": 5,
        "cri1": "IVA",
        "cri2": "ICONS",
        "cri3": "INCP",
        "cri4": "INC",
        "cri5": "",
        "cri6": ""
      }
    ]
  }
}
```

## ⚠️ Ejemplo de error 400 Bad Request
```bash
{
  "status": 400,
  "mensaje": "Parámetros inválidos o faltantes: IdCia, IdBodega, IdPrecio"
}
```
---

## 🔮 **Explicación** Response body:
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