# 🏗️ CENTROS DE OPERACION

| **ID_CO** | **Descripción**                     | **API** |
|----------------|-------------------------------------|------------|
| 002 | EDS ESTANCIA | LIQUIDOS – GNV |
| 003 | EDS TEXANA | LIQUIDOS - GNV |
| 010 | EDS REINA | GNV |
| 011 | EDS AVENIDA | GNV |
| 013 | EDS TERMINAL | GNV |
| 015 | EDS MONTEARROYO | LIQUIDOS - GNV |
| 016 | EDS LA GRAN AVENIDA | LIQUIDOS |
| 018 | EDS NUEVA DIANA | LIQUIDOS - GNV |
| 019 | EDS COTA | LIQUIDOS |
| 021 | EDS TRANSUNIDOS | GNV |
| 025 | EDS PEGASO | GNV | 


## ⚙️ Endpoint: **CENTROSOPERACION**
```bash
https://SERVER/v3/ejecutarconsulta?idCompania=6207&descripcion=CENTROSOPERACION&parametros=IdCO={IdBodega}|IdCia={IdCia}
```

## 🔍 Query Params
```bash
idCompania: 6207
descripcion: CENTROSOPERACION
parametros: IdCO={IdCC}|IdCia={IdCia}
```

## 💻 Ejemplo
```bash
Centro de Operación TEXANA : 003
Compañia : 1
```

## Curl
```bash
curl -X 'GET' \
  'http://SERVER/v3/EjecutarConsulta?idCompania=6207&descripcion=CENTROSOPERACION&parametros=IdCO%3D003%7CIdCia%3D1 \
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
        "IdCO": "003",
        "Descripcion": "EDS TEXANA"
      }
    ]
  }
```

## ⚠️ Ejemplo de error 400 Bad Request
```bash
{
  "status": 400,
  "mensaje": "Parámetros inválidos o faltantes: IdCO o IdCia"
}
```
---