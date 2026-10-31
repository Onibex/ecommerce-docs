<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Part of the Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->

[English](../../../en/technical-documents/07-reference/01-sap-object-list.md) · **Español** | [↑ Índice de documentos técnicos](../README.md) | [README del repositorio](../../../README.md)

# Especificación completa de la lista de objetos de SAP

> **Fuente:** versión en español del artículo “15. Complete SAP Object List Specification” del Help Center de Onibex — <https://help.onibex.com/portal/en/kb/articles/complete-sap-object-list-specification>; redacción tomada del capítulo D.5 de la especificación funcional “D1 – Integración de sistemas”.

En las secciones anteriores de esta serie sobre integración de sistemas, ya se definieron los IDocs de una manera enunciativa mas no limitativa. En este artículo se definen las listas de mensajes, programas, funciones, *web services* y, en general, todas las mejoras en el código estándar de SAP, ahora sí de manera limitativa para la completa integración del sistema SAP con el sistema de E-Commerce.

## Lista de Customer Exits, User Exits, BADIS y Enhancements

**CMOD PR**

| OBJECT | OBJ_NAME | COMENTARIOS |
| --- | --- | --- |
| CMOD | ZONPR_ED | Proyecto de Exits para EDI |
| CMOD | ZONPR_ED | Exits de IDocs |
| CMOD | ZVSV0001 | Exits de IDocs |

**BADIS, ENHANCEMENTS Y USER EXITS**

| OBJECT | OBJ_NAME | COMENTARIOS |
| --- | --- | --- |
| Badi | ZONCL_IM_ECOM_SAVE_COND | Llena tabla Z para deltas de precios |
| Badi | ZONCL_IM_IDOC_CREA_CHCK | Filtrado de IDocs |
| ENHO | ZONEI_ONIBEX_IDOC_STS | Enhancement para enviar estatus de IDocs |
| ENHO | ZONEI_CREATE_ADRRMAS | Crear ADRMAS para SHIP_TO |
| ENHO | ZONEI_ONIBEX_IDOC_STS | Notificación de IDOCS en ERROR función IDOC_START_INBOUND |
| ENHO | ZONEI_ONIBEX_IDOC_STS2 | Notificación de IDOCS en ERROR función IDOC_START_INBOUND |
| Prog | ZXVEDU13 | User Exit EDI /ALE |
| Prog | ZXVEDU03 | User Exit EDI /ALE |
| Prog | ZXVEDU06 | User Exit EDI /ALE |
| Prog | ZXVEDU15 | User Exit EDI /ALE |
| Prog | ZXVSVU01 | User Exit EDI /ALE |

## Lista de Web Services

**WEB SERVICES**

| OBJECT | OBJ_NAME | COMENTARIOS |
| --- | --- | --- |
| Ws | ZONIF_IDOC_XML | Web Service Class IDOC Execution |
| Control | ZONCL_IDOC_XML_REQUEST | Web Service Class IDOC Execution |
| SICF | ZONIF_IDOC_XML EEPI2GLFNOLHN7IW9R54I61RZ | Web Service Class IDOC Execution |
| Function | ZIDOC_INBOUND_XML_VIA_HTTP | Función Z de Preparación de IDOCS |
| Ws | ZONIF_INV_PRICE | Web Service Class Inventory /Price |
| Control | ZONCL_MAT_INV_PRE_JSON | Web Service Class Inventory /Price |
| SICF | ZONIF_INV_PRICE00O2TGK59XU8QTY64A7YAAVON | Web Service Class Inventory /Price |
| Function | ZONFM_INV_PRICE | Función de Cálculo de Inventario Disponible |

## Lista de Programas

**PROGRAMAS**

