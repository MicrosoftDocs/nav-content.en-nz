---
title: How to work With GST on Sales and Purchases
description: This topic describes how perform tasks such as correcting posted VAT. In EU countries/regions, every sales and purchase transaction is subject to VAT calculations. This topic describes how.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: VAT, sales, purchases,
ms.date: 09/08/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 4a639b0da8e7f06f4120c89e75121edd324e0bfd
ms.contentlocale: en-nz
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-work-with-vat-on-sales-and-purchases"></a>How to: Work with GST on Sales and Purchases
If your country or region requires you to calculate value-added tax (VAT) on sales and purchase transactions so that you can report the amounts to a tax authority, you can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to calculate VAT automatically on sales and purchase documents. For more information, see [Setting Up to Calculations and Posting Methods for Value-Added Tax] (finance-setup-vat.md).

There are, however, some GST-related tasks that you can do manually. For example, you might need to correct a posted amount if you discover that a vendor uses a different rounding method.

## <a name="calculating-and-displaying-vat-amounts-in-sales-and-purchase-documents"></a>Calculating and Displaying GST Amounts in Sales and Purchase Documents  
You can calculate and display GST amounts in sales and purchase documents differently, depending on the type of customer or vendor that you are dealing with. You can also override the calculated GST amount to match the GST amount calculated by your vendor on a given transaction.  

### <a name="unit-price-and-line-amount-includingexcluding-vat-on-sales-documents"></a>Unit Price and Line Amount Including/Excluding GST on sales documents  
When you choose an item number in the **No.** field on a sales document, [!INCLUDE[d365fin](includes/d365fin_md.md)] fills in the **Unit Price** field. The unit price comes from either the **Item** card or the item prices allowed for the item and customer. [!INCLUDE[d365fin](includes/d365fin_md.md)]calculates the **Line Amount** when you enter a quantity for the line.  

If you are selling to retail consumers, you may want prices on sales documents to include GST. To do this, choose the **Prices Including GST** check box on the document.  

### <a name="including-or-excluding-vat-on-prices"></a>Including or excluding GST on prices
If the **Prices Including GST** check box is chosen on a sales document, the **Unit Price** and **Line Amount** fields include GST, and the field names will also reflect this. By default, GST is not included in these fields.  

If the field is not selected, the program will fill in the **Unit Price** and **Line Amount** field excluding GST and the field names will reflect this.  

You can set up the default setting of the **Prices Including GST** for all sales documents for a customer in the **Prices Including GST** field on the **Customer** card. You can also set up item prices to include or exclude GST. Normally, item prices contained in the Item Card will be the price excluding GST. The program uses the information from the **Price Includes GST** field on the **Item** card to determine the unit price amount for sales documents.  

The following table provides an overview of how the program calculates the unit price amounts for a sales document when you have not set up prices in the **Sales Prices** window:  

|**Price Includes GST field on Item Card**|**Prices Including GST field in Sales Header**|**Action Performed**|  
|-----------------------------------------------|----------------------------------------------------|--------------------------|  
|No check mark|No check mark|The **Unit Price** on the Item Card is copied to **Unit Price Excl. GST** field on the sales lines.|  
|No check mark|Check mark|The program calculates the GST amount per unit and adds to the **Unit Price** on the Item Card. This total Unit Price is then entered in the **Unit Price Incl. GST field** on the sales lines.|  
|Check mark|No check mark|The program calculates the GST amount included in the **Unit Price** on the Item Card using the GST% related to the GST Bus. Posting Gr. (Price) and the GST Prod. Posting Group combination. The **Unit Price** on the Item Card, reduced by the GST amount, is then entered in the **Unit Price Excl. GST** field in the sales lines.|  
|Check mark|Check mark|The **Unit Price** on the Item Card is copied to **Unit Price Incl. GST** field on the sales lines.|

## <a name="correcting-vat-amounts-manually-in-sales-and-purchase-documents"></a>Correcting GST Amounts Manually in Sales and Purchase Documents  
You can make corrections to posted GST entries. This allows you to change the total sales or purchase GST amounts without changing the GST base. You may need to do this, for example, if you receive an invoice from a vendor that has calculated GST incorrectly.  

Although you may have set up one or more combinations to handle import GST, you must set up at least one GST product posting group. For example, you can name it **CORRECT** for correction purposes, unless you can use the same general ledger account in the **Purchase GST Account** field on the GST posting setup line. For more information, see [Setting Up to Calculations and Posting Methods for Value-Added Tax](finance-setup-vat.md).

If a payment discount has been calculated on the basis of an invoice amount that includes GST, you revert the payment discount part of the GST amount when the payment discount is granted. Note that you must activate the **Adjust for Payments Disc.** field in both the general ledger setup in general and the GST posting setup for specific combinations of a GST business posting group and a GST product posting group.  

