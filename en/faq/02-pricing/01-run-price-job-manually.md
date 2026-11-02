<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Part of the Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->

**English** · [Español](../../../es/faq/02-pricing/01-run-price-job-manually.md) | [↑ FAQ index](../README.md) | [Repository README](../../../README.md)

# Running the price job manually when a customer cannot see certain products

> **Source:** English version of the Spanish FAQ article “Correr el job de precios de forma manual cuando el cliente no ve ciertos productos” in the Onibex Help Center — <https://help.onibex.com/portal/en/kb/articles/correr-job-de-precios-de-forma-manual-en-caso-de-que-el-cliente-no-vea-ciertos-productos>.

One of the most common incidents is when a customer cannot find certain products within the eCommerce platform

First, it must be validated whether the customer has the channels related to that product line enabled.

If the customer IS enabled in the indicated channel and still cannot see certain products, most likely no prices have been assigned to those specific products, which is why they are not visible to the customer.

To assign prices to the customer from the SAP side, the following process is carried out:

1. Run transaction ZON_CUST_IDOC
2. Identify the customer number and make sure NOT to select the change pointer button

   *(Screenshot not available in the original article.)*

After doing this, the indicated prices should be assigned to the customer automatically, so the products should now be visible to the customer in the eCommerce platform.

If the products are not displayed for the customer after doing this, please contact [support@onibex.com](mailto:support@onibex.com) for a more specific validation and review of the customer's case.

---

© 2026 Onibex, LLC · Licensed under [CC BY-NC-ND 4.0](../../../LICENSE) (SPDX: CC-BY-NC-ND-4.0) · [Commercial license](../../../COMMERCIAL-LICENSE.md) · [Trademarks and third-party notices](../../../THIRD-PARTY-NOTICES.md) · SAP and other SAP products and services mentioned herein are trademarks or registered trademarks of SAP SE or an SAP affiliate company in Germany and other countries; names are used for identification only.