| OBJECT | OBJ_NAME | COMENTARIOS |
| --- | --- | --- |
| Prog | ZONRE_ACC_STS_IDOC | Estado de Cuenta (IDoc) |
| Prog | ZONIN_ACC_STS_IDOC_TOP | Estado de Cuenta (IDoc) |
| Prog | ZONIN_ACC_STS_IDOC_FO1 | Estado de Cuenta (IDoc) |
| Prog | ZONRE_ATS | Inventario Disponible (IDoc) |
| Prog | ZONIN_ATS_TOP | Inventario Disponible (IDoc) |
| Prog | ZONIN_ATS_F01 | Inventario Disponible (IDoc) |
| Prog | ZONRE_CUST_MAT_PRICE | Precios por Cliente Material (IDoc) |
| Prog | ZONI_CUST_MAT_PRICE_TOP | Precios por Cliente Material (IDoc) |
| Prog | ZONI_CUST_MAT_PRICE_F01 | Precios por Cliente Material (IDoc) |
| Prog | ZONRE_CUST_MAT_PRICE2 | Precios por Cliente Material (IDoc) |
| Prog | ZONIN_CUST_MAT_PRICE2_TOP | Precios por Cliente Material (IDoc) |
| Prog | ZONIN_CUST_MAT_PRICE2_F01 | Precios por Cliente Material (IDoc) |
| Prog | ZONRE_CUSTOMER_CHKPNT_UPD | Update de Clientes (IDoc) |
| Prog | ZONIN_CUSTOMER_CHKPNT_UPD_TOP | Update de Clientes (IDoc) |
| Prog | ZONIN_CUSTOMER_CHKPNT_UPD_F01 | Update de Clientes (IDoc) |
| Prog | ZONRE_IDOC_CREDIT_RELEASE | Pedidos Notificación de Liberación de Crédito (IDoc) |
| Prog | ZONRE_IDOC_PURGE | Borrar IDocs (IDoc) |
| Prog | ZONRE_IDOCS_SO_LOG | Log de Ejecución de IDocs |
| Prog | ZONIN_IDOCS_SO_LOG_TOP | Log de Ejecución de IDocs |
| Prog | ZONIN_IDOCS_SO_LOG_F01 | Log de Ejecución de IDocs |
| Prog | ZONRE_INVENTORY_SALES | Inventario Disponible Diario (IDoc) |
| Prog | ZONIN_INVENTORY_SALES_TOP | Inventario Disponible Diario (IDoc) |
| Prog | ZONIN_INVENTORY_SALES_F01 | Inventario Disponible Diario (IDoc) |
| Prog | ZONRE_MAT_CLASSS_UPDATE | Material Class (IDoc) |
| Prog | ZONIN_MAT_CLASSS_UPDATE_TOP | Material Class (IDoc) |
| Prog | ZONIN_MAT_CLASSS_UPDATE_F01 | Material Class (IDoc) |
| Prog | ZONRE_MAT_REF_IDOC | Reporte de Materiales Referenciados (IDoc) |
| Prog | ZONIN_MAT_REF_IDOC_TOP | Reporte de Materiales Referenciados (IDoc) |
| Prog | ZONIN_MAT_REF_IDOC_F01 | Reporte de Materiales Referenciados (IDoc) |
| Prog | ZONRE_MATERIAL_CHKPNT_UPD | Update de Materiales (IDoc) |
| Prog | ZONIN_MATERIAL_CHKPNT_UPD_TOP | Update de Materiales (IDoc) |
| Prog | ZONIN_MATERIAL_CHKPNT_UPD_F01 | Update de Materiales (IDoc) |
| Prog | ZONRE_ONI_SO_EXPORT | Exportar Historial de Órdenes, Entregas y Facturas (IDoc) |
| Prog | ZONIN_ONI_SO_EXPORT_TOP | Exportar Historial de Órdenes, Entregas y Facturas (IDoc) |
| Prog | ZONIN_ONI_SO_EXPORT_F01 | Exportar Historial de Órdenes, Entregas y Facturas (IDoc) |
| Prog | ZONRE_RBDSEDEB | IDoc DEBMAS |
| Prog | ZONIN_MBDCONST | IDoc DEBMAS |
| Prog | ZONIN_MBDSUBPS | IDoc DEBMAS |
| Prog | ZONIN_RBDAUTHI | IDoc DEBMAS |
| Prog | ZONRE_RFITEMAR | Export de Partidas Abiertas por Deudor para Edo. de Cuenta |

## Lista de Funciones

**GRUPOS DE FUNCIONES**

| OBJECT | OBJ_NAME | COMENTARIOS |
| --- | --- | --- |
| FUGR | ZONFG_EDI | Funciones para adjuntar IDocs complementarios al DEBMAS |
| FUGR | ZONFG_EDIN | Funciones para IDOCS |
| FUGR | ZONFG_ONIBEX | Funciones para obtener Inventario y precios |
| Func | ZONFM_SPLIT_ITEMS | Función para obtener Viajes por camión en la Toma de Pedidos |

## Lista de IDocs

**IDOCS**

