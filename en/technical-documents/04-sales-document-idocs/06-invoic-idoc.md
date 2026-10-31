<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Part of the Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->

**English** · [Español](../../../es/technical-documents/04-sales-document-idocs/06-invoic-idoc.md) | [↑ Technical documents index](../README.md) | [Repository README](../../../README.md)

# Setting up the INVOIC IDoc to send the invoice

> **Source:** Onibex Help Center article “13. Setting up the INVOIC iDOC to send the invoice” — <https://help.onibex.com/portal/en/kb/articles/setting-up-the-invoic-idoc-to-send-the-invoice>. Spanish chapter D.4.i of the functional specification “D1 – Integración de sistemas”.

The first step is to configure an ***output type*** for message output in the **VF01** transaction. This *Output Type*’s configuration is done starting out in the NACE transaction and thus, creating a ZIEC message type for **V3** application area, as shown in Figure-127. From Figure-128 to Figure-131, the settings for the different tabs comprising this new ZIEC message class in the NACE transaction are shown.

![SAP NACE applications list, V3 Billing selected](../../../assets/invoic-idoc/invoic-idoc-01.png) ![SAP NACE billing output types, ZIEC Invoice to E-Comerce selected](../../../assets/invoic-idoc/invoic-idoc-02.png)

**Figure-127** Creation of the new **ZIEC** message in V3 application area of the NACE transaction.

![SAP NACE output type ZIEC general data tab](../../../assets/invoic-idoc/invoic-idoc-03.png)

**Figure-128** Configuring the access sequence for the new ZIEC output type in the V3 Application Area of the NACE transaction.

![SAP NACE output type ZIEC default values, ALE, bill-to party](../../../assets/invoic-idoc/invoic-idoc-04.png)

**Figure-129** Setting up the second tab for the new ZIEC output type.

![SAP NACE output type ZIEC time tab](../../../assets/invoic-idoc/invoic-idoc-05.png)

**Figure-130** Setting up the third tab for the new ZIEC output type.

![SAP NACE output type ZIEC storage system tab](../../../assets/invoic-idoc/invoic-idoc-06.png)

**Figure-131** Setting up the fourth tab for the new ZIEC output type.

The last three tabs are empty for this kind of ZIEC message.

Within the Message Class Dialog Structure, select the folder corresponding to *Processing Routines* and double-click it; Figure-132 appears to add the corresponding settings to the ALE Distribution processing medium.

![SAP NACE ZIEC processing routines including RSNASTED ALE_PROCESSING](../../../assets/invoic-idoc/invoic-idoc-07.png)

**Figure-132** Setup screen of the *Processing Routines* in the NACE Transaction for the new ZIEC message.

Within the same Message Class Dialog Structure, move to the Partner Functions folder and double-click on it to display the Figure-133.

![SAP NACE ZIEC partner functions, BP bill-to party](../../../assets/invoic-idoc/invoic-idoc-08.png)

**Figure-133** Configuration screen of the Partner Functions in the NACE Transaction for the new ZIEC message.

Return to the main menu of the NACE Transaction to configure the *MESSAGE DETERMINATION PROCEDURE* ![SAP NACE Procedures button](../../../assets/invoic-idoc/invoic-idoc-09.png) . A screen similar to Figure-134 will be displayed, from there it is needed to have: Procedure **V10000** *Billing Output* as well as the **Control** folder options selected, and thus right-click on the mouse to *Choose subdialog*.

![SAP NACE billing procedures, V10000 Billing Output selected](../../../assets/invoic-idoc/invoic-idoc-10.png)

**Figure-134** Configuration screen of the Partner Functions in the NACE Transaction for the new ZIEC message.

The screen from Figure-135 appears, and there, the highlighted line from **ZIEC** message that would be defined by clicking ![SAP New Entries button](../../../assets/invoic-idoc/invoic-idoc-11.png) button.

![SAP NACE procedure V10000 control steps with ZIEC](../../../assets/invoic-idoc/invoic-idoc-12.png)

**Figure-135** Setup screen for invoice *output* in the NACE Transaction.

Now create the *Condition Record* from the main menu of the **NACE** transaction for the **V3** area and the **ZIEC** *output type*.

![SAP NACE output types popup, ZIEC selected](../../../assets/invoic-idoc/invoic-idoc-13.png)

**Figure-136** Setup screen for the *Condition* *record* of the invoice in the NACE Transaction.

Double-click on this record in Figure-136 and enter the screen of Figure-137 to create that *Condition* *Record.* The next step is to fill out the Condition Records fields using the data of Figure-138.

![SAP VV32 change output condition ZIEC selection screen](../../../assets/invoic-idoc/invoic-idoc-14.png)

**Figure-137** Invoice *Condition* *record* creation screen in NACE Transaction.

![SAP VV32 condition record for ZIEC, billing type F2, BP, ALE](../../../assets/invoic-idoc/invoic-idoc-15.png)

**Figure-138** Screen that defines the Partner Function in the creation of the Invoice *Condition* *record* in the NACE Transaction.

Once the message has been created go to the **WE20** transaction to add the **INVOIC** standard *Message Type*:

![SAP WE20 partner profile ECOMMERCE, outbound message type INVOIC](../../../assets/invoic-idoc/invoic-idoc-16.png)

**Figure-139** Display on which the output parameters for the INVOIC message type are configured in WE20 transaction.

In the detail of this configuration, use **INVOIC** *Message Type* and the **INVOIC02** Basic *Type* as shown in Figure-140 and Figure-141:

![SAP WE20 outbound parameters INVOIC, port ECOMMERCE, INVOIC02](../../../assets/invoic-idoc/invoic-idoc-17.png)

**Figure-140** First tab configuration screen for the INVOIC message type in transaction WE20.

![SAP WE20 outbound INVOIC parameters, Message Control tab with ZIEC SD09](../../../assets/invoic-idoc/invoic-idoc-18.png)

**Figure-141** Second tab configuration screen for INVOIC message type in WE20 transaction.

Now add this *Message Type* in **BD64** transaction: *Distribution Model*, in order to define the direction in which that message will be generated:

![SAP BD64 Add Message Type dialog for INVOIC in model view ECOMMERCE](../../../assets/invoic-idoc/invoic-idoc-19.png)

**Figure-142** Adding a new entry for the INVOIC message type in BD64 transaction.

![SAP BD64 distribution model tree with INVOIC message type highlighted](../../../assets/invoic-idoc/invoic-idoc-20.png)

**Figure-143** Deployment of the newly created INVOIC message type in BD64 transaction.

← Previous: [DESADV IDoc configuration to send delivery confirmation](../04-sales-document-idocs/05-desadv-idoc.md) · Next: [ZON_SHP IDoc configuration to send the transport document](../04-sales-document-idocs/07-zon-shp-transport-idoc.md) →

---

© 2026 Onibex, LLC · Licensed under [CC BY-NC-ND 4.0](../../../LICENSE) (SPDX: CC-BY-NC-ND-4.0) · [Commercial license](../../../COMMERCIAL-LICENSE.md) · [Trademarks and third-party notices](../../../THIRD-PARTY-NOTICES.md) · SAP and other SAP products and services mentioned herein are trademarks or registered trademarks of SAP SE or an SAP affiliate company in Germany and other countries; names are used for identification only.
