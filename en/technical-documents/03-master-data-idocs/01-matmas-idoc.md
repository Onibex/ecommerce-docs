<!-- SPDX-License-Identifier: CC-BY-NC-ND-4.0 -->
<!-- Copyright (c) 2026 Onibex, LLC. Part of the Onibex eCommerce 360° Documentation — https://github.com/Onibex/ecommerce-docs -->

**English** · [Español](../../../es/technical-documents/03-master-data-idocs/01-matmas-idoc.md) | [↑ Technical documents index](../README.md) | [Repository README](../../../README.md)

# MATMAS IDoc configuration (material master)

> **Source:** Onibex Help Center article “6. MATMAS iDoc configuration” — <https://help.onibex.com/portal/en/kb/articles/matmas-idoc-configuration>. Spanish chapter D.4.a of the functional specification “D1 – Integración de sistemas”.

As mentioned in the configuration table of Figure-16, MATMAS IDoc is used for sending information from SAP Material Master to an External system, in this case, to the E-Commerce system.

To start creating those messages, access the screen in **Figure-13**, then select the ***Outbound*** section and, press the icon ![SAP toolbar icon](../../../assets/matmas-idoc/matmas-idoc-01.png) to add a new entry.

![SAP WE20 outbound MATMAS parameters, Outbound Options tab, basic type MATMAS05](../../../assets/matmas-idoc/matmas-idoc-02.png)

***Figure-17*** *WE20 Initial Screen for MATMAS Material Master.*

The following tabs are left unchanged; since IDoc MATMAS is related to master data, it is not necessary to configure any message.

![SAP WE20 Message Control tab left empty for MATMAS](../../../assets/matmas-idoc/matmas-idoc-03.png)

***Figure-18*** *Message Control tab*

![SAP WE20 Post Processing Permitted Agent tab, empty fields](../../../assets/matmas-idoc/matmas-idoc-04.png)

***Figure-19*** *Post-Processing tab*

![SAP WE20 Telephony tab with empty fields](../../../assets/matmas-idoc/matmas-idoc-05.png)

***Figure-20*** *Telephony tab*

![SAP WE20 EDI Standard tab with empty fields](../../../assets/matmas-idoc/matmas-idoc-06.png)

***Figure-21*** *EDI Standard tab.*

Once the appropriate options have been filled in, the next step is to configure the *DISTRIBUTION MODEL:* this is done in transaction **BD64.** Accessing BD64 T-Code, a screen like the one illustrated in Figure-22 is shown.

![SAP BD64 Display Distribution Model, list of model views](../../../assets/matmas-idoc/matmas-idoc-07.png)

***Figure-22*** *Initial BD64 Transaction Screen:* *Distribution Model.*

Click on ![SAP Display/Change toggle icon](../../../assets/matmas-idoc/matmas-idoc-08.png) to enter modification mode, then press ![SAP BD64 Create model view button](../../../assets/matmas-idoc/matmas-idoc-09.png), this will bring up a screen like the one shown in Figure-23.

![SAP BD64 Create Model View dialog for ECOMMERCE](../../../assets/matmas-idoc/matmas-idoc-10.png)

***Figure-23*** *Screen for creating the Definition of the Distribution Model, transaction BD64.*

Next add all the messages from the table in Figure-16; pay attention to the source and target system; for OUTBOUND messages, the Source system is the logical system that belongs to SAP, and the target system must be the E-COMMERCE. To start adding messages to transaction BD64 from Figure-22, press ![SAP BD64 Add message type button](../../../assets/matmas-idoc/matmas-idoc-11.png) and then fill in the fields with the following data:

![SAP BD64 Add Message Type dialog for MATMAS in model view ECOMMERCE](../../../assets/matmas-idoc/matmas-idoc-12.png)

***Figure-24*** *Creating the MATMAS Message type to send Material Master records to ECOMMERCE using transaction BD64.*

Continue with a similar procedure for all other messages based on the table of Figure-16, and thus, a Model View is set up for ONIBEX E-COMMERCE B2B DATA MODEL like the one shown in Figure-25.

![SAP BD64 distribution model ONIBEX expanded with its message types](../../../assets/matmas-idoc/matmas-idoc-13.png)

**Figure-25** Messages for ***Outbound*** IDocs in T-Code BD64: *Distribution Model*.

From this DATA MODEL some FILTERS can be setup in order to discriminate on certain organizational structures and record types. For instance, when opening MATMAS, no filter has been set. To display the filter attributes, press ![SAP BD64 Create filter group button](../../../assets/matmas-idoc/matmas-idoc-14.png) as shown in Figure-26.

![SAP BD64 Filter Changed dialog listing MATMAS filter fields](../../../assets/matmas-idoc/matmas-idoc-15.png)

***Figure-26*** *Setting a Filter for the IDoc MATMAS in transaction BD64.*

To specify the values for each field, left double-click to enter the screen illustrated in Figure-27.

![SAP BD64 MATMAS filter: Material Type value HAWA](../../../assets/matmas-idoc/matmas-idoc-16.png)

***Figure-27*** *Placing values in the Material Master Filter using transaction BD64.*

Notice that ONIBEX takes the HAWA material type from the inventory only.

Finally, send the records to the target system using transaction **BD10 MATERIAL SHIPPING.**

![SAP BD10 Send Material screen for message type MATMAS](../../../assets/matmas-idoc/matmas-idoc-17.png)

***Figure-28*** *Transaction screen BD10 to send Materials to Ecommerce catalog*

Click on the tick mark in T-Code BD10 from Figure-28, an IDoc for each material number is generated. SAP shows the following messages to confirm that material information is being sent.

![SAP popup: 22 master IDocs set up for MATMAS](../../../assets/matmas-idoc/matmas-idoc-18.png)![SAP popup: 22 communication IDocs generated for MATMAS](../../../assets/matmas-idoc/matmas-idoc-19.png)

***Figure-29*** *Messages given by the system when processing IDocs using transaction BD10.*

The previous IDocs in Figure-29 can be viewed from transaction **WE02**, when marked green, IDocs were transmitted correctly, as shown in Figure-30.

![SAP WE02 list of outbound MATMAS IDocs sent to ECOMMERCE](../../../assets/matmas-idoc/matmas-idoc-20.png)

***Figure-30*** *IDoc* ***Outbound*** *MATMAS processed correctly and viewed by transaction WE02.*

← Previous: [Setting up change pointers](../02-ale-foundations/05-change-pointers.md) · Next: [DEBMAS IDoc configuration (customer master)](../03-master-data-idocs/02-debmas-idoc.md) →

---

© 2026 Onibex, LLC · Licensed under [CC BY-NC-ND 4.0](../../../LICENSE) (SPDX: CC-BY-NC-ND-4.0) · [Commercial license](../../../COMMERCIAL-LICENSE.md) · [Trademarks and third-party notices](../../../THIRD-PARTY-NOTICES.md) · SAP and other SAP products and services mentioned herein are trademarks or registered trademarks of SAP SE or an SAP affiliate company in Germany and other countries; names are used for identification only.
