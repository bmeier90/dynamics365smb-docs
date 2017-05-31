---
title: "How to: Create VAT Reports"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
ms.assetid: 9afe60e3-7312-4875-91c0-cd76b0c3cef2
caps.latest.revision: 5
ms.author: "edupont"
translation.priority.ht: 
  - "de-de"
---
# How to: Create VAT Reports
You can configure different types of VAT reports based on requirements. Then, when you have to submit a VAT report, you can create it in the **\($ N\_740 VAT Report $\)** window and then export it in electronic format that conforms to the ELMA5 format requirements.  
  
### To create a VAT report  
  
1.  In the **Search** box, enter **VAT Report**, and then choose the related link.  
  
2.  Fill in the fields in the **General** FastTab, including the fields that are described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**\($ T\_740\_1 No. $\)**|Specify the report number.<br /><br /> Depending on the type of report, and the configuration in your company, you can use the automatically generated number, select a different number series, or enter a different number manually.|  
    |**\($ T\_740\_3 VAT Report Type $\)**|Select the appropriate VAT Report type. The default setting is  **Standard**. If the report is an update to an existing report, choose **Corrective**.|  
    |**\($ T\_740\_28 Trade Type $\)**|Specify the type of trade that the report is to describe. The default is **Sales**. Other options are **Purchases** or **Both**.|  
    |**\($ T\_740\_4 Start Date $\)**|Specify the start date of the report period.|  
    |**\($ T\_740\_5 End Date $\)**|Specify the end date of the report period.|  
    |**\($ T\_740\_29 EU Goods\/Services $\)**|Specify whether the report applies to **Goods**, **Services**, or both. The default is **Both**.|  
    |**\($ T\_740\_10 Report Period Type $\)**|Specify the time period that the report applies to:<br /><br /> -   Month<br />-   Quarter<br />-   Year<br />-   Bi\-Monthly|  
    |**\($ T\_740\_11 Report Period No. $\)**|Specify the number of the VAT period.|  
    |**\($ T\_740\_12 Report Year $\)**|Specify the year that the VAT report covers.|  
    |**\($ T\_740\_16 Processing Date $\)**|Specify the date that the VAT report is created.|  
  
3.  Fill in the fields in the **Sign\-off** FastTab, including the key fields that are described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**\($ T\_740\_51 Sign\-off Place $\)**|Specify the location where the VAT report was signed off.|  
    |**\($ T\_740\_52 Sign\-off Date $\)**|Specify the date that the VAT report has been signed off.|  
    |**\($ T\_740\_53 Signed by Employee No. $\)**|Specify the number of the employee who signed the VAT report from the lookup list.|  
    |**\($ T\_740\_54 Created by Employee No. $\)**|Specify the number of the employee who created the VAT report from the lookup list.|  
  
4.  Import the VAT ledger entries that must be included in the VAT report.  
  
     On the **Actions** tab, choose **Suggest Lines**.  
  
     This adds VAT entries to the window. For each line, in the **Amount** field, you can drill down to see the VAT ledger entries that are the source of the line.  
  
 After you create the VAT report, you have to submit it to the tax authorities.  
  
### To submit a VAT report  
  
1.  In the **VAT Report** window, on the **Actions** tab, in the **Functions** group, choose **Release**.  
  
2.  Confirm that you want to release the report.  
  
     [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] validates that the VAT report is set up correctly. If the validation fails, the errors are shown in the **\($ N\_745 VAT Report Error Log $\)** window so that you can make the appropriate changes. For example, an error displays if you try to release a standard VAT report but you have not yet added any lines to the report.  
  
     When you mark a VAT report as released, it becomes non\-editable. If you must change the report after marking it as released, you must first reopen it.  
  
3.  On the **Actions** tab, choose **Export** to create a VAT report of EU Sales List data in ELMA5 format. Save a copy of the report, which has the required name specified by ELMA5.  
  
     You can now submit the report to the tax authorities.  
  
4.  On the **Home** tab, choose **Mark as Submitted**.  
  
## See Also  
 [How to: Correct VAT Reports](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Germany/how-to-correct-vat-reports.md)   
 [How to: Set Up VAT Reports](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Germany/how-to-set-up-vat-reports.md)