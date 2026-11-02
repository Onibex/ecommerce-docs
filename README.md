<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->
<!-- Suggested GitHub "About" description:
     Official documentation hub for Onibex eCommerce 360°, the B2B/B2C eCommerce platform designed for use with SAP ERP: ALE/IDoc configuration guides, SICF web services, SAP object list and FAQ. Bilingual (English/Spanish). CC BY-NC-ND 4.0.
     Suggested topics:
     onibex, ecommerce-360, sap, sap-erp, sap-s4hana, idoc, ale, b2b-ecommerce, b2c-ecommerce, prestashop, documentation, bilingual, spanish, cc-by-nc-nd
     Social preview image: .github/social-preview.png (upload it in Settings → General → Social preview) -->

<img width="4168" height="1064" alt="Onibex logo" src="https://github.com/user-attachments/assets/9514ac42-a356-41b4-9751-5c7d789cf713" />

# Onibex eCommerce 360° Documentation — B2B/B2C eCommerce for SAP ERP: ALE/IDoc configuration guides, SICF web services and FAQ (English · Español)

> **The B2B/B2C eCommerce platform built for SAP ERP.** Designed for use with SAP ERP to manage inventory, pricing, orders, and customer engagement in real time. From a Proof of Concept to a live storefront in as little as 10 days.

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC_BY--NC--ND_4.0-lightgrey.svg)](LICENSE) [![Languages: English · Español](https://img.shields.io/badge/Languages-English_%C2%B7_Espa%C3%B1ol-blue.svg)](#documentation) [![Commercial license available](https://img.shields.io/badge/Commercial_license-available-orange.svg)](COMMERCIAL-LICENSE.md)

**Languages / Idiomas:** [English](#english) · [Español](#español)

This repository is the official documentation hub for **Onibex eCommerce 360°**, the self-service commerce platform for SAP ERP that empowers wholesale and retail businesses to sell online without disconnecting from their SAP ERP core. The documentation is published in **English and Spanish**, with the same documents in both languages, under the Creative Commons **CC BY-NC-ND 4.0** license (noncommercial sharing with attribution; commercial license available).

---

## English

### Documentation

This branch (`technical-documents`) contains **19 documents in English and the same 19 in Spanish**, with **211 screenshots**. The FAQ articles are published in the branch [`faq`](https://github.com/Onibex/ecommerce-docs/tree/faq).

#### Technical documents — ALE, IDocs and web services in SAP ERP

Step-by-step configuration in SAP ERP, from the logical system to the IDocs that exchange master data and sales documents with the storefront. Read them in order the first time; each document also stands on its own.

| # | Document | Group |
|---|---|---|
| 1 | [Systems integration overview: SAP ERP and eCommerce 360°](en/technical-documents/01-overview/01-systems-integration-overview.md) | Overview |
| 2 | [Logical system definition in SAP](en/technical-documents/02-ale-foundations/01-logical-system-definition.md) | ALE foundations: logical system, RFC destination, port, partner profile, change pointers |
| 3 | [Defining the RFC destination in SAP](en/technical-documents/02-ale-foundations/02-rfc-destination.md) | ALE foundations: logical system, RFC destination, port, partner profile, change pointers |
| 4 | [Port definition for IDoc processing in SAP](en/technical-documents/02-ale-foundations/03-idoc-port-definition.md) | ALE foundations: logical system, RFC destination, port, partner profile, change pointers |
| 5 | [SAP partner profile definition for IDocs](en/technical-documents/02-ale-foundations/04-partner-profile.md) | ALE foundations: logical system, RFC destination, port, partner profile, change pointers |
| 6 | [Setting up change pointers](en/technical-documents/02-ale-foundations/05-change-pointers.md) | ALE foundations: logical system, RFC destination, port, partner profile, change pointers |
| 7 | [MATMAS IDoc configuration (material master)](en/technical-documents/03-master-data-idocs/01-matmas-idoc.md) | Master data IDocs: MATMAS and DEBMAS |
| 8 | [DEBMAS IDoc configuration (customer master)](en/technical-documents/03-master-data-idocs/02-debmas-idoc.md) | Master data IDocs: MATMAS and DEBMAS |
| 9 | [Setting up the IDoc to create SD quotations](en/technical-documents/04-sales-document-idocs/01-quotation-idoc.md) | Sales document IDocs: quotations, contracts, orders, deliveries, invoices, transport |
| 10 | [Setting up the IDoc to confirm zQuote creation](en/technical-documents/04-sales-document-idocs/02-quotation-confirmation-idoc.md) | Sales document IDocs: quotations, contracts, orders, deliveries, invoices, transport |
| 11 | [ORDERS IDoc configuration for sales orders](en/technical-documents/04-sales-document-idocs/03-orders-idoc.md) | Sales document IDocs: quotations, contracts, orders, deliveries, invoices, transport |
| 12 | [Setting up the ORDRSP IDoc for confirmation of the sales order](en/technical-documents/04-sales-document-idocs/04-ordrsp-idoc.md) | Sales document IDocs: quotations, contracts, orders, deliveries, invoices, transport |
| 13 | [DESADV IDoc configuration to send delivery confirmation](en/technical-documents/04-sales-document-idocs/05-desadv-idoc.md) | Sales document IDocs: quotations, contracts, orders, deliveries, invoices, transport |
| 14 | [Setting up the INVOIC IDoc to send the invoice](en/technical-documents/04-sales-document-idocs/06-invoic-idoc.md) | Sales document IDocs: quotations, contracts, orders, deliveries, invoices, transport |
| 15 | [ZON_SHP IDoc configuration to send the transport document](en/technical-documents/04-sales-document-idocs/07-zon-shp-transport-idoc.md) | Sales document IDocs: quotations, contracts, orders, deliveries, invoices, transport |
| 16 | [Deployment of SICF services for communications using web services](en/technical-documents/05-web-services/01-sicf-web-services.md) | Web services: SICF |
| 17 | [Creating a credit-control blocking reason in the Business Partner (BP)](en/technical-documents/06-sales-configuration/01-credit-block-reason-business-partner.md) | Sales configuration: credit block, cross-selling and up-selling |
| 18 | [Cross-selling and up-selling configuration (alternative materials)](en/technical-documents/06-sales-configuration/02-cross-selling-up-selling.md) | Sales configuration: credit block, cross-selling and up-selling |
| 19 | [Complete SAP object list specification](en/technical-documents/07-reference/01-sap-object-list.md) | Reference: complete SAP object list |


#### FAQ — store administration

Short how-to articles for the store administration panel (catalog, pricing, orders, administration).

Published in the branch [`faq`](https://github.com/Onibex/ecommerce-docs/tree/faq) — see its [English index](https://github.com/Onibex/ecommerce-docs/blob/faq/en/faq/README.md).

#### How to read this repository

- `en/` holds the English documents and `es/` the Spanish ones, with **identical structure and file names**; every document has a language switch at the top.
- `assets/` holds the screenshots shared by both languages. Screenshots were reviewed and, where needed, redacted before publication.
- [CONTENT-MAP.md](CONTENT-MAP.md) maps every document to its original Help Center article and states whether it is an original or a translation.
- [llms.txt](llms.txt) lists the documentation for AI assistants and search engines.
- The same content is available in the Onibex Help Center: <https://help.onibex.com/portal/en/kb/ecommerce360>.

### What is eCommerce 360°?

**eCommerce 360°** is an all-inclusive B2B and B2C commerce platform designed specifically for enterprises running SAP ERP. Unlike generic eCommerce platforms that require complex middleware to connect to SAP ERP, eCommerce 360° is designed for use with SAP ERP from the ground up. Every product, price, inventory level, and order flows in real time between your storefront and your SAP system, with no batch jobs, no data drift, and no reconciliation nightmares.

Built with business owners, product engineers, sales teams, and end customers in mind, eCommerce 360° gives your organization a modern, self-service commerce experience while preserving the SAP business processes your organization already runs on.

> 💡 **The Onibex difference:** If you had a heart condition, would you choose any doctor or a heart specialist? Onibex is eCommerce specialized in SAP ERP.

### Key Capabilities

#### 🛒 Self-Service Commerce Platform

Give your customers a modern, intuitive shopping experience with everything they need to do business with you 24/7:

- **Product catalog** with rich media, categorization, and search.
- **Real-time inventory** by plant and warehouse.
- **Customer-specific pricing** driven directly from SAP ERP pricing conditions.
- **Order placement** with validation against SAP ERP business rules.
- **Order history and tracking** with live status updates.
- **Account statements** and self-service AR visibility.

#### 🔗 Designed for use with SAP ERP

No middleware. No batch delays. eCommerce 360° talks directly to SAP ERP:

- **Real-time order flow** into SAP sales orders.
- **Live inventory** from SAP MM (`MARD`, `MSEG`).
- **Customer-specific pricing** from SAP SD pricing conditions.
- **Delivery and billing** synchronized with SAP ERP.
- **Master data governance** with SAP ERP as the source of truth.

#### 💬 Communication and Collaboration Tools

Turn your storefront into a collaboration hub between B2B Buyers, Sales Reps, and Customer Service:

- **Push notifications** for order updates, back-in-stock alerts, and campaigns.
- **Integrated ticketing system** for support requests.
- **Live chat** between customers and sales/support agents.
- **Reports and analytics** on customer behavior, sales performance, and support metrics.

#### 🎓 Onboarding and Self-Training

Reduce time-to-value for your customers and internal teams:

- **Virtual tour** for first-time users.
- **Self-explanatory UI** built on years of user research across industries.
- **Self-service help center** with searchable documentation.

#### ☁️ Enterprise-Grade Infrastructure

- **Cloud infrastructure on AWS** designed for enterprise security, reliability, and scalability.
- **Cloud-agnostic** deployment options.
- **Multi-tenant architecture** with role-based access control.
- **Enterprise-grade security and audit practices.**

### Who Is It For?

eCommerce 360° serves different roles across your organization:

| Role | What eCommerce 360° gives you |
|---|---|
| **Business Owners** | A modern digital sales channel that scales with your SAP business processes, without ripping and replacing your core. |
| **Sales Teams** | Live visibility into customer accounts, orders, and pipeline. Communication tools to interact with B2B Buyers directly. |
| **Product Engineers** | A flexible, non-linear platform to reorganize, compare, and improve products while keeping everything in place. |
| **Customer Service** | A ticketing system, live chat, and reports to serve customers proactively and reduce resolution times. |
| **B2B Buyers** | Self-service access to inventory, pricing, order placement, history, and account statements. No more waiting for a sales rep. |

### Why eCommerce 360° vs. Generic eCommerce Platforms

Generic eCommerce platforms treat SAP ERP as an afterthought. eCommerce 360° is built around SAP ERP from day one. Here's what that means in practice:

| Common Limitation of Generic Platforms | How eCommerce 360° Solves It |
|---|---|
| SAP data synced via batch jobs, causing pricing and inventory drift. | Real-time bidirectional data exchange with SAP ERP. |
| Customer-specific pricing requires custom middleware. | Built-in support for SAP ERP pricing conditions. |
| Order errors due to SAP validation failures after checkout. | Pre-checkout validation against SAP ERP business rules. |
| No visibility of the customer's actual SAP account state. | Live account statements, orders, and deliveries in-app. |
| Long implementation timelines (6-12 months). | Proof of Concept connected to your SAP ERP in **10 days**. |

### Request a Demo or Proof of Concept

Onibex offers a **Proof of Concept connected to your SAP ERP system in as little as 10 days**. Get in touch to see eCommerce 360° running against your own SAP data.

- 🌐 [Request a demo](https://www.onibex.com)
- 📧 [contact@onibex.com](mailto:contact@onibex.com)

### Related Solutions

eCommerce 360° works seamlessly with the rest of the Onibex product family:

- **[OneConnect](https://github.com/Onibex/oneconnect-docs)** — The real-time data integration platform for SAP systems that powers data flow between SAP systems and downstream systems.
- **[ASK. Agentic Semantic Knowledge](https://github.com/Onibex/agentic-semantic-knowledge-ask)** — AI-powered semantic querying over your SAP data products, giving your commerce and sales teams natural-language access to business insights.

### About Onibex

Onibex is a global software and services company specialized in **SAP data integration**, **agentic AI**, and **B2B/B2C eCommerce**. We help enterprises unlock the full value of their SAP data through real-time streaming, intelligent automation, and self-service digital commerce, all built with enterprise-grade governance.

- 🌐 **Website:** [www.onibex.com](https://www.onibex.com)
- 💼 **LinkedIn:** [linkedin.com/company/onibex](https://www.linkedin.com/company/onibex)
- 📧 **Email:** [contact@onibex.com](mailto:contact@onibex.com)
- 🛟 **Support:** [support@onibex.com](mailto:support@onibex.com)

### License

Copyright © 2026 Onibex, LLC. This documentation is licensed under the **Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0)** — see [LICENSE](LICENSE) (SPDX: `CC-BY-NC-ND-4.0`).

- You **may** copy and redistribute the documentation, unmodified, for noncommercial purposes, with attribution: *"Onibex eCommerce 360° Documentation" by Onibex, LLC, CC BY-NC-ND 4.0 — https://github.com/Onibex/ecommerce-docs*.
- You **may not** use it commercially or distribute modified versions (including translations and adaptations) without permission.
- **Commercial license available:** for commercial use, derivative works, translations or custom versions, contact **contact@onibex.com** — see [COMMERCIAL-LICENSE.md](COMMERCIAL-LICENSE.md).
- Third-party software shown or described here (SAP products, PrestaShop and third-party PrestaShop modules, Google Chrome, Microsoft Excel) keeps its own licenses and trademarks, and its user interfaces in the screenshots are not licensed by Onibex — see [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md) and [NOTICE](NOTICE).
- Found an error? See [CONTRIBUTING.md](CONTRIBUTING.md).

SAP and other SAP products and services mentioned in this documentation are trademarks or registered trademarks of SAP SE or an SAP affiliate company in Germany and other countries. PrestaShop is a trademark of PrestaShop SA. Amazon Web Services and AWS are trademarks of Amazon.com, Inc. or its affiliates. Other product and company names are trademarks of their respective owners. Onibex is an independent company; this is not SAP documentation and is not endorsed by SAP SE. Names are used for identification only.

### Citation

If you reference this documentation, please cite it using the metadata in [CITATION.cff](CITATION.cff) (GitHub shows a "Cite this repository" button).

---

## Español

### Documentación

Esta rama (`technical-documents`) contiene **19 documentos en inglés y los mismos 19 en español**, con **211 capturas de pantalla**. Las preguntas frecuentes se publican en la rama [`faq`](https://github.com/Onibex/ecommerce-docs/tree/faq).

#### Documentos técnicos — ALE, IDocs y servicios web en SAP ERP

Configuración paso a paso en SAP ERP, desde el sistema lógico hasta los IDocs que intercambian datos maestros y documentos de venta con la tienda en línea. Léalos en orden la primera vez; cada documento también se sostiene por sí mismo.

| # | Documento | Grupo |
|---|---|---|
| 1 | [Integración de sistemas: visión general (SAP ERP y eCommerce 360°)](es/technical-documents/01-overview/01-systems-integration-overview.md) | Visión general |
| 2 | [Definición de sistema lógico en SAP](es/technical-documents/02-ale-foundations/01-logical-system-definition.md) | Fundamentos ALE: sistema lógico, destino RFC, puerto, perfil de interlocutor, change pointers |
| 3 | [Definición del destino RFC (Remote Function Call) en SAP](es/technical-documents/02-ale-foundations/02-rfc-destination.md) | Fundamentos ALE: sistema lógico, destino RFC, puerto, perfil de interlocutor, change pointers |
| 4 | [Definición del puerto para el procesamiento de IDocs en SAP](es/technical-documents/02-ale-foundations/03-idoc-port-definition.md) | Fundamentos ALE: sistema lógico, destino RFC, puerto, perfil de interlocutor, change pointers |
| 5 | [Definición de perfiles de interlocutor (partner profile) en SAP](es/technical-documents/02-ale-foundations/04-partner-profile.md) | Fundamentos ALE: sistema lógico, destino RFC, puerto, perfil de interlocutor, change pointers |
| 6 | [Configuración de los punteros de modificación (change pointers)](es/technical-documents/02-ale-foundations/05-change-pointers.md) | Fundamentos ALE: sistema lógico, destino RFC, puerto, perfil de interlocutor, change pointers |
| 7 | [Configuración del IDoc MATMAS (maestro de materiales)](es/technical-documents/03-master-data-idocs/01-matmas-idoc.md) | IDocs de datos maestros: MATMAS y DEBMAS |
| 8 | [Configuración del IDoc DEBMAS (maestro de clientes)](es/technical-documents/03-master-data-idocs/02-debmas-idoc.md) | IDocs de datos maestros: MATMAS y DEBMAS |
| 9 | [Configuración del IDoc para crear cotizaciones (quotations) SD](es/technical-documents/04-sales-document-idocs/01-quotation-idoc.md) | IDocs de documentos de venta: cotizaciones, contratos, pedidos, entregas, facturas, transporte |
| 10 | [Configuración del IDoc para confirmar la creación de la cotización](es/technical-documents/04-sales-document-idocs/02-quotation-confirmation-idoc.md) | IDocs de documentos de venta: cotizaciones, contratos, pedidos, entregas, facturas, transporte |
| 11 | [Configuración del IDoc ORDERS para pedidos de venta (sales orders)](es/technical-documents/04-sales-document-idocs/03-orders-idoc.md) | IDocs de documentos de venta: cotizaciones, contratos, pedidos, entregas, facturas, transporte |
| 12 | [Configuración del IDoc ORDRSP para la confirmación del pedido de venta](es/technical-documents/04-sales-document-idocs/04-ordrsp-idoc.md) | IDocs de documentos de venta: cotizaciones, contratos, pedidos, entregas, facturas, transporte |
| 13 | [Configuración del IDoc DESADV para enviar la confirmación de la entrega](es/technical-documents/04-sales-document-idocs/05-desadv-idoc.md) | IDocs de documentos de venta: cotizaciones, contratos, pedidos, entregas, facturas, transporte |
| 14 | [Configuración del IDoc INVOIC para enviar la factura](es/technical-documents/04-sales-document-idocs/06-invoic-idoc.md) | IDocs de documentos de venta: cotizaciones, contratos, pedidos, entregas, facturas, transporte |
| 15 | [Configuración del IDoc ZON_SHP para enviar el documento de transporte](es/technical-documents/04-sales-document-idocs/07-zon-shp-transport-idoc.md) | IDocs de documentos de venta: cotizaciones, contratos, pedidos, entregas, facturas, transporte |
| 16 | [Creación de servicios en SICF para la comunicación por web services](es/technical-documents/05-web-services/01-sicf-web-services.md) | Servicios web: SICF |
| 17 | [Creación del motivo de bloqueo para control de crédito en el Business Partner (BP)](es/technical-documents/06-sales-configuration/01-credit-block-reason-business-partner.md) | Configuración de ventas: bloqueo de crédito, cross-selling y up-selling |
| 18 | [Configuración de materiales alternativos: cross-selling y up-selling](es/technical-documents/06-sales-configuration/02-cross-selling-up-selling.md) | Configuración de ventas: bloqueo de crédito, cross-selling y up-selling |
| 19 | [Especificación completa de la lista de objetos de SAP](es/technical-documents/07-reference/01-sap-object-list.md) | Referencia: lista completa de objetos SAP |


#### Preguntas frecuentes (FAQ) — administración de la tienda

Artículos breves de "cómo hacer" para el panel de administración de la tienda (catálogo, precios, pedidos, administración).

Publicadas en la rama [`faq`](https://github.com/Onibex/ecommerce-docs/tree/faq) — vea su [índice en español](https://github.com/Onibex/ecommerce-docs/blob/faq/es/faq/README.md).

#### Cómo leer este repositorio

- `en/` contiene los documentos en inglés y `es/` los documentos en español, con **la misma estructura y los mismos nombres de archivo**; cada documento tiene un selector de idioma al inicio.
- `assets/` contiene las capturas de pantalla compartidas por ambos idiomas. Las capturas se revisaron y, donde hizo falta, se anonimizaron antes de publicar.
- [CONTENT-MAP.md](CONTENT-MAP.md) relaciona cada documento con su artículo original del Help Center e indica si es un original o una traducción.
- [llms.txt](llms.txt) lista la documentación para asistentes de IA y buscadores.
- El mismo contenido está disponible en el Help Center de Onibex: <https://help.onibex.com/portal/en/kb/ecommerce360>.

### ¿Qué es eCommerce 360°?

**eCommerce 360°** es una plataforma integral de comercio B2B y B2C diseñada específicamente para empresas que operan SAP ERP. A diferencia de las plataformas de comercio electrónico genéricas, que requieren middleware complejo para conectarse con SAP ERP, eCommerce 360° está diseñada desde su origen para usarse con SAP ERP. Cada producto, precio, nivel de inventario y pedido fluye en tiempo real entre su tienda en línea y su sistema SAP, sin procesos por lotes, sin desfases de datos y sin conciliaciones interminables.

Pensada para dueños de negocio, ingenieros de producto, equipos de ventas y clientes finales, eCommerce 360° ofrece a su organización una experiencia de comercio moderna y de autoservicio, conservando los procesos de negocio SAP con los que su organización ya opera.

> 💡 **La diferencia Onibex:** si tuviera una afección cardíaca, ¿elegiría a cualquier médico o a un cardiólogo? Onibex es comercio electrónico especializado en SAP ERP.

### Capacidades clave

#### 🛒 Plataforma de comercio de autoservicio

Ofrezca a sus clientes una experiencia de compra moderna e intuitiva con todo lo que necesitan para hacer negocios con usted las 24 horas:

- **Catálogo de productos** con contenido multimedia, categorización y búsqueda.
- **Inventario en tiempo real** por centro y almacén.
- **Precios específicos por cliente** tomados directamente de las condiciones de precio de SAP ERP.
- **Captura de pedidos** con validación contra las reglas de negocio de SAP ERP.
- **Historial y seguimiento de pedidos** con estatus en vivo.
- **Estados de cuenta** y visibilidad de cuentas por cobrar en autoservicio.

#### 🔗 Diseñada para usarse con SAP ERP

Sin middleware. Sin retrasos por lotes. eCommerce 360° se comunica directamente con SAP ERP:

- **Flujo de pedidos en tiempo real** hacia pedidos de venta de SAP.
- **Inventario en vivo** desde SAP MM (`MARD`, `MSEG`).
- **Precios específicos por cliente** desde las condiciones de precio de SAP SD.
- **Entregas y facturación** sincronizadas con SAP ERP.
- **Gobierno de datos maestros** con SAP ERP como fuente de la verdad.

#### 💬 Herramientas de comunicación y colaboración

Convierta su tienda en un centro de colaboración entre compradores B2B, representantes de ventas y servicio al cliente:

- **Notificaciones push** sobre actualizaciones de pedidos, alertas de disponibilidad y campañas.
- **Sistema de tickets integrado** para solicitudes de soporte.
- **Chat en vivo** entre clientes y agentes de ventas o soporte.
- **Reportes y analítica** sobre comportamiento de clientes, desempeño de ventas y métricas de soporte.

#### 🎓 Incorporación y autocapacitación

Reduzca el tiempo de adopción para sus clientes y equipos internos:

- **Recorrido virtual** para usuarios nuevos.
- **Interfaz autoexplicativa** basada en años de investigación con usuarios de distintas industrias.
- **Centro de ayuda de autoservicio** con documentación consultable.

#### ☁️ Infraestructura de clase empresarial

- **Infraestructura en la nube de AWS** diseñada para seguridad, confiabilidad y escalabilidad empresarial.
- Opciones de despliegue **independientes del proveedor de nube**.
- **Arquitectura multiinquilino** con control de acceso basado en roles.
- **Prácticas de seguridad y auditoría de clase empresarial.**

### ¿Para quién es?

eCommerce 360° atiende a distintos roles de su organización:

| Rol | Lo que eCommerce 360° le ofrece |
|---|---|
| **Dueños de negocio** | Un canal de ventas digital moderno que escala con sus procesos de negocio SAP, sin reemplazar su núcleo. |
| **Equipos de ventas** | Visibilidad en vivo de cuentas, pedidos y pipeline. Herramientas de comunicación para interactuar directamente con los compradores B2B. |
| **Ingenieros de producto** | Una plataforma flexible y no lineal para reorganizar, comparar y mejorar productos sin perder nada en el camino. |
| **Servicio al cliente** | Un sistema de tickets, chat en vivo y reportes para atender a los clientes de forma proactiva y reducir los tiempos de resolución. |
| **Compradores B2B** | Acceso en autoservicio a inventario, precios, captura de pedidos, historial y estados de cuenta. Sin esperar a un representante. |

### Por qué eCommerce 360° frente a las plataformas genéricas

Las plataformas genéricas tratan a SAP ERP como algo secundario. eCommerce 360° se construyó alrededor de SAP ERP desde el primer día. En la práctica:

| Limitación común de las plataformas genéricas | Cómo lo resuelve eCommerce 360° |
|---|---|
| Datos de SAP sincronizados por lotes, con desfases de precios e inventario. | Intercambio bidireccional de datos en tiempo real con SAP ERP. |
| Los precios por cliente requieren middleware a la medida. | Soporte incluido para las condiciones de precio de SAP ERP. |
| Errores de pedido por fallas de validación en SAP después del checkout. | Validación contra las reglas de negocio de SAP ERP antes del checkout. |
| Sin visibilidad del estado real de la cuenta del cliente en SAP. | Estados de cuenta, pedidos y entregas en vivo dentro de la aplicación. |
| Tiempos de implementación largos (6 a 12 meses). | Prueba de concepto conectada a su SAP ERP en **10 días**. |

### Solicite una demostración o una prueba de concepto

Onibex ofrece una **prueba de concepto conectada a su sistema SAP ERP en tan solo 10 días**. Contáctenos para ver eCommerce 360° funcionando con sus propios datos de SAP.

- 🌐 [Solicitar una demostración](https://www.onibex.com)
- 📧 [contact@onibex.com](mailto:contact@onibex.com)

### Soluciones relacionadas

eCommerce 360° trabaja en conjunto con el resto de la familia de productos Onibex:

- **[OneConnect](https://github.com/Onibex/oneconnect-docs)** — La plataforma de integración de datos en tiempo real para sistemas SAP que impulsa el flujo de datos entre los sistemas SAP y los sistemas destino.
- **[ASK. Agentic Semantic Knowledge](https://github.com/Onibex/agentic-semantic-knowledge-ask)** — Consultas semánticas con IA sobre sus productos de datos (data products) de SAP, que dan a sus equipos de comercio y ventas acceso en lenguaje natural a la información del negocio.

### Acerca de Onibex

Onibex es una empresa global de software y servicios especializada en **integración de datos SAP**, **IA agéntica** y **comercio electrónico B2B/B2C**. Ayudamos a las empresas a aprovechar todo el valor de sus datos SAP mediante streaming en tiempo real, automatización inteligente y comercio digital de autoservicio, todo construido con gobierno de clase empresarial.

- 🌐 **Sitio web:** [www.onibex.com](https://www.onibex.com)
- 💼 **LinkedIn:** [linkedin.com/company/onibex](https://www.linkedin.com/company/onibex)
- 📧 **Correo:** [contact@onibex.com](mailto:contact@onibex.com)
- 🛟 **Soporte:** [support@onibex.com](mailto:support@onibex.com)

### Licencia

Copyright © 2026 Onibex, LLC. Esta documentación se licencia bajo la **licencia Creative Commons Atribución-NoComercial-SinDerivadas 4.0 Internacional (CC BY-NC-ND 4.0)** — vea [LICENSE](LICENSE) (SPDX: `CC-BY-NC-ND-4.0`).

- **Puede** copiar y redistribuir la documentación, sin modificar, con fines no comerciales y con atribución: *"Onibex eCommerce 360° Documentation" de Onibex, LLC, CC BY-NC-ND 4.0 — https://github.com/Onibex/ecommerce-docs*.
- **No puede** usarla con fines comerciales ni distribuir versiones modificadas (incluidas traducciones y adaptaciones) sin permiso.
- **Licencia comercial disponible:** para uso comercial, obras derivadas, traducciones o versiones personalizadas, escriba a **contact@onibex.com** — vea [COMMERCIAL-LICENSE.md](COMMERCIAL-LICENSE.md).
- El software de terceros mostrado o descrito aquí (productos SAP, PrestaShop y módulos de PrestaShop de terceros, Google Chrome, Microsoft Excel) conserva sus propias licencias y marcas, y sus interfaces en las capturas no quedan licenciadas por Onibex — vea [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md) y [NOTICE](NOTICE).
- ¿Encontró un error? Vea [CONTRIBUTING.md](CONTRIBUTING.md).

SAP y los demás productos y servicios SAP mencionados en esta documentación son marcas comerciales o marcas registradas de SAP SE o de una empresa afiliada a SAP en Alemania y otros países. PrestaShop es marca de PrestaShop SA. Amazon Web Services y AWS son marcas de Amazon.com, Inc. o sus filiales. Los demás nombres de productos y empresas son marcas de sus respectivos titulares. Onibex es una empresa independiente; esta no es documentación de SAP ni está respaldada por SAP SE. Los nombres se usan solo con fines de identificación.

### Cómo citar

Si hace referencia a esta documentación, cítela con los metadatos de [CITATION.cff](CITATION.cff) (GitHub muestra el botón "Cite this repository").
