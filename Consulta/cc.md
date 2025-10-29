## ⚙️ Endpoint: **CENTROSDECOSTOS**

```bash
https://SERVER/v3/ejecutarconsulta?idCompania=6207&descripcion=CENTROSDECOSTOS&parametros=IdCC={IdBodega}|IdCia={IdCia}
```

## 🔍 Query Params
```bash
idCompania: 6207
descripcion: CENTROSDECOSTOS
parametros: IdBodega={IdCC}|IdCia={IdCia}
```

## 💻 Ejemplo
Centro de costos TIC : 233
Compañia : 1

## Curl
```bash
curl -X 'GET' \
  'http://SERVER/v3/EjecutarConsulta?idCompania=6207&descripcion=CENTROSDECOSTOS&parametros=IdCC%3D233%7CIdCia%3D1' \
  -H 'accept: */*' \
  -H 'Key: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX' \
  -H 'Token: WSXWSXWSXWSXWSXWSXWSXWSXWSXWS'
```

## ✅ Ejemplo de respuesta 200 OK
```bash
{
  "codigo": 0,
  "mensaje": "transacción exitosa",
  "detalle": {
    "Table": [
      {
        "IdCC": "233",
        "Descripcion": "TIC"
      }
    ]
  }
```

## ⚠️ Ejemplo de error 400 Bad Request
```bash
{
  "status": 400,
  "mensaje": "Parámetros inválidos o faltantes: IdCC o IdCia"
}
```
---