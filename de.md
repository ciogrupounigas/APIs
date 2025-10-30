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

## 🏨 BODEGAS POS - CANASTILLA

*COMBUSTIBLES UNIGAS SAS*

| **ID_BODEGA** | **Descripción**                     | **ID_CO** |
|----------------|-------------------------------------|------------|
| 3 | BOD ESTANCIA, TIENDA | 002 |
| 8 | BOD TEXANA, TIENDA | 003 |
| 38 | BOD MONTEARROYO TIENDA | 015 |
| 43 | BOD LA GRAN AVENIDA, TIENDA | 016 |
| 53 | BOD NUEVA DIANA, TIENDA | 018 |
| 78 | BOD COTA, TIENDA | 019 |


> **Aplica en el parámetro:** `IdBodega` Endpoint **ITEMPRECIOSPOS**

*AUTOMOTORES REINA SAS*

| **ID_BODEGA** | **Descripción** | **ID_CO** |
|----------------|-------------------------------------|------------|
| 83 | BOD REINA  TIENDA | 001 |

> **Aplica en el parámetro:** `IdBodega` Endpoint **ITEMPRECIOSPOS**
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
| 0190005 | GNV |

> **Aplica para los campos:** `f470_id_item`
---


## 🎏 Lista de precios

*COMBUSTIBLES UNIGAS SAS*

| **ID_LISTA_PRECIO** | **Descripción lista precio** |
|------------|-------------------------------------|
| 002 | LP EDS ESTANCIA |
| 003 | LP EDS TEXANA |
| 010 | LP EDS REINA (GNV) |
| 011 | LP EDS LA AVENIDA |
| 013 | LP EDS TERMINAL |
| 015 | LP EDS MONTEARROYO |
| 016 | LP EDS LA GRAN AVENIDA |
| 018 | LP EDS NUEVA DIANA |
| 019 | LP EDS COTA |
| 022 | LP EDS TRANSUNIDOS |

> **Aplica para los campos:** `f470_id_lista_precio`

*AUTOMOTORES REINA SAS*

| **ID_LISTA_PRECIO** | **Descripción lista precio** |
|------------|-------------------------------------|
| 001 | LP AUTOMOTORES REINA |

> **Aplica para los campos:** `f470_id_lista_precio` 
---


## 💳 Medios de pago

| **ID_MEDIOS_PAGO** | **Descripción Tipo** |
|------------|-------------------------------------|
| EFE | Efectivo |
| TD | Tarjeta | 

> **Aplica para los campos:** `F358_ID_MEDIOS_PAGO`
---


## 👲 Tipo cliente factura

| **ID_TIPO_CLI_FACT** | **Descripción** |
|------------|-------------------------------------|
| 100 | COMERCIALES LIQUIDOS |
| 101 | COMERCIALES GNV |

> **Aplica para los campos:** `f461_id_tipo_cli_fact`, `f460_id_tipo_cli_fact`
---


## 📧 Tipo de documentos

| **ID_TIPO_DOCTO** | **Descripción** |
|------------|-------------------------------------|
| FE1 | FACTURA ELECTRONICA |
| RM | REMISION |
| VD | VENTAS DIAN |
| VC | VENTA CONTADO |
| VDP | VENTAS DIAN POS - CANASTILLA |

> **Aplica para los campos:**  `F350_ID_TIPO_DOCTO`, `f470_id_tipo_docto`, `f471_id_tipo_docto`
---


## 📮 Tipo sucursales cliente

*COMBUSTIBLES UNIGAS SAS*

| **ID_SUCURSAL_FACT** | **Descripción** |
|------------|-------------------------------------|
| 001 | PRUEBAS INTEGRACION |
| 101 | PUENTE ARANDA |
| 102 | EDS ESTANCIA |
| 103 | EDS TEXANA |
| 110 | EDS REINA |
| 111 | EDS AVENIDA |
| 113 | EDS TERMINAL |
| 115 | EDS MONTEARROYO |
| 116 | EDS LA GRAN AVENIDA |
| 118 | EDS NUEVA DIANA |
| 119 | EDS COTA |
| 121 | EDS TRANSUNIDOS |
| 125 | EDS PEGASO |

> **Aplica para los campos:** `F201_ID_SUCURSAL`, `F_ID_SUCURSAL`, `Id_Sucursal`,
`f461_id_sucursal_fact`, `f461_id_sucursal_rem`, `f460_id_sucursal_fact`,
`f460_id_sucursal_rem`

*AUTOMOTORES REINA SAS*

| **ID_SUCURSAL_FACT** | **Descripción** |
|------------|-------------------------------------|
| 001 | EDS REINA |


> **Aplica para los campos:** `F201_ID_SUCURSAL`, `F_ID_SUCURSAL`, `Id_Sucursal`,
`f461_id_sucursal_fact`, `f461_id_sucursal_rem`, `f460_id_sucursal_fact`,
`f460_id_sucursal_rem`
---


## 📲 Unidades de medida

| **ID_UNIDAD_MEDIDA** | **Descripción** |
|------------|-------------------------------------|
| CAJ | CAJA |   
| CAN | CANECA  |
| CUA | CUARTO |
| GAL | GALON |
| GLA | GALON ACEITES |
| GLC | GALON COMBUSTIBLES |
| GRA | GRANEL |
| GRS | GRAMO |
| KGS | KILOGRAMOS |
| LIBR | LIBRA |
| LTS | LITROS |
| MLS | MILILITRO |
| MT3 | METROS CUBICOS |
| ONZ | ONZA |
| PAQ | PAQUETE |
| PIN | PINTA |
| TAM | TAMBOR |
| UN | UNIDAD |
| UND | UNIDADES |
| UNI | UNIDAD |

> **Aplica para los campos:** `f470_id_unidad_medida`
---


## 💰 Unidades de negocio

| **ID_UN** | **Descripción de Unidad de negocio** |
|------------|-------------------------------------|
| 02 | LIQUIDOS        |
| 03 | GNV |
| 05 | TIENDA |
| 06 | ARRENDAMIENTOS |

> **Aplica para los campos:** `f470_id_un_movto`
---
© 2025 - Departamento TIC - Combustibles Unigas SAS