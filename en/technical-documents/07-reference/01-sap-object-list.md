<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Part of the Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->

**English** · [Español](../../../es/technical-documents/07-reference/01-sap-object-list.md) | [↑ Technical documents index](../README.md) | [Repository README](../../../README.md)

# Complete SAP object list specification

> **Source:** Onibex Help Center article “15. Complete SAP Object List Specification” — <https://help.onibex.com/portal/en/kb/articles/complete-sap-object-list-specification>. Spanish chapter D.5 of the functional specification “D1 – Integración de sistemas”.

In the previous sections of this systems integration series, IDocs were already defined in a more non-limiting explanatory manner. This article defines the lists of messages, programs, functions, web services, and in general all improvements to the SAP standard code, now in a limiting way for the complete integration of the SAP system with the E-Commerce system.

## List of Customer Exits, User Exits, BADIS and Enhancements

**CMOD PR**

| OBJECT | OBJ_NAME | COMMENTS |
| --- | --- | --- |
| CMOD | ZONPR_ED | Exits Project for EDI |
| CMOD | ZONPR_ED | IDOCS Exits |
| CMOD | ZVSV0001 | IDOCS Exits |

**BADIS, ENHANCEMENTS AND USER EXITS**

| OBJECT | OBJ_NAME | COMMENTS |
| --- | --- | --- |
| Badi | ZONCL_IM_ECOM_SAVE_COND | Fill out Z-table for price deltas |
| Badi | ZONCL_IM_IDOC_CREA_CHCK | IDOCS filtering |
| ENHO | ZONEI_ONIBEX_IDOC_STS | Enhancement to send IDOCS status |
| ENHO | ZONEI_CREATE_ADRRMAS | Create ADRMAS for SHIP_TO |
| ENHO | ZONEI_ONIBEX_IDOC_STS | IDOCS notification in ERROR, function IDOC_START_INBOUND |
| ENHO | ZONEI_ONIBEX_IDOC_STS2 | IDOCS notification in ERROR, function IDOC_START_INBOUND |
| Prog | ZXVEDU13 | User Exit EDI /ALE |
| Prog | ZXVEDU03 | User Exit EDI /ALE |
| Prog | ZXVEDU06 | User Exit EDI /ALE |
| Prog | ZXVEDU15 | User Exit EDI /ALE |
| Prog | ZXVSVU01 | User Exit EDI /ALE |

## Web Services List

**WEB SERVICES**

| OBJECT | OBJ_NAME | COMMENTS |
| --- | --- | --- |
| Ws | ZONIF_IDOC_XML | Web Service Class IDOC Execution |
| Control | ZONCL_IDOC_XML_REQUEST | Web Service Class IDOC Execution |
| SICF | ZONIF_IDOC_XML EEPI2GLFNOLHN7IW9R54I61RZ | Web Service Class IDOC Execution |
| Function | ZIDOC_INBOUND_XML_VIA_HTTP | IDOCS Preparation Z function |
| Ws | ZONIF_INV_PRICE | Web Service Class Inventory /Price |
| Control | ZONCL_MAT_INV_PRE_JSON | Web Service Class Inventory /Price |
| SICF | ZONIF_INV_PRICE00O2TGK59XU8QTY64A7YAAVON | Web Service Class Inventory /Price |
| Function | ZONFM_INV_PRICE | Available Inventory Calculation Function |

## Program List

**Programs**

