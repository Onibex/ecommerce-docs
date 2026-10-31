<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Part of the Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->

**English** · [Español](../../../es/faq/02-pricing/02-price-refresh-materials-prices.md) | [↑ FAQ index](../README.md) | [Repository README](../../../README.md)

# PRICE_REFRESH when adding materials and prices

> **Source:** English version of the Spanish FAQ article “PRICE_REFRESH al añadir materiales y precios” in the Onibex Help Center — <https://help.onibex.com/portal/en/kb/articles/a%C3%B1adir-materia>.

When adding new materials and prices, it is important to remember **NOT** to enable the **“Refresh Prices” (“Refrescar Precios”), or “PRICE_REFRESH”,** checkbox.

It is important to remember that the "Refresh" is responsible for deleting all the prices and assigning new ones; that is, if a new material is created, prices will be generated only for that material, or if a channel is created, they are generated only for that channel.

The **“PRICE_REFRESH”** checkbox should not be enabled, allowing the **“Change Pointers”** to do their job automatically; otherwise, all the prices for that specific customer would have to be sent again (an example is attached):

   *(Screenshot not available in the original article.)*

The "Refresh Prices" checkbox should be enabled only when a "Total Pricing" ("Pricing Total") is to be performed, which will affect the other products and channels.

Enabling this checkbox accidentally when adding a new material can cause the prices of other materials or products to become outdated, making them invisible to customers.

---

© 2026 Onibex, LLC · Licensed under [CC BY-NC-ND 4.0](../../../LICENSE) (SPDX: CC-BY-NC-ND-4.0) · [Commercial license](../../../COMMERCIAL-LICENSE.md) · [Trademarks and third-party notices](../../../THIRD-PARTY-NOTICES.md) · SAP and other SAP products and services mentioned herein are trademarks or registered trademarks of SAP SE or an SAP affiliate company in Germany and other countries; names are used for identification only.