#### <a name="to-manually-enter-vat-in-sales-documents"></a>To manually enter GST in sales documents  
1. On the **General Ledger Setup** page, specify a **Max. GST Difference Allowed** between the amount calculated by the program and the manual amount.  
2. On the **Sales & Receivables Setup** page, place a check mark in the **Allow Vat Difference** field.  

#### <a name="to-adjust-vat-for-a-sales-document"></a>To adjust GST for a sales document  
1. Open the relevant sales order.  
2. Choose the **Statistics** action.  
3. Choose the **Invoicing** FastTab.  
  
    > [!NOTE]  
    >  The total GST amount for the invoice, grouped by GST identifier, is displayed in the lines. You can manually adjust the amount in the **GST Amount** field on the lines for each GST identifier. When you modify the **GST Amount** field, the program checks to ensure that you have not changed the GST by more than the amount you have specified as the maximum difference allowed. If the amount is outside the range of the **Max. GST Difference Allowed**, a warning will be displayed stating the maximum allowed difference. You will be unable to proceed until the amount is adjusted to within the acceptable parameters. Choose **OK** and enter another **GST Amount** that is within the allowed range. If the GST difference is equal to or lower than the maximum allowed, the GST will be divided proportionally among the document lines that have the same GST identifier.  

## <a name="calculating-vat-manually-using-journals"></a>Calculating GST Manually Using Journals  
You can also adjust GST amounts in general, sales, and purchase journals. For example, you might need to do this when you enter a vendor invoice in your journal and there is a difference between the GST amount that [!INCLUDE[d365fin](includes/d365fin_md.md)] calculated and the GST amount on the vendor's invoice.  

#### <a name="before-you-manually-enter-vat-on-a-general-journal"></a>Before you manually enter GST on a general journal  
1. On the **General Ledger Setup** page, specify a **Max. GST Difference Allowed** between the amount calculated by the program and the manual amount.  
2. On the **General Journal Templates** page, choose the **Allow GST Difference** check box for the relevant journal.  

#### <a name="before-you-manually-enter-vat-on-sales-and-purchase-journals"></a>Before you manually enter GST on sales and purchase journals  
1. On the **Purchases & Payables Setup** page, choose the **Allow VAT Difference** check box.  
2. After you complete the setup described above, you can adjust the **GST Amount** field on the general journal line, or the **Bal. GST Amount** field on the sales or purchase journal line. [!INCLUDE[d365fin](includes/d365fin_md.md)] will check that the difference is not greater than the specified maximum.  
  
    > [!NOTE]  
    > If the difference is greater, a warning will be displayed stating the maximum allowed difference. To continue, you must adjust the amount. Choose **OK** and then enter an amount that is within the allowed range. If the GST difference is equal to or lower than the maximum allowed, [!INCLUDE[d365fin](includes/d365fin_md.md)] will show the difference in the **GST Difference** field.  

## <a name="to-post-import-vat-with-purchase-invoices"></a>To post import GST with purchase invoices
Instead of using a general journal to post an import GST invoice, you can use a purchase invoice.  

### <a name="to-set-up-purchasing-for-posting-import-vat-invoices"></a>To set up purchasing for posting import GST invoices  
1. Set up a vendor card for the import authority that sends you the import GST invoice. The **Gen. Bus. Posting Group** and **GST Bus. Posting Group** must be set up in the same way as the general ledger account for the import GST.  
2. Create a **Gen. Product Posting Group** for the import GST and set up an import GST **Def. GST Product Posting Group** for the related **Gen. Product Posting Group**.  
3. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.  
4. Select the import GST general ledger account, and then on the **Home** tab, in the **Manage** group, choose **Edit**.  
5. On the **Posting** FastTab, select the **Gen. Prod. Posting Group** setup for import GST. [!INCLUDE[d365fin](includes/d365fin_md.md)] automatically fills in the **GST Prod. Posting Group** field.  
6. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Posting Setup**, and then choose the related link.  
7. Create a combination of the **Gen. Bus. Posting Group** for the GST authority and the **Gen. Prod. Posting Group** for import GST. For this new combination, in the **Purchase Account** field, choose the import GST general ledger account.  

### <a name="to-create-a-new-invoice-for-the-import-authority-vendor-once-you-have-completed-the-setup"></a>To create a new invoice for the import authority vendor once you have completed the setup  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.  
2. Create a new purchase invoice.  
3. In the **Buy-from Vendor No.** field, choose the import authority vendor, and then choose the **OK** button.  
4. In the purchase line, in the **Type** field, choose **G/L Account**, and in the **No.** field, choose the import GST general ledger account.  
5. In the **Quantity** field, type **1**.  
6. In the **Direct Unit Cost Excl. GST** field, specify the GST amount.  
7. Post the invoice.  

## <a name="to-process-certificates-of-supply"></a>To process certificates of supply
When you sell goods to a customer in another EU country/region, you must send the customer a certificate of supply that the customer must sign and return to you. The following procedures are for processing certificates of supply for sales shipments, but the same steps apply for service shipments of items, and return shipments to vendors.  

