<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Part of the Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->

[English](../../../en/faq/02-pricing/01-run-price-job-manually.md) · **Español** | [↑ Índice de preguntas frecuentes](../README.md) | [README del repositorio](../../../README.md)

# Correr el job de precios de forma manual cuando el cliente no ve ciertos productos

> **Fuente:** artículo “Correr el job de precios de forma manual cuando el cliente no ve ciertos productos” del Help Center de Onibex — <https://help.onibex.com/portal/en/kb/articles/correr-job-de-precios-de-forma-manual-en-caso-de-que-el-cliente-no-vea-ciertos-productos>.

Una de las incidencias más comunes es cuando un cliente no encuentra ciertos productos dentro de la plataforma de ECommerce

En primer lugar hay que validar si el cliente tiene habilitados los canales relacionados con esa línea de productos.

En caso de que el cliente SÍ esté habilitado en el canal indicado y aun así no pueda ver ciertos productos, lo más probable es que no tenga asignados precios para esos determinados productos, por lo que estos no le resultan visibles.

Para asignar precios al cliente desde la parte de SAP, se realiza el siguiente proceso:

1. Se ejecuta la transacción ZON_CUST_IDOC
2. Identificar el número de cliente y asegurarnos de NO seleccionar el botón de change pointer

   *(Captura de pantalla no disponible en el artículo original.)*

Al realizar esto, al cliente deberían asignársele los precios indicados de forma automática, por lo que ahora debería de ser visible para ellos en el ECommerce.

En caso de que los productos no se visualicen para el cliente después de realizar esto favor de comunicarse a [support@onibex.com](mailto:support@onibex.com) para realizar una validación y revisión más puntual del caso del cliente.

---

© 2026 Onibex, LLC · Licenciado bajo [CC BY-NC-ND 4.0](../../../LICENSE) (SPDX: CC-BY-NC-ND-4.0) · [Licencia comercial](../../../COMMERCIAL-LICENSE.md) · [Marcas y avisos de terceros](../../../THIRD-PARTY-NOTICES.md) · SAP y los demás productos y servicios SAP mencionados son marcas comerciales o marcas registradas de SAP SE o de una empresa afiliada a SAP en Alemania y otros países; los nombres se usan solo con fines de identificación.
