![GET](https://img.shields.io/badge/v3/EjecutarConsulta-GET-brightgreen.svg)

## ⚙️ Endpoint: **CENTROSOPERACION**
```bash
https://SERVER/v3/ejecutarconsulta?idCompania=6207&descripcion=TERCEROS&parametros=FechaInicio={FechaInicio}|FechaFin={FechaFin}|IdCia={IdCia}
```

## 🧾 Request Headers
```bash
Key: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
Token: WSXWSXWSXWSXWSXWSXWSXWSXWSXWS
```

## 🔍 Query Params
```bash
idCompania: 6207
descripcion: CENTROSOPERACION
parametros: FechaInicio={FechaInicio}|FechaFin={FechaFin}|IdCia={IdCia}
```

## 💻 Ejemplo
```bash
FechaInicio=20241201
FechaFin=20250101
IdCia=1
```

## Curl
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
```

## ⚠️ Ejemplo de error 400 Bad Request
```bash
{
  "status": 400,
  "mensaje": "Parámetros inválidos o faltantes: FechaInicio,FechaFin,IdCia"
}
```
---