### <a name="to-view-certificate-of-supply-details"></a>To view certificate of supply details  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Shipments**, and then choose the related link.  
2. Choose the relevant sales shipment to a customer in another EU country/region.  
3. Choose **Certificate of Supply Details**.  
4. By default, if the **Certificate of Supply Required** check box is selected for GST Posting Group setup for the customer, the **Status** field is set to **Required**. You can update the field to indicate whether the customer has returned the certificate.  

    > [!Note]  
    >  If the GST Posting Group setup does not have the **Certificate of Supply Required** check box selected, then a record is created and the **Status** field is set to **Not Applicable**. You can update the field to reflect the correct status information. You can manually change the status from **Not Applicable** to **Required**, and from **Required** to **Not Applicable** as needed.  

   When you update the **Status** field to **Required**, **Received**, or **Not Received**, a certificate is created.  
  
    > [!TIP]  
    >  You can use the **Certificates of Supply** window to get a view of the status of all posted shipments for which a certificate of supply has been created.  

5. Choose **Print Certificate of Supply**.  
  
    > [!Note]  
    >  You can preview or print the document. When you choose **Print Certificate of Supply** and print the document, the **Printed** check box is automatically selected. In addition, if not already specified, the status of the certificate is updated to **Required**. If needed, you include the printed certificate with the shipment.  

### <a name="to-print-a-certificate-of-supply"></a>To print a certificate of supply  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Shipments**, and then choose the related link.  
2. Choose the relevant sales shipment to a customer in another EU country/region.  
3. Choose the **Print Certificate of Supply** action.  

    > [!NOTE]  
    >  Alternatively, you can print a certificate from the **Certificate of Supply** page.  

4. To include information from the lines on the shipment document in the certificate, select the **Print Line Details** check box.  
5. Choose the **Create Certificates of Supply if Not Already Created** check box to have [!INCLUDE[d365fin](includes/d365fin_md.md)] create certificates for posted shipments that do not have one at the moment of execution. When you choose the check box, new certificates will be created for all posted shipments that do not have certificates within the selected range.  
6. By default, the filter settings are for the shipment document that you have selected. Fill in the filter information to select a specific certificate of supply that you want to print.  
7. On the **Certificate of Supply** page, choose the **Print** action to print the report, or choose the **Preview** action to view it on the screen.  

    > [!Note]  
    > The **Certificate of Supply Status** field and the **Printed** field are updated for the shipment in the **Certificates of Supply** page.  

8. Send the printed certificate of supply to the customer for signature.  

### <a name="to-update-the-status-of-a-certificate-of-supply-for-a-shipment"></a>To update the status of a certificate of supply for a shipment  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Shipments**, and then choose the related link.  
2. Choose the relevant sales shipment to a customer in another EU country/region.  
3. In the **Status** field, choose the relevant option.  

   If the customer has returned the signed certificate of supply, choose **Received**. The **Receipt Date** field is updated. By default, the receipt date is set to the current work date.  

   You can modify the date to reflect the date that you received the customer's signed certificate of supply. You can also add a link to the signed certificate using standard [!INCLUDE[d365fin](includes/d365fin_md.md)] linking.  

   If the customer does not return the signed certificate of supply, choose **Not Received**. You must then send the customer a new invoice that includes GST, because the original invoice will not be accepted by the tax authority.  

To view a group of certificates, you start from the **Certificates of Supply** window, and then update the information about the status of outstanding certificates as you receive them back from your customers. This can be useful when you want to search for all certificates that have a certain status, for example, **Required**, for which you want to update their status to **Not Received**.  

### <a name="to-update-the-status-of-a-group-of-certificates-of-supply"></a>To update the status of a group of certificates of supply  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Certificates of Supply**, and choose the related link.  
2. Filter the **Status** field to the value that you want in order to create the list of certificates that you want to manage.  
3. To update the status information, choose **Edit List**.  
4. In the **Status** field, choose the relevant option.  

   If the customer has returned the signed certificate of supply, choose **Received**. The **Receipt Date** field is updated. By default, the receipt date is set to the current work date.  

   You can modify the date to reflect the date that you received the signed the certificate of supply. You can also add a link to the signed certificate using standard [!INCLUDE[d365fin](includes/d365fin_md.md)] document linking.  

    > [!NOTE]  
    >  You cannot create a new certificate of supply in the **Certificate of Supply** window when you navigate to it using this procedure. To create a certificate for a shipment that was not set up to require one, open the posted sales shipment, and use either of two procedures described above:  
    >   
    > * To manually create a certificate of supply certificate  
    > * To print a certificate of supply.

## <a name="see-also"></a>See Also  
[Setting Up to Calculations and Posting Methods for Value-Added Tax](finance-setup-vat.md)   
[How To: Report GST to a Tax Authority](finance-how-report-vat.md)   

