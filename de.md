## 🏗️ BODEGAS 

*COMBUSTIBLES UNIGAS SAS*

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

*AUTOMOTORES REINA SAS*

| **ID_BODEGA** | **Descripción** | **ID_CO** |
|----------------|-------------------------------------|------------|
| REI02 | BOD REINA  LIQUIDOS | 001 |
| REI03 | BOD REINA  TIENDA | 001 |

> **Aplica para los campos:** `f470_id_bodega`
---


## 🏣 Centros de Operación

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

> **Aplica para los campos:** `F350_ID_CO`, `f470_id_co`, `f470_id_co_movto`, `f461_id_co_fact`,
`f471_id_co`, `F201_ID_CO_FACTURA`
---


## 🏢 Compañias

| **ID_COMPAÑIA** | **NIT** | **Razón social** | **idInterface** |
|----------------|------------|-------------------------------------|------------|
| 1 | 830085008 | COMBUSTIBLES UNIGAS SAS | **1216** |
| 3 | 800041135 | AUTOMOTORES REINA SAS | **1236** |

> **Aplica en los campos:** `F_CIA, IdCia`
---


## 💵 Condiciones de pago

| **ID_CON_PAGO** | **Descripción** |
|------------|-------------------------------------|
| **CON** | CONTADO |
| 28D | CREDITO 28 DIAS |
| 10D | CREDITO A 10 DIAS |
| 12D | CREDITO A 12 DIAS |
| 14 | CREDITO A 14 DIAS |
| 15D | CREDITO A 15 DIAS |
| 20D | CREDITO A 20 DIAS |
| 23D | CREDITO A 23 DIAS |
| 30D | CREDITO A 30 DIAS |
| 45D | CREDITO A 45 DIAS |
| 5D | CREDITO A 5 DIAS |
| 8D | CREDITO A 8 DIAS |
| ANT | 100% ANTICIPADO |
| CUO | CUOTAS |

> **Aplica en los campos:** `f460_id_cond_pago`
---


## 💨 Items Operación EDS

| **ID_ITEM** | **Descripción del Item** |
|------------|-------------------------------------|
| 0190010 | A.C.P.M. | 
| 0190009 | GASOLINA CORRIENTE |
| 0190011 | GASOLINA EXTRA |
| 0190012 | MAX PRO |
| 0190005 | GNV 

> **Aplica para los campos:** `f470_id_item`
---


## 🎏 Lista de precios

---


## 💳 Medios de pago

---


## 👲 Tipo cliente factura

---


## 📧 Tipo de documentos

---


## 📮 Tipo sucursales cliente

---


## 📲 Unidades de medida

---


## 💰 Unidades de negocio
  - [Bodegas](Consulta/bd.md)
  - [Centros de operación](Consulta/co.md)
  - [Compañías](Consulta/cia.md)
  - [Condiciones de pago](Consulta/cp.md)
  - [Items](Consulta/item.md)
  - [Lista de Precios](Consulta/lp.md)
  - [Medios de Pago](Consulta/mp.md)
  - [Tipo cliente factura](Consulta/tcf.md)
  - [Tipo de documentos](Consulta/td.md)
  - [Tipo sucursales cliente](Consulta/tsc.md)
  - [Unidades de medida](Consulta/um.md)
  - [Unidades de negocio](Consulta/un.md)
