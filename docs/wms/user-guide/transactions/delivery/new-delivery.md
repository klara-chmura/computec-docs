---
sidebar_position: 6
---

# New Delivery

Since version 2.10.23.1, a new version of the Delivery document is available.

A Delivery document can be created from the following base documents: Pick List, Sales Order, A/R Reserve Invoice, or Draft.
![image](https://github.com/user-attachments/assets/ae4baf7b-5f6f-414a-8b89-1a0511470bfa)


Once you select a base document or start a new one, the Document Details screen will appear. This screen visualizes the lines from the selected SAP base document:
![image](https://github.com/user-attachments/assets/306587d2-5442-4701-b463-b4dc0199869d)

You can customize this view by adding up to two additional fields with information about each line. To configure this, go to:
<details>
<summary>Custom Configuration → Manager → Extra SQL Fields on Main List Items</summary>
<div>
    Load one of the fields:
![image](https://github.com/user-attachments/assets/43b1c422-0291-4a23-b559-de81d6d52fd3)
Enter the SQL query to get certain info:
  ![image](https://github.com/user-attachments/assets/d05d49e6-806a-4ff3-a1e5-c5c3b2bffba0)
</div>
</details>
Additionally, you can customize the buttons displayed on the bottom bar to disable the option to add a Storage Unit, if needed:
<details>
<summary>Custom Configuration → Delivery → Hide SU</summary>
<div>
![image](https://github.com/user-attachments/assets/9578e790-62af-4399-bb4d-cfbaece1f235)
</div>
</details>
If you choose to create a Storage Unit, its SU Code will appear in the top bar:
![image](https://github.com/user-attachments/assets/c7649f39-e236-4aa9-9a9c-dc5157dac0bf)

After selecting or scanning an item, you can enter the requested or allocated quantity. A list of available batches will be shown:
![image](https://github.com/user-attachments/assets/ae4548c4-97c5-4c4e-b4e1-27ae650d8277)

When you add a new Storage Unit, its SU Code will also be displayed in the top bar. You can switch between Storage Units by either scanning the SU Code / SSCC, or by tapping the top bar (to stop adding to the current SU), and selecting the SU you want to edit:
![image](https://github.com/user-attachments/assets/e9f95c67-07d4-472e-bf0f-7491e58ada93) ![image](https://github.com/user-attachments/assets/e3e6ab5b-6d79-417c-9345-b7b896cb329d)

You can enable the Packing Slip feature to track what was packed into each Storage Unit. To enable it, go to:
<details>
<summary>Custom Configuration → Delivery → Enable Packing Slip</summary>
<div>
![image](https://github.com/user-attachments/assets/80db5922-539d-4845-9fc3-26960f96f95f)
Once the Delivery document is saved, you can open the Packing Slip directly from it:

The Packing Slip shows which items were packed into which Storage Units:

</div>
</details>
When the requested quantity is fulfilled, the line will turn green.
![image](https://github.com/user-attachments/assets/61691f94-c54e-43b5-aff7-970c13cf14a0)

You can now save the document either as a Delivery or as a Draft.
![image](https://github.com/user-attachments/assets/06c1eac9-3b8b-44d5-9a5b-87bf4434e70b)
You may also attach a file – these options can be enabled in the Custom Configuration → Delivery tab:
<details>
<summary>Custom Configuration → Delivery</summary>
<div>
![image](https://github.com/user-attachments/assets/45862b18-9fce-4e27-8c1c-2d315115b253)
</div>
</details>




:::info
Some forms' order and availability during document creation may vary depending on individual settings. Click here to find out more.
:::

- Press the Delivery in the main menu to create a delivery document.
![Delivery](./media/delivery.png)
![Delivery](./media/delivery-operations-01.png)

- The Source Warehouse window will appear.
Choose the desired warehouse by clicking its row.
![Warehouse Filter](./media/warehouse-filter.png)

:::caution
Searching through the records is available in every window in which a Filter row is displayed by typing in at least a part of a name, e.g., a part of a Warehouse name, in the Warehouse Selection window.
:::
    ![Warehouse](./media/warehouse.png)

:::caution
This step can be skipped by clicking the right arrow icon. In this case, Source Warehouse can choose from setting Item details.
:::

It is possible to [set up a default Warehouse](../../starting.md#documents-tab). In this case, the Warehouse Selection screen is skipped, and the Warehouse set as default is chosen automatically.

- The Customer Selection window will appear.

Clicking a row of a Customer picks it and leads to another window.

![Customer Selection](./media/customer-selection.png)

- The Document Details screen appears.

You can add an Item to the list in different ways.
![Document Details](./media/doc-details-01.png)
<details>
<summary>A. Add new Item from the Item's list.</summary>
<div>
Add an item manually:
![New Item List](./media/new-item-list.png)

Add an item by scanning its barcode:
You can scan an Item's barcode, which leads you directly to the quantity screen.
This is the barcode of non-managed item A00001.
![Barcode](./media/barcode.png)

Scanning the barcode leads directly to the quantity screen.
![Quantity Screen](./media/quantity-screen.png)
</div>
</details>

<details>
<summary>B. Add a SU to the item's list.</summary>
<div>
You can create a New SU or add an existing SU.
![Add SU](./media/add-su.png)
</div>
</details>

- There are items added in the Document Details screen:
![Document Details Added](./media/doc-det-added.png)

**Remarks screen**

You can add remarks, change document series, or set the supplier ref no on the remarks screen. Add a UDF to the previous screen or save the document.
    ![Remarks](./media/remarks-01.png)

- Message info about the created delivery no appears.

    ![Created Delivery](./media/delivery-created.png)

- The Delivery document is posted in SAP Business One.

    ![SAP Delivery](./media/sap-delivery-01.png)

---