| OBJECT | OBJ_NAME | COMENTARIOS |
| --- | --- | --- |
| Types | ZON_MREF | Materiales Referenciados |
| Segment | ZON_MRF | Segmento de IDoc |
| Types | Z846IDOC_PRICE | Precios por Cliente |
| Segment | Z1846CU_PRICE | Estructuras de IDocs |
| Segment | Z1846DT_PRICE | Estructuras de IDocs |
| Types | ZON_ATS | Inventario Disponible |
| SEGMENT3 | ZON_ATS | Estructuras de IDocs |
| Segment | ZONSG_ATS | Estructuras de IDocs |
| Types | ZON_STS | Status de Ejecución de IDocs |
| Segment | ZON_STS | Estructuras de IDocs |
| Types | ZONACCSTS | Estado de Cuenta Clientes |
| Segment | ZON_ACCSTS | Estructuras de IDocs |
| Segment | ZON_OPEITM | Estructuras de IDocs |

## Diccionario de estructuras y tablas

**DICCIONARIO**

| OBJECT | OBJ_NAME | COMENTARIOS |
| --- | --- | --- |
| TABD | ZONST_INV_RES | Estructura |
| TABD | ZONST_MAT_INV_IN | Estructura |
| TABL | ZONST_MAT_REF | Estructura |
| TABL | ZONST_VBEP | Estructura |
| TABL | ZONST_XKOMV | Estructura |
| TABL | ZALSMEX_TABLINE | Estructura |
| TABL | ZESD_PORTALVTAS_PRECIOS_INV | Estructura |
| TABL | ZJSON_KEY_VALUE | Estructura |
| TABL | ZONST_846_MATNR | Estructura |
| TABL | ZONST_846_STK | Estructura |
| TABL | ZONST_856_ORD | Estructura |
| TABL | ZONST_INV_ENTRY | Estructura |
| TABL | ZONST_INV_RES | Estructura |
| TABL | ZONST_MATPLANT | Estructura |
| TABL | ZONST_MAT_INV_DETAIL | Estructura |
| TABL | ZONST_MAT_INV_IN | Estructura |
| TABL | ZONST_PORTALVTAS_CLIENTES | Estructura |
| TABL | ZONST_PORTALVTAS_LEERCATALOGO | Estructura |
| TABL | ZONST_PORTALVTAS_PRECIOS_DTL | Estructura |
| TABL | ZONST_PORTALVTAS_PRECIOS_HDR | Estructura |
| TABL | ZONST_PORTALVTAS_PRECIOS_INV | Estructura |
| TABL | ZONST_PORTALVTAS_PRECIOS_PRECI | Estructura |
| TABL | ZONST_PRICE_REPORT | Estructura |
| TABL | ZST_UDCRANGE | Estructura |
| TABD | ZONST_INV_ENTRY | Estructura |
| TABL | ZONTA_PRICE_INFR | Tabla |
| TTYP | ZONTT_MAT_REF | Tipo Tabla |
| TTYP | ZONTT_VBEP | Tipo Tabla |
| TTYP | ZONTT_XKOMV | Tipo Tabla |
| TTYP | ZJSON_KEY_VALUE_T | Tipo Tabla |
| TTYP | ZONTT_846_MATNR | Tipo Tabla |
| TTYP | ZONTT_846_STK | Tipo Tabla |
| TTYP | ZONTT_856_ORD | Tipo Tabla |
| TTYP | ZONTT_INV_RES | Tipo Tabla |
| TTYP | ZONTT_MATPLANT | Tipo Tabla |
| TTYP | ZONTT_MAT_INV_DETAIL | Tipo Tabla |
| TTYP | ZONTT_MAT_INV_IN | Tipo Tabla |
| TTYP | ZONTT_PORTALVTAS_PRECIOS_INV | Tipo Tabla |
| TTYP | ZONTT_PORTALVTAS_PRECIOS_PRECI | Tipo Tabla |
| TTYP | ZONTT_PRICE_REPORT | Tipo Tabla |
| TTYP | ZTY_UDCRANGE | Tipo Tabla |

← Anterior: [Configuración de materiales alternativos: cross-selling y up-selling](../06-sales-configuration/02-cross-selling-up-selling.md)

---

© 2026 Onibex, LLC · Licenciado bajo [CC BY-NC-ND 4.0](../../../LICENSE) (SPDX: CC-BY-NC-ND-4.0) · [Licencia comercial](../../../COMMERCIAL-LICENSE.md) · [Marcas y avisos de terceros](../../../THIRD-PARTY-NOTICES.md) · SAP y los demás productos y servicios SAP mencionados son marcas comerciales o marcas registradas de SAP SE o de una empresa afiliada a SAP en Alemania y otros países; los nombres se usan solo con fines de identificación.
