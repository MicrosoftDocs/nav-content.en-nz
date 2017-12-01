---
title: How to Determine Sales Price by Cost Plus Percentage
description: Use the cost plus percentage function to set a sales price based on the cost of an item. The cost of the item can be calculated along with cost plus calculation. The discount will be based on this calculation.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 827217d1c5b0db6354d9c1f0036180c7e2157788
ms.contentlocale: en-nz
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-determine-sales-price-by-cost-plus-percentage"></a><span data-ttu-id="fef93-105">How to: Determine Sales Price by Cost Plus Percentage</span><span class="sxs-lookup"><span data-stu-id="fef93-105">How to: Determine Sales Price by Cost Plus Percentage</span></span>
<span data-ttu-id="fef93-106">Use the cost plus percentage function to set a sales price based on the cost of an item.</span><span class="sxs-lookup"><span data-stu-id="fef93-106">Use the cost plus percentage function to set a sales price based on the cost of an item.</span></span> <span data-ttu-id="fef93-107">The cost of the item can be calculated along with cost plus calculation.</span><span class="sxs-lookup"><span data-stu-id="fef93-107">The cost of the item can be calculated along with cost plus calculation.</span></span> <span data-ttu-id="fef93-108">The discount will be based on this calculation.</span><span class="sxs-lookup"><span data-stu-id="fef93-108">The discount will be based on this calculation.</span></span> <span data-ttu-id="fef93-109">This functionality eliminates the need for the use of spreadsheets in determining percentage discounts as they correspond to cost plus percentage.</span><span class="sxs-lookup"><span data-stu-id="fef93-109">This functionality eliminates the need for the use of spreadsheets in determining percentage discounts as they correspond to cost plus percentage.</span></span>  

## <a name="to-determine-sales-tax-by-cost-plus-percentage"></a><span data-ttu-id="fef93-110">To determine US sales tax by cost plus percentage</span><span class="sxs-lookup"><span data-stu-id="fef93-110">To determine sales tax by cost plus percentage</span></span>  

1.  <span data-ttu-id="fef93-111">Choose the **Receivables** action.</span><span class="sxs-lookup"><span data-stu-id="fef93-111">Choose the **Receivables** action.</span></span>  
3.  <span data-ttu-id="fef93-112">Choose the **Customers** action.</span><span class="sxs-lookup"><span data-stu-id="fef93-112">Choose the **Customers** action.</span></span>  
4.  <span data-ttu-id="fef93-113">Open the card for a relevant customer.</span><span class="sxs-lookup"><span data-stu-id="fef93-113">Open the card for a relevant customer.</span></span>  

     <span data-ttu-id="fef93-114">–or–</span><span class="sxs-lookup"><span data-stu-id="fef93-114">–or–</span></span>  

    <span data-ttu-id="fef93-115">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="fef93-115">Choose the **New** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="fef93-116">For a new customer, in the **No.**</span><span class="sxs-lookup"><span data-stu-id="fef93-116">For a new customer, in the **No.**</span></span> <span data-ttu-id="fef93-117">field, enter the customer number.</span><span class="sxs-lookup"><span data-stu-id="fef93-117">field, enter the customer number.</span></span>  

