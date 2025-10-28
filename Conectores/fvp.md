## 🧾 Ejemplo: 1 productos 1 metodo de pago

```json
  {
    "Inicial": [
      {
        "F_CIA": "1"
      }
    ],
    "Doctoventascomercial": [
      {
        "F_CIA": "1",
        "F350_ID_CO": "003",
        "F350_ID_TIPO_DOCTO": "VDP",
        "F350_CONSEC_DOCTO": "3",
        "F350_FECHA": "20250901",
        "F350_ID_TERCERO": "222222222222",
        "f461_id_sucursal_fact": "003",
        "f461_id_tipo_cli_fact": "100",
        "f461_id_co_fact": "003",
        "f461_id_tercero_rem": "222222222222",
        "f461_id_sucursal_rem": "103",
        "f461_id_tercero_vendedor": "222222222222",
        "f461_referencia": "65498",
        "f461_id_punto_envio": "000"
      }
    ],
    "Movimientos": [
      {
        "F_CIA": "1",
        "f470_id_co": "003",
        "f470_id_tipo_docto": "VDP",
        "f470_consec_docto": "3",
        "f470_nro_registro": "1",
        "f470_id_bodega": "TEX03",
        "f470_id_co_movto": "003",
        "f470_id_lista_precio": "003",
        "f470_id_unidad_medida": "UND",
        "f470_cant_base": "1",
        "f470_vlr_bruto": "20000",
        "f470_notas": "",
        "f470_id_item": "105164",
        "f470_id_ext1_detalle": "165",
        "f470_id_un_movto": "05"
      }
    ],
    "Final": [
      {
        "F_CIA": "1"
      }
    ],
    "Caja": [
      {
        "F_CIA": "1",
        "F350_ID_CO": "003",
        "F350_ID_TIPO_DOCTO": "VDP",
        "F350_CONSEC_DOCTO": "3",
        "F358_ID_MEDIOS_PAGO": "TD",
        "F_VLR_MEDIO_PAGO": "20000",
        "F358_NRO_CUENTA": "0",
        "F358_COD_SEGURIDAD": "0",
        "F358_NRO_AUTORIZACION": "123456",
        "F358_FECHA_VCTO": "203001"
      }
    ]
  }
```

## 🧾 Ejemplo: 2 productos 1 metodo de pago

Item : 105164 Ext : 165
Item : 110210 sin extension

Extensión se interpreta como criterio de AROMA - SABOR, compartiendo el mismo codigo **"f470_id_item":** se diferencia por el codigo de barras

```json
{
    "Inicial": [
      {
        "F_CIA": "1"
      }
    ],
    "Doctoventascomercial": [
      {
        "F_CIA": "1",
        "F350_ID_CO": "003",
        "F350_ID_TIPO_DOCTO": "VDP",
        "F350_CONSEC_DOCTO": "4",
        "F350_FECHA": "20250901",
        "F350_ID_TERCERO": "222222222222",
        "f461_id_sucursal_fact": "003",
        "f461_id_tipo_cli_fact": "100",
        "f461_id_co_fact": "003",
        "f461_id_tercero_rem": "222222222222",
        "f461_id_sucursal_rem": "103",
        "f461_id_tercero_vendedor": "222222222222",
        "f461_referencia": "65498",
        "f461_id_punto_envio": "000"
      }
    ],
    "Movimientos": [
      {
        "F_CIA": "1",
        "f470_id_co": "003",
        "f470_id_tipo_docto": "VDP",
        "f470_consec_docto": "4",
        "f470_nro_registro": "1",
        "f470_id_bodega": "TEX03",
        "f470_id_co_movto": "003",
        "f470_id_lista_precio": "003",
        "f470_id_unidad_medida": "UND",
        "f470_cant_base": "1",
        "f470_vlr_bruto": "20000",
        "f470_notas": "",
        "f470_id_item": "105164",
        "f470_id_ext1_detalle": "165",
        "f470_id_un_movto": "05"
      },
      {
        "F_CIA": "1",
        "f470_id_co": "003",
        "f470_id_tipo_docto": "VDP",
        "f470_consec_docto": "4",
        "f470_nro_registro": "2",
        "f470_id_bodega": "TEX03",
        "f470_id_co_movto": "003",
        "f470_id_lista_precio": "003",
        "f470_id_unidad_medida": "CUA",
        "f470_cant_base": "1",
        "f470_vlr_bruto": "39000",
        "f470_notas": "",
        "f470_id_item": "110210",
        "f470_id_ext1_detalle": "",
        "f470_id_un_movto": "05"
      }
    ],
    "Final": [
      {
        "F_CIA": "1"
      }
    ],
    "Caja": [
      {
        "F_CIA": "1",
        "F350_ID_CO": "003",
        "F350_ID_TIPO_DOCTO": "VDP",
        "F350_CONSEC_DOCTO": "4",
        "F358_ID_MEDIOS_PAGO": "TD",
        "F_VLR_MEDIO_PAGO": "59000",
        "F358_NRO_CUENTA": "",
        "F358_COD_SEGURIDAD": "",
        "F358_NRO_AUTORIZACION": "",
        "F358_FECHA_VCTO": ""
      }
    ]
  }
```