| OBJECT | OBJ_NAME | COMMENTS |
| --- | --- | --- |
| Prog | ZONRE_ACC_STS_IDOC | Statement of Account (IDoc) |
| Prog | ZONIN_ACC_STS_IDOC_TOP | Statement of Account (IDoc) |
| Prog | ZONIN_ACC_STS_IDOC_FO1 | Statement of Account (IDoc) |
| Prog | ZONRE_ATS | Available Inventory (IDOC) |
| Prog | ZONIN_ATS_TOP | Available Inventory (IDOC) |
| Prog | ZONIN_ATS_F01 | Available Inventory (IDOC) |
| Prog | ZONRE_CUST_MAT_PRICE | Prices per Customer Material (IDOC) |
| Prog | ZONI_CUST_MAT_PRICE_TOP | Prices per Customer Material (IDOC) |
| Prog | ZONI_CUST_MAT_PRICE_F01 | Prices per Customer Material (IDOC) |
| Prog | ZONRE_CUST_MAT_PRICE2 | Prices per Customer Material (IDOC) |
| Prog | ZONIN_CUST_MAT_PRICE2_TOP | Prices per Customer Material (IDOC) |
| Prog | ZONIN_CUST_MAT_PRICE2_F01 | Prices per Customer Material (IDOC) |
| Prog | ZONRE_CUSTOMER_CHKPNT_UPD | Customer Update (IDOC) |
| Prog | ZONIN_CUSTOMER_CHKPNT_UPD_TOP | Customer Update (IDOC) |
| Prog | ZONIN_CUSTOMER_CHKPNT_UPD_F01 | Customer Update (IDOC) |
| Prog | ZONRE_IDOC_CREDIT_RELEASE | Credit Release Notification Orders (IDOC) |
| Prog | ZONRE_IDOC_PURGE | Delete IDOCS (IDOC) |
| Prog | ZONRE_IDOCS_SO_LOG | IDOCS Execution Log |
| Prog | ZONIN_IDOCS_SO_LOG_TOP | IDOCS Execution Log |
| Prog | ZONIN_IDOCS_SO_LOG_F01 | IDOCS Execution Log |
| Prog | ZONRE_INVENTORY_SALES | Daily Available Inventory (IDoc) |
| Prog | ZONIN_INVENTORY_SALES_TOP | Daily Available Inventory (IDoc) |
| Prog | ZONIN_INVENTORY_SALES_F01 | Daily Available Inventory (IDoc) |
| Prog | ZONRE_MAT_CLASSS_UPDATE | Material Class (IDOC) |
| Prog | ZONIN_MAT_CLASSS_UPDATE_TOP | Material Class (IDOC) |
| Prog | ZONIN_MAT_CLASSS_UPDATE_F01 | Material Class (IDOC) |
| Prog | ZONRE_MAT_REF_IDOC | Referenced Materials Report (IDoc) |
| Prog | ZONIN_MAT_REF_IDOC_TOP | Referenced Materials Report (IDoc) |
| Prog | ZONIN_MAT_REF_IDOC_F01 | Referenced Materials Report (IDoc) |
| Prog | ZONRE_MATERIAL_CHKPNT_UPD | Materials Update (IDOC) |
| Prog | ZONIN_MATERIAL_CHKPNT_UPD_TOP | Materials Update (IDOC) |
| Prog | ZONIN_MATERIAL_CHKPNT_UPD_F01 | Materials Update (IDOC) |
| Prog | ZONRE_ONI_SO_EXPORT | Export Order, Delivery and Invoice History (IDoc) |
| Prog | ZONIN_ONI_SO_EXPORT_TOP | Export Order, Delivery and Invoice History (IDoc) |
| Prog | ZONIN_ONI_SO_EXPORT_F01 | Export Order, Delivery and Invoice History (IDoc) |
| Prog | ZONRE_RBDSEDEB | IDOC DEBMAS |
| Prog | ZONIN_MBDCONST | IDOC DEBMAS |
| Prog | ZONIN_MBDSUBPS | IDOC DEBMAS |
| Prog | ZONIN_RBDAUTHI | IDOC DEBMAS |
| Prog | ZONRE_RFITEMAR | Export Open Items per Debtor for Account Statement |

## Function List

**FUNCTION GROUPS**

| OBJECT | OBJ_NAME | COMMENTS |
| --- | --- | --- |
| FUGR | ZONFG_EDI | Functions to attach complementary IDocs to DEBMAS |
| FUGR | ZONFG_EDIN | Functions for IDocs |
| FUGR | ZONFG_ONIBEX | Functions to get Inventory and Pricing |
| Func | ZONFM_SPLIT_ITEMS | Function to obtain Truck Trips in Ordering |

## List of IDocs

**IDOCS**