5.  <span data-ttu-id="fef93-118">To open the **Sales Prices** window, choose the **Prices** action.</span><span class="sxs-lookup"><span data-stu-id="fef93-118">To open the **Sales Prices** window, choose the **Prices** action.</span></span>  
6.  <span data-ttu-id="fef93-119">In the **General** section, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="fef93-119">In the **General** section, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="fef93-120">Field</span><span class="sxs-lookup"><span data-stu-id="fef93-120">Field</span></span>|<span data-ttu-id="fef93-121">Description</span><span class="sxs-lookup"><span data-stu-id="fef93-121">Description</span></span>|  
    |-----------|-----------------|  
    |<span data-ttu-id="fef93-122">**Sales Type Filter**</span><span class="sxs-lookup"><span data-stu-id="fef93-122">**Sales Type Filter**</span></span>|<span data-ttu-id="fef93-123">Select one of the following options:</span><span class="sxs-lookup"><span data-stu-id="fef93-123">Select one of the following options:</span></span><br /><br /> <span data-ttu-id="fef93-124">-   **Customer**</span><span class="sxs-lookup"><span data-stu-id="fef93-124">-   **Customer**</span></span><br /><span data-ttu-id="fef93-125">-   **Customer Price Group**</span><span class="sxs-lookup"><span data-stu-id="fef93-125">-   **Customer Price Group**</span></span><br /><span data-ttu-id="fef93-126">-   **All Customers**</span><span class="sxs-lookup"><span data-stu-id="fef93-126">-   **All Customers**</span></span><br /><span data-ttu-id="fef93-127">-   **Campaign**</span><span class="sxs-lookup"><span data-stu-id="fef93-127">-   **Campaign**</span></span><br /><span data-ttu-id="fef93-128">-   **None**</span><span class="sxs-lookup"><span data-stu-id="fef93-128">-   **None**</span></span>|  
    |<span data-ttu-id="fef93-129">**Sales Code Filter**</span><span class="sxs-lookup"><span data-stu-id="fef93-129">**Sales Code Filter**</span></span>|<span data-ttu-id="fef93-130">The sales code.</span><span class="sxs-lookup"><span data-stu-id="fef93-130">The sales code.</span></span>|  
    |<span data-ttu-id="fef93-131">**Item No. Filter**</span><span class="sxs-lookup"><span data-stu-id="fef93-131">**Item No. Filter**</span></span>|<span data-ttu-id="fef93-132">The item number.</span><span class="sxs-lookup"><span data-stu-id="fef93-132">The item number.</span></span>|  
    |<span data-ttu-id="fef93-133">**Starting Date Filter**</span><span class="sxs-lookup"><span data-stu-id="fef93-133">**Starting Date Filter**</span></span>|<span data-ttu-id="fef93-134">The starting date.</span><span class="sxs-lookup"><span data-stu-id="fef93-134">The starting date.</span></span>|  
    |<span data-ttu-id="fef93-135">**Currency Code Filter**</span><span class="sxs-lookup"><span data-stu-id="fef93-135">**Currency Code Filter**</span></span>|<span data-ttu-id="fef93-136">The currency code.</span><span class="sxs-lookup"><span data-stu-id="fef93-136">The currency code.</span></span>|  

7.  <span data-ttu-id="fef93-137">Enter information into the relevant fields.</span><span class="sxs-lookup"><span data-stu-id="fef93-137">Enter information into the relevant fields.</span></span>  
8.  <span data-ttu-id="fef93-138">To send the details to a recipient, choose the **Send To** action, and then select one of the following formats:</span><span class="sxs-lookup"><span data-stu-id="fef93-138">To send the details to a recipient, choose the **Send To** action, and then select one of the following formats:</span></span>  

    - <span data-ttu-id="fef93-139">**Recipient as Attachment**</span><span class="sxs-lookup"><span data-stu-id="fef93-139">**Recipient as Attachment**</span></span>  
    - <span data-ttu-id="fef93-140">**Microsoft Word**</span><span class="sxs-lookup"><span data-stu-id="fef93-140">**Microsoft Word**</span></span>  
    - <span data-ttu-id="fef93-141">**Microsoft Excel**</span><span class="sxs-lookup"><span data-stu-id="fef93-141">**Microsoft Excel**</span></span>  

9. <span data-ttu-id="fef93-142">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="fef93-142">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fef93-143">See Also</span><span class="sxs-lookup"><span data-stu-id="fef93-143">See Also</span></span>  
 [<span data-ttu-id="fef93-144">New Zealand Local Functionality</span><span class="sxs-lookup"><span data-stu-id="fef93-144">New Zealand Local Functionality</span></span>](new-zealand-local-functionality.md)

