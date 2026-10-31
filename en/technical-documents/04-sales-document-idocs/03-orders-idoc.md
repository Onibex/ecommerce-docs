<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Part of the Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->

**English** · [Español](../../../es/technical-documents/04-sales-document-idocs/03-orders-idoc.md) | [↑ Technical documents index](../README.md) | [Repository README](../../../README.md)

# ORDERS IDoc configuration for sales orders

> **Source:** Onibex Help Center article “10. ORDERS iDOC configuration for Sales Orders” — <https://help.onibex.com/portal/en/kb/articles/orders-idoc-configuration-for-sales-orders>. Spanish chapter D.4.f of the functional specification “D1 – Integración de sistemas”.

ORDERS IDoc is used to create a Sales Order. This IDoc is sent as a message to the SAP system from the E-Commerce portal.

In SAP, the configuration of ORDERS IDoc begins in transaction **WE20**, on the Logical Systems part as an Inbound message, as described in the screen from Figure-87.

![SAP WE20 partner profile ECOMMERCE with inbound ORDERS selected](../../../assets/orders-idoc/orders-idoc-01.png)

**Figure-87** Setting up the Inbound ORDERS IDoc to receive Sales Orders from the E-Commerce portal in SAP.

When this entry is added, fill in the Inbound parameters as shown in Figure-88:

![SAP WE20 inbound ORDERS parameters with process code ORDE](../../../assets/orders-idoc/orders-idoc-02.png)

**Figure-88** Setting up the IDoc in WE20 for sales order message reception.

All other tabs from Figure-88 will remain empty.

The message that must be received before successfully creating this order is shown in the following example, or using WE02:

