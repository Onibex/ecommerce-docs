<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Part of the Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->

[English](../../en/technical-documents/README.md) · **Español** | [README del repositorio](../../README.md)

# Documentos técnicos — ALE, IDocs y servicios web en SAP ERP

Configuración paso a paso en SAP ERP para Onibex eCommerce 360°: ajustes ALE, IDocs de datos maestros y de documentos de venta, y servicios web SICF. Los documentos están numerados en orden de lectura; cada uno también se sostiene por sí mismo. Versiones en inglés: [`en/technical-documents/`](../../en/technical-documents/README.md).

## Visión general

| # | Documento | Fuente en el Help Center |
|---|---|---|
| 1 | [Integración de sistemas: visión general (SAP ERP y eCommerce 360°)](01-overview/01-systems-integration-overview.md) | D1 – Integración de sistemas, Introducción |

## Fundamentos ALE: sistema lógico, destino RFC, puerto, perfil de interlocutor, change pointers

| # | Documento | Fuente en el Help Center |
|---|---|---|
| 2 | [Definición de sistema lógico en SAP](02-ale-foundations/01-logical-system-definition.md) | 2. Logical system definition in SAP (EN → ES) |
| 3 | [Definición del destino RFC (Remote Function Call) en SAP](02-ale-foundations/02-rfc-destination.md) | 3. Defining the RFC Destination in SAP (EN → ES) |
| 4 | [Definición del puerto para el procesamiento de IDocs en SAP](02-ale-foundations/03-idoc-port-definition.md) | 4. Port definition for iDoc processing in SAP (EN → ES) |
| 5 | [Definición de perfiles de interlocutor (partner profile) en SAP](02-ale-foundations/04-partner-profile.md) | 5. SAP Partner profile definition idocs (EN → ES) |
| 6 | [Configuración de los punteros de modificación (change pointers)](02-ale-foundations/05-change-pointers.md) | 16. Setting up Change pointers (EN → ES) |

## IDocs de datos maestros: MATMAS y DEBMAS

| # | Documento | Fuente en el Help Center |
|---|---|---|
| 7 | [Configuración del IDoc MATMAS (maestro de materiales)](03-master-data-idocs/01-matmas-idoc.md) | 6. MATMAS iDoc configuration (EN → ES) |
| 8 | [Configuración del IDoc DEBMAS (maestro de clientes)](03-master-data-idocs/02-debmas-idoc.md) | 7. DEBMAS iDoc configuration (EN → ES) |

## IDocs de documentos de venta: cotizaciones, contratos, pedidos, entregas, facturas, transporte

| # | Documento | Fuente en el Help Center |
|---|---|---|
| 9 | [Configuración del IDoc para crear cotizaciones (quotations) SD](04-sales-document-idocs/01-quotation-idoc.md) | 8. Setting up the iDoc to create SD QUOTATIONS (EN → ES) |
| 10 | [Configuración del IDoc para confirmar la creación de la cotización](04-sales-document-idocs/02-quotation-confirmation-idoc.md) | 9. Setting up the iDOC to confirm zQuote creation (EN → ES) |
| 11 | [Configuración del IDoc ORDERS para pedidos de venta (sales orders)](04-sales-document-idocs/03-orders-idoc.md) | 10. ORDERS iDOC configuration for Sales Orders (EN → ES) |
| 12 | [Configuración del IDoc ORDRSP para la confirmación del pedido de venta](04-sales-document-idocs/04-ordrsp-idoc.md) | 11. Setting up the ORDRSP iDOC for confirmation of the Sales Order (EN → ES) |
| 13 | [Configuración del IDoc DESADV para enviar la confirmación de la entrega](04-sales-document-idocs/05-desadv-idoc.md) | 12. DESADV iDoc configuration to send Delivery confirmation (EN → ES) |
| 14 | [Configuración del IDoc INVOIC para enviar la factura](04-sales-document-idocs/06-invoic-idoc.md) | 13. Setting up the INVOIC iDOC to send the invoice (EN → ES) |
| 15 | [Configuración del IDoc ZON_SHP para enviar el documento de transporte](04-sales-document-idocs/07-zon-shp-transport-idoc.md) | D1 – Integración de sistemas, D.4.j |

## Servicios web: SICF

| # | Documento | Fuente en el Help Center |
|---|---|---|
| 16 | [Creación de servicios en SICF para la comunicación por web services](05-web-services/01-sicf-web-services.md) | 14. Deployment of SICF Service for communications using Web Services (EN → ES) |

## Configuración de ventas: bloqueo de crédito, cross-selling y up-selling

| # | Documento | Fuente en el Help Center |
|---|---|---|
| 17 | [Creación del motivo de bloqueo para control de crédito en el Business Partner (BP)](06-sales-configuration/01-credit-block-reason-business-partner.md) | D1 – Integración de sistemas, D.4.i (bis) |
| 18 | [Configuración de materiales alternativos: cross-selling y up-selling](06-sales-configuration/02-cross-selling-up-selling.md) | D1 – Integración de sistemas, D.7 |

## Referencia: lista completa de objetos SAP

| # | Documento | Fuente en el Help Center |
|---|---|---|
| 19 | [Especificación completa de la lista de objetos de SAP](07-reference/01-sap-object-list.md) | 15. Complete SAP Object List Specification (EN → ES) |

---

© 2026 Onibex, LLC · Licenciado bajo [CC BY-NC-ND 4.0](../../LICENSE) (SPDX: CC-BY-NC-ND-4.0) · [Licencia comercial](../../COMMERCIAL-LICENSE.md) · [Marcas y avisos de terceros](../../THIRD-PARTY-NOTICES.md) · SAP y los demás productos y servicios SAP mencionados son marcas comerciales o marcas registradas de SAP SE o de una empresa afiliada a SAP en Alemania y otros países; los nombres se usan solo con fines de identificación.
