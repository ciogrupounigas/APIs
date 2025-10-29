# 🏗️ BODEGAS COMBUSTIBLES UNIGAS SAS

| **ID_BODEGA** | **Descripción**                     | **ID_CO** |
|----------------|-------------------------------------|------------|
| EST01 | BOD ESTANCIA GNV | 002 |
| EST02 | BOD ESTANCIA, LIQUIDOS | 002 |
| EST03 | BOD ESTANCIA, TIENDA | 002 |
| TEX01 | BOD TEXANA GNV | 003 |
| TEX02 | BOD TEXANA, LIQUIDOS | 003 |
| TEX03 | BOD TEXANA, TIENDA | 003 |
| REI01 | BOD REINA GNV | 010 |
| AVE01 | BOD AVENIDA GNV | 011 |
| TER01 | BOD TERMINAL, GNV | 013 |
| MON01 | BOD MONTEARROYO, GNV | 015 |
| MON02 | BOD MONTEARROYO LIQUIDOS | 015 |
| MON03 | BOD MONTEARROYO TIENDA | 015 |
| GRA02 | BOD LA GRAN AVENIDA, LIQUIDOS | 016 |
| GRA03 | BOD LA GRAN AVENIDA, TIENDA | 016 |
| DIA01 | BOD NUEVA DIANA, GNV | 018 |
| DIA02 | BOD NUEVA DIANA, LIQUIDOS | 018 |
| DIA03 | BOD NUEVA DIANA, TIENDA | 018 |
| COT02 | BOD COTA, LIQUIDOS | 019 |
| COT03 | BOD COTA, TIENDA | 019 |
| TRA01 | BOD TRANSUNIDOS GNV | 021 |
| PEG01 | BOD PEGASO GNV | 022 |

> **Aplica para los campos:** `f470_id_bodega`

---

## ⚙️ Endpoint: **BODEGAS**

```bash
https://SERVER/v3/ejecutarconsulta?idCompania=6207&descripcion=BODEGAS&parametros=IdBodega={IdBodega}|IdCia={IdCia}
```

## 🧾 Request Headers
```bash
Key: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
Token: WSXWSXWSXWSXWSXWSXWSXWSXWSXWS
```

## 🔍 Query Params
```bash
idCompania: 6207
descripcion: BODEGAS
parametros: IdBodega={IdBodega}|IdCia={IdCia}
```

## ✅ Ejemplo de respuesta 200 OK
```bash
{
  "status": 200,
  "mensaje": "Consulta ejecutada correctamente",
  "data": [
    {
      "IdBodega": "EST01",
      "Descripcion": "BOD ESTANCIA GNV",
      "IdCO": "002"
    }
  ]
}
```

## ⚠️ Ejemplo de error 400 Bad Request
```bash
{
  "status": 400,
  "mensaje": "Parámetros inválidos o faltantes: IdBodega o IdCia"
}
```
---

# 🏗️ BODEGAS AUTOMOTORES REINA SAS

BODEGAS
ID_BODEGA Descripción ID_CO
REI02 BOD REINA LIQUIDOS 001
REI03 BOD REINA TIENDA 001
> **Aplica para los campos:** `f470_id_bodega`