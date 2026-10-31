<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Part of the Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->

**English** · [Español](../../es/technical-documents/README.md) | [Repository README](../../README.md)

# Technical documents — ALE, IDocs and web services in SAP ERP

Step-by-step configuration in SAP ERP for Onibex eCommerce 360°: ALE settings, IDocs for master data and sales documents, and SICF web services. The documents are numbered in reading order; each one also stands on its own. Spanish versions: [`es/technical-documents/`](../../es/technical-documents/README.md).

## Overview

| # | Document | Help Center source |
|---|---|---|
| 1 | [Systems integration overview: SAP ERP and eCommerce 360°](01-overview/01-systems-integration-overview.md) | D1 – Integración de sistemas, Introducción (ES → EN) |

## ALE foundations: logical system, RFC destination, port, partner profile, change pointers

| # | Document | Help Center source |
|---|---|---|
| 2 | [Logical system definition in SAP](02-ale-foundations/01-logical-system-definition.md) | 2. Logical system definition in SAP |
| 3 | [Defining the RFC destination in SAP](02-ale-foundations/02-rfc-destination.md) | 3. Defining the RFC Destination in SAP |
| 4 | [Port definition for IDoc processing in SAP](02-ale-foundations/03-idoc-port-definition.md) | 4. Port definition for iDoc processing in SAP |
| 5 | [SAP partner profile definition for IDocs](02-ale-foundations/04-partner-profile.md) | 5. SAP Partner profile definition idocs |
| 6 | [Setting up change pointers](02-ale-foundations/05-change-pointers.md) | 16. Setting up Change pointers |

## Master data IDocs: MATMAS and DEBMAS

| # | Document | Help Center source |
|---|---|---|
| 7 | [MATMAS IDoc configuration (material master)](03-master-data-idocs/01-matmas-idoc.md) | 6. MATMAS iDoc configuration |
| 8 | [DEBMAS IDoc configuration (customer master)](03-master-data-idocs/02-debmas-idoc.md) | 7. DEBMAS iDoc configuration |

## Sales document IDocs: quotations, contracts, orders, deliveries, invoices, transport

| # | Document | Help Center source |
|---|---|---|
| 9 | [Setting up the IDoc to create SD quotations](04-sales-document-idocs/01-quotation-idoc.md) | 8. Setting up the iDoc to create SD QUOTATIONS |
| 10 | [Setting up the IDoc to confirm zQuote creation](04-sales-document-idocs/02-quotation-confirmation-idoc.md) | 9. Setting up the iDOC to confirm zQuote creation |
| 11 | [ORDERS IDoc configuration for sales orders](04-sales-document-idocs/03-orders-idoc.md) | 10. ORDERS iDOC configuration for Sales Orders |
| 12 | [Setting up the ORDRSP IDoc for confirmation of the sales order](04-sales-document-idocs/04-ordrsp-idoc.md) | 11. Setting up the ORDRSP iDOC for confirmation of the Sales Order |
| 13 | [DESADV IDoc configuration to send delivery confirmation](04-sales-document-idocs/05-desadv-idoc.md) | 12. DESADV iDoc configuration to send Delivery confirmation |
| 14 | [Setting up the INVOIC IDoc to send the invoice](04-sales-document-idocs/06-invoic-idoc.md) | 13. Setting up the INVOIC iDOC to send the invoice |
| 15 | [ZON_SHP IDoc configuration to send the transport document](04-sales-document-idocs/07-zon-shp-transport-idoc.md) | D1 – Integración de sistemas, D.4.j (ES → EN) |

## Web services: SICF

| # | Document | Help Center source |
|---|---|---|
| 16 | [Deployment of SICF services for communications using web services](05-web-services/01-sicf-web-services.md) | 14. Deployment of SICF Service for communications using Web Services |

## Sales configuration: credit block, cross-selling and up-selling

| # | Document | Help Center source |
|---|---|---|
| 17 | [Creating a credit-control blocking reason in the Business Partner (BP)](06-sales-configuration/01-credit-block-reason-business-partner.md) | D1 – Integración de sistemas, D.4.i (bis) (ES → EN) |
| 18 | [Cross-selling and up-selling configuration (alternative materials)](06-sales-configuration/02-cross-selling-up-selling.md) | D1 – Integración de sistemas, D.7 (ES → EN) |

## Reference: complete SAP object list

| # | Document | Help Center source |
|---|---|---|
| 19 | [Complete SAP object list specification](07-reference/01-sap-object-list.md) | 15. Complete SAP Object List Specification |

---

© 2026 Onibex, LLC · Licensed under [CC BY-NC-ND 4.0](../../LICENSE) (SPDX: CC-BY-NC-ND-4.0) · [Commercial license](../../COMMERCIAL-LICENSE.md) · [Trademarks and third-party notices](../../THIRD-PARTY-NOTICES.md) · SAP and other SAP products and services mentioned herein are trademarks or registered trademarks of SAP SE or an SAP affiliate company in Germany and other countries; names are used for identification only.
