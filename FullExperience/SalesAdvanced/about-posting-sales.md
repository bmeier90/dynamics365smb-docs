---
title: "About Posting Sales"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "posting, about"
ms.assetid: 58c05508-2492-475e-a3e3-a763f81e7fe5
caps.latest.revision: 5
ms.author: "sgroespe"
manager: "terryaus"
translation.priority.ht: 
  - "da-dk"
  - "de-at"
  - "de-ch"
  - "de-de"
  - "en-au"
  - "en-ca"
  - "en-gb"
  - "en-in"
  - "en-nz"
  - "es-es"
  - "es-mx"
  - "fi-fi"
  - "fr-be"
  - "fr-ca"
  - "fr-ch"
  - "fr-fr"
  - "is-is"
  - "it-ch"
  - "it-it"
  - "nb-no"
  - "nl-be"
  - "nl-nl"
  - "ru-ru"
  - "sv-se"
---
# About Posting Sales
In the **Posting** group on a sales document, you can choose between the following posting functions:  
  
-   **Post**  
  
-   **Test Report**  
  
-   **Post and Send** for more information, see [How to: Set Up Document Sending Profiles](../Sales/how-to-set-up-document-sending-profiles.md).  
  
-   **Post and Print**  
  
-   **Post and Email** For more information, see [How to: Send Documents by Email](../BusinessFunctionality/IntegratingWithMicrosoftOffice/how-to-send-documents-by-email.md).  
  
-   **Post Batch**  
  
-   **Preview Posting** for more information, see [How to: Preview Posting Results](../WorkingWithDynamics/how-to-preview-posting-results.md).  
  
 When you have completed all the lines and entered all the information on the sales order, you can post it. This creates a shipment and an invoice.  
  
 When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.  
  
 For each sales order, a sales entry is created in the [\($ T\_17 G\/L Entry $\)](assetId:///2b5b8281-fbfa-4b7f-a154-a9ec61afadfe) table. An entry is also created in the customer's account in the [\($ T\_21 Cust. Ledger Entry $\)](../Topic/\($%20T_21%20Cust.%20Ledger%20Entry%20$\).md) table and a general ledger entry is created in the relevant receivables account. In addition, posting the order may result in a VAT entry and a general ledger entry for the discount amount. Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field in the **Sales & Receivables Setup** table.  
  
 For each sales order line, an item ledger entry will be created in the [\($ T\_32 Item Ledger Entry $\)](../Topic/\($%20T_32%20Item%20Ledger%20Entry%20$\).md) table \(if the sales lines contain item numbers\) or a general ledger entry will be created in the **G\/L Entry** table \(if the sales lines contain a general ledger account\). If your location is set up to use bins and you have set a bin code on the sales order line, a warehouse entry will be created in the [\($ T\_7312 Warehouse Entry $\)](../Topic/\($%20T_7312%20Warehouse%20Entry%20$\).md).  
  
 In addition to this, sales orders are always recorded in the [Sales Shipment Header](../Topic/\($%20T_110%20Sales%20Shipment%20Header%20$\).md) and [Sales Invoice Header](../Topic/\($%20T_112%20Sales%20Invoice%20Header%20$\).md) tables.  
  
> [!IMPORTANT]  
>  When you post an order, you can create both a shipment and an invoice. These can be done at the same time or independently.  
>   
>  You can also create a partial shipment and a partial invoice by completing the [\($ T\_37\_18 Qty. to Ship $\)](../Topic/\($%20T_37_18%20Qty.%20to%20Ship%20$\).md) or [\($ T\_37\_17 Qty. to Invoice $\)](../Topic/\($%20T_37_17%20Qty.%20to%20Invoice%20$\).md) fields on the individual sales order lines before you post. Note that you cannot create an invoice for something that is not shipped. That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.  
  
 When the posting is completed, the posted sales lines are removed from the order. A message tells you when the posting is completed. After this, you will be able to see the posted entries in the various windows that contain posted entries, such as **Cust. Ledger Entries**, **G\/L Entries**, **Item Ledger Entries**, **Warehouse Entries**, **Posted Sales Shipment**, and **Posted Sales Invoice**.  
  
## See Also  
 [\($ N\_42 Sales Order $\)](../Topic/\($%20N_42%20Sales%20Order%20$\).md)   
 [How to: Post Sales Orders](../Sales/how-to-post-sales-orders.md)   
 [\($ B\_296 Batch Post Sales Orders $\)](../Topic/\($%20B_296%20Batch%20Post%20Sales%20Orders%20$\).md)   
 [How to: Preview Posting Results](../WorkingWithDynamics/how-to-preview-posting-results.md)