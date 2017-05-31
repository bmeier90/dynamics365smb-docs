---
title: "How to: Use One VAT Code in Journals"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
ms.assetid: 4e6ce4e6-6d10-46d1-8e00-1388422c82bf
caps.latest.revision: 2
ms.author: "edupont"
translation.priority.ht: 
  - "nb-no"
---
# How to: Use One VAT Code in Journals
In Norway, you can use the feature one VAT code in a journal, so that you can post VAT by using a single field, **VAT Code**. After it is set up, the one VAT code is a quick way to fill in the commonly used VAT fields.  
  
 To set up the VAT code for purchase orders and sales orders, the corresponding VAT business posting groups and the VAT product posting groups have to be defined.  
  
 The VAT rate is calculated from the combination of VAT business posting groups, buyer information, and VAT product posting groups.  
  
### To create a VAT code  
  
1.  In the **Search** box, enter **VAT Codes**, and then choose the related link.  
  
2.  On the  **Home** tab, choose **New**.  
  
3.  Enter information in the **Code**, **General Posting Type**, and **Description** fields for each VAT code.  
  
4.  Choose the **OK** button to close the **VAT Codes** window.  
  
 The following procedure explains the VAT posting setup.  
  
### To set up VAT posting  
  
1.  In the **Search** box, enter **VAT Posting Setup**, and then choose the related link.  
  
2.  On the **Home** tab, choose **New**.  
  
3.  In the **\($ N\_473 VAT Posting Setup $\)** card, fill in the following fields:  
  
    -   **\($ T\_325\_1 VAT Business Posting Group $\)**  
  
    -   **\($ T\_325\_2 VAT Product Posting Group $\)**  
  
    -   **\($ T\_325\_13 VAT Identifier $\)**  
  
    -   **\($ T\_325\_4 VAT Percentage $\)**  
  
    -   **\($ T\_325\_7 Sales VAT Account $\)**  
  
    -   **\($ T\_325\_9 Purchase VAT Account $\)**  
  
4.  In the **\($ T\_325\_10606 VAT Code $\)** field, select a code from the list.  
  
 Now, when you post a document in the general journal and close it, the information specified in the **VAT Posting Setup** card is applied.  
  
 For example, the VAT rate posted in the journal is defined by the setup that you have specified in the **VAT Posting Setup** window.  
  
> [!NOTE]  
>  The **VAT Code** and the **Bal. VAT Code**  fields have been added to the journal. The **Bal. VAT Code** is the VAT code that is used to calculate the balancing account.  
>   
>  No changes are made to the posting.  
  
## See Also  
 [Norwegian VAT Codes](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/norwegian-vat-codes.md)