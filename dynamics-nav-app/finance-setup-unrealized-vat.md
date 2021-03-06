---
title: Setting Up Unrealized Value Added Tax
description: If you're using cash-based accounting, you can specify how to handle unrealised GST for sales and purchases.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cash, VAT, unrealized, cash-based
ms.date: 09/08/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f5786a79e8f12bd86b3d6f7ce53e0c698b19cef4
ms.contentlocale: en-nz
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-set-up-unrealized-vat-for-cash-based-accounting"></a>How to: Set Up Unrealised GST for Cash-Based Accounting
If you're using cash-based accounting methods, you can set up [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] to handle unrealized VAT.

## <a name="to-use-general-ledger-accounts-for-unrealized-vat"></a>To use general ledger accounts for unrealised GST
You can choose to have GST amounts calculated and posted to a temporary general ledger account when an invoice is posted, and then posted to the correct general ledger account and included in GST statements when the actual payment of the invoice is posted. Before you can do this, you must complete the GST posting setup.

To use accounts for unrealised GST, follow these steps:
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, and enter **General Ledger Setup**. 
2. On the **General Ledger Setup** page, on the **General** FastTab, choose **Show More**, and then choose the **Unrealized VAT** check box.
3. Close the page.
4. choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), and enter **VAT Posting Setup**. 
5. On the **VAT Posting Setup** page, choose the VAT posting group, and then choose **Edit**. 
6. In the **Unrealized VAT Type** field, choose an option to specify how to allocate payments to the invoice amount (excluding VAT) and the VAT amount itself, and how to transfer VAT amounts from the unrealized VAT account to the realized account. The following table describes the options.

| Option | Description |
| --- | --- |
| Blank | Choose this option if you don't want to use the unrealised GST feature. |
| Percentage | Payments covers both GST and the invoice amount in proportion to the payment's percentage of the remaining invoice amount. The paid GST amount is transferred from the unrealised GST account to the realised GST account. |
| First | Payments cover GST first and then invoice amounts. In this case, the amount transferred from the unrealised GST account to the GST account will equal the amount of the payment until the total GST has been paid. |
| Last | Payments cover the invoice amount first and then GST. In this case, no amount will be transferred from the unrealised GST account to the GST account until the total amount of the invoice, excluding GST, has been paid. |
| First (Fully Paid) | Payments will cover VAT first (like the _First_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid. |
| Last (Fully Paid) | Payments will cover invoice amount first (like the _Last_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid. |

6. In the **Sales VAT Unreal. Account** field, choose the account for unrealized sales VAT.

    > [!NOTE]  
>   The GST amount will be posted to this account, and stay there until the customer payment is posted. The amount is then transferred to the account for sales GST.
7. In the **Purch. VAT Unreal. Account** field, enter the general ledger count for unrealized purchase VAT.

    > [!NOTE]  
>   The GST amount will be posted to this account, and stay there until the customer payment is posted. The amount is then transferred to the account for sales GST.

## <a name="see-also"></a>See Also
[Setting Up Value Added Tax](finance-setup-vat.md)