| OBJECT | OBJ_NAME | COMMENTS |
| --- | --- | --- |
| Types | ZON_MREF | Referenced Materials |
| Segment | ZON_MRF | IDoc segment |
| Types | Z846IDOC_PRICE | Prices per Customer |
| Segment | Z1846CU_PRICE | IDocs structures |
| Segment | Z1846DT_PRICE | IDocs structures |
| Types | ZON_ATS | Inventory Available |
| SEGMENT3 | ZON_ATS | IDocs structures |
| Segment | ZONSG_ATS | IDocs structures |
| Types | ZON_STS | IDocs Execution Status |
| Segment | ZON_STS | IDocs structures |
| Types | ZONACCSTS | Customer Statement |
| Segment | ZON_ACCSTS | IDocs structures |
| Segment | ZON_OPEITM | IDocs structures |

## Dictionary of structures and tables

**Dictionary**

| OBJECT | OBJ_NAME | COMMENTS |
| --- | --- | --- |
| TABD | ZONST_INV_RES | Structure |
| TABD | ZONST_MAT_INV_IN | Structure |
| TABL | ZONST_MAT_REF | Structure |
| TABL | ZONST_VBEP | Structure |
| TABL | ZONST_XKOMV | Structure |
| TABL | ZALSMEX_TABLINE | Structure |
| TABL | ZESD_PORTALVTAS_PRECIOS_INV | Structure |
| TABL | ZJSON_KEY_VALUE | Structure |
| TABL | ZONST_846_MATNR | Structure |
| TABL | ZONST_846_STK | Structure |
| TABL | ZONST_856_ORD | Structure |
| TABL | ZONST_INV_ENTRY | Structure |
| TABL | ZONST_INV_RES | Structure |
| TABL | ZONST_MATPLANT | Structure |
| TABL | ZONST_MAT_INV_DETAIL | Structure |
| TABL | ZONST_MAT_INV_IN | Structure |
| TABL | ZONST_PORTALVTAS_CLIENTES | Structure |
| TABL | ZONST_PORTALVTAS_LEERCATALOGO | Structure |
| TABL | ZONST_PORTALVTAS_PRECIOS_DTL | Structure |
| TABL | ZONST_PORTALVTAS_PRECIOS_HDR | Structure |
| TABL | ZONST_PORTALVTAS_PRECIOS_INV | Structure |
| TABL | ZONST_PORTALVTAS_PRECIOS_PRECI | Structure |
| TABL | ZONST_PRICE_REPORT | Structure |
| TABL | ZST_UDCRANGE | Structure |
| TABD | ZONST_INV_ENTRY | Structure |
| TABL | ZONTA_PRICE_INFR | Table |
| TTYP | ZONTT_MAT_REF | Table Type |
| TTYP | ZONTT_VBEP | Table Type |
| TTYP | ZONTT_XKOMV | Table Type |
| TTYP | ZJSON_KEY_VALUE_T | Table Type |
| TTYP | ZONTT_846_MATNR | Table Type |
| TTYP | ZONTT_846_STK | Table Type |
| TTYP | ZONTT_856_ORD | Table Type |
| TTYP | ZONTT_INV_RES | Table Type |
| TTYP | ZONTT_MATPLANT | Table Type |
| TTYP | ZONTT_MAT_INV_DETAIL | Table Type |
| TTYP | ZONTT_MAT_INV_IN | Table Type |
| TTYP | ZONTT_PORTALVTAS_PRECIOS_INV | Table Type |
| TTYP | ZONTT_PORTALVTAS_PRECIOS_PRECI | Table Type |
| TTYP | ZONTT_PRICE_REPORT | Table Type |
| TTYP | ZTY_UDCRANGE | Table Type |

← Previous: [Cross-selling and up-selling configuration (alternative materials)](../06-sales-configuration/02-cross-selling-up-selling.md)

---

© 2026 Onibex, LLC · Licensed under [CC BY-NC-ND 4.0](../../../LICENSE) (SPDX: CC-BY-NC-ND-4.0) · [Commercial license](../../../COMMERCIAL-LICENSE.md) · [Trademarks and third-party notices](../../../THIRD-PARTY-NOTICES.md) · SAP and other SAP products and services mentioned herein are trademarks or registered trademarks of SAP SE or an SAP affiliate company in Germany and other countries; names are used for identification only.