```
<?xml version="1.0" encoding="UTF-8"?>
<ORDERS05>

 <IDOC BEGIN="1">
  <EDI_DC40 SEGMENT="1">
   <TABNAM>EDI_DC40</TABNAM>
   <MANDT>800</MANDT>
   <DOCNUM>0000000025103215</DOCNUM>
   <DOCREL>740</DOCREL>
   <STATUS>30</STATUS>
   <DIRECT>1</DIRECT>
   <OUTMOD>2</OUTMOD>
   <IDOCTYP>ORDERS05</IDOCTYP>
   <MESTYP>ORDERS</MESTYP>
   <SNDPOR>SAPERP</SNDPOR>
   <SNDPRT>LS</SNDPRT>
   <SNDPRN>EH7CLNT800</SNDPRN>
   <RCVPOR>ECOMMERCE</RCVPOR>
   <RCVPRT>LS</RCVPRT>
   <RCVPRN>ECOMMERCE</RCVPRN>
   <CREDAT>20160901</CREDAT>
   <CRETIM>072024</CRETIM>
   <SERIAL>20160819072024</SERIAL>
  </EDI_DC40>

  <E1EDK01 SEGMENT="1">
   <ACTION>000</ACTION>
   <BELNR>25103000</BELNR>
   <CURCY>USD</CURCY>
   <ZTERM>Z030</ZTERM>
   <BSART>OR</BSART>
   <LIFSK>90</LIFSK>
  </E1EDK01>

  <E1EDK14 SEGMENT="1">
   <QUALF>012</QUALF>
   <ORGID>TA</ORGID>
  </E1EDK14>

   <E1EDK14 SEGMENT="1">
   <QUALF>005</QUALF>
   <ORGID>3800</ORGID>
  </E1EDK14>

<E1EDK14 SEGMENT="1">
   <QUALF>006</QUALF>
   <ORGID>00</ORGID>
  </E1EDK14>

  <E1EDK14 SEGMENT="1">
   <QUALF>007</QUALF>
   <ORGID>10</ORGID>
  </E1EDK14>

  <E1EDK14 SEGMENT="1">
   <QUALF>008</QUALF>
   <ORGID>3000</ORGID>
  </E1EDK14>

  <E1EDK03 SEGMENT="1">
   <IDDAT>002</IDDAT>
   <DATUM>20160913</DATUM>
  </E1EDK03>

  <E1EDKA1 SEGMENT="1">
   <PARVW>AG</PARVW>
   <PARTN>0000100016</PARTN>
   <NAME1>John Sample</NAME1>
   <STRAS>100 Sample Street</STRAS>
   <ORT01>Los Angeles</ORT01>
   <PSTLZ>92308</PSTLZ>
   <LAND1>US</LAND1>
   <REGIO>CA</REGIO>
   <PFORT>92308</PFORT>
  </E1EDKA1>

  <E1EDKA1 SEGMENT="1">
   <PARVW>RE</PARVW>
   <PARTN>0000100016</PARTN>
   <NAME1>John Sample</NAME1>
   <STRAS>100 Sample Street</STRAS>
   <ORT01>Los Angeles</ORT01>
   <PSTLZ>02308</PSTLZ>
   <LAND1>US</LAND1>
   <REGIO>CA</REGIO>
   <PFORT>92308</PFORT>
  </E1EDKA1>

  <E1EDKA1 SEGMENT="1">
   <PARVW>RG</PARVW>
   <PARTN>0000100016</PARTN>
   <NAME1>John Sample</NAME1>
   <STRAS>100 Sample Street</STRAS>
   <ORT01>Los Angeles</ORT01>
   <PSTLZ>773811234</PSTLZ>
   <LAND1>US</LAND1>
   <REGIO>CA</REGIO>
   <PFORT>92308</PFORT>
  </E1EDKA1>

  <E1EDKA1 SEGMENT="1">
   <PARVW>WE</PARVW>
   <PARTN>0000100016</PARTN>
   <NAME1>John Sample</NAME1>
   <STRAS>100 Sample Street</STRAS>
   <ORT01>Los Angeles</ORT01>
   <PSTLZ>92308</PSTLZ>
   <LAND1>US</LAND1>
   <REGIO>CA</REGIO>
   <PFORT>92308</PFORT>
  </E1EDKA1>

   <E1EDK02 SEGMENT="1">
   <QUALF>001</QUALF>
   <BELNR>450012345</BELNR>
   <DATUM>20160813</DATUM>
  </E1EDK02>

   <E1EDP01 SEGMENT="1">
   <QUALF>001</QUALF>
   <IDTNR>021V007534937002</IDTNR>
   <POSEX>00010</POSEX>
   <PSTYP>TAN</PSTYP>
   <MENGE>2</MENGE>
   <WERKS>3800</WERKS>
   <LGORT>0001</LGORT>

   <E1EDP19 SEGMENT="1">
    <QUALF>001</QUALF>
    <IDTNR>021V007534937002</IDTNR>
   </E1EDP19>

   <E1EDP19 SEGMENT="1">
    <QUALF>002</QUALF>
    <IDTNR>US-01-1000</IDTNR>
   </E1EDP19>

    <E1EDP01 SEGMENT="1">
   <QUALF>001</QUALF>
   <IDTNR>021V007534937002</IDTNR>
   <POSEX>00020</POSEX>
   <PSTYP>TAN</PSTYP>
   <MENGE>8</MENGE>
   <WERKS>3800</WERKS>
   <LGORT>0001</LGORT>

   <E1EDP19 SEGMENT="1">
    <QUALF>001</QUALF>
    <IDTNR>021V007534937004</IDTNR>
   </E1EDP19>

   <E1EDP19 SEGMENT="1">
    <QUALF>002</QUALF>
    <IDTNR>US-01-2000</IDTNR>
   </E1EDP19>

   <E1EDP19 SEGMENT="1">
    <QUALF>003</QUALF>
    <IDTNR>753793815800</IDTNR>
   </E1EDP19>

   </E1EDP01>
 </IDOC>
</ORDERS05>
```

← Previous: [Setting up the IDoc to confirm zQuote creation](../04-sales-document-idocs/02-quotation-confirmation-idoc.md) · Next: [Setting up the ORDRSP IDoc for confirmation of the sales order](../04-sales-document-idocs/04-ordrsp-idoc.md) →

---

© 2026 Onibex, LLC · Licensed under [CC BY-NC-ND 4.0](../../../LICENSE) (SPDX: CC-BY-NC-ND-4.0) · [Commercial license](../../../COMMERCIAL-LICENSE.md) · [Trademarks and third-party notices](../../../THIRD-PARTY-NOTICES.md) · SAP and other SAP products and services mentioned herein are trademarks or registered trademarks of SAP SE or an SAP affiliate company in Germany and other countries; names are used for identification only.
