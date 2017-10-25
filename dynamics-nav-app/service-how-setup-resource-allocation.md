---
title: Set Up Resource Allocation
description: Learn how the system can help ensure that you assign someone who has the skills required to provide a service.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: resource, skill, service, zones
ms.date: 08/22/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9ca6bb733eb0f7cf090551da7a6d5c7b5cd3216b
ms.contentlocale: en-nz
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-set-up-resource-allocation"></a><span data-ttu-id="abdfe-103">How to: Set Up Resource Allocation</span><span class="sxs-lookup"><span data-stu-id="abdfe-103">How to: Set Up Resource Allocation</span></span>
<span data-ttu-id="abdfe-104">To ensure that a service task is performed well, it's important to find a resource who is qualified to do the work.</span><span class="sxs-lookup"><span data-stu-id="abdfe-104">To ensure that a service task is performed well, it's important to find a resource who is qualified to do the work.</span></span> <span data-ttu-id="abdfe-105">You can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] so that it's easy to allocate someone who has the right skills for the job.</span><span class="sxs-lookup"><span data-stu-id="abdfe-105">You can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] so that it's easy to allocate someone who has the right skills for the job.</span></span> <span data-ttu-id="abdfe-106">In [!INCLUDE[d365fin](includes/d365fin_md.md)], we call this _resource allocation_.</span><span class="sxs-lookup"><span data-stu-id="abdfe-106">In [!INCLUDE[d365fin](includes/d365fin_md.md)], we call this _resource allocation_.</span></span> <span data-ttu-id="abdfe-107">You can allocate resources based on their skill, availability, or whether they are in the same service zone as the customer.</span><span class="sxs-lookup"><span data-stu-id="abdfe-107">You can allocate resources based on their skill, availability, or whether they are in the same service zone as the customer.</span></span> 

<span data-ttu-id="abdfe-108">To use resource allocation, you must set up:</span><span class="sxs-lookup"><span data-stu-id="abdfe-108">To use resource allocation, you must set up:</span></span>  
  
* <span data-ttu-id="abdfe-109">The skills required to repair and maintain service items.</span><span class="sxs-lookup"><span data-stu-id="abdfe-109">The skills required to repair and maintain service items.</span></span> <span data-ttu-id="abdfe-110">You assign these to service items and resources.</span><span class="sxs-lookup"><span data-stu-id="abdfe-110">You assign these to service items and resources.</span></span>  
* <span data-ttu-id="abdfe-111">Geographic regions, called zones, that you define for your market.</span><span class="sxs-lookup"><span data-stu-id="abdfe-111">Geographic regions, called zones, that you define for your market.</span></span> <span data-ttu-id="abdfe-112">For example, East, West, Central, and so on.</span><span class="sxs-lookup"><span data-stu-id="abdfe-112">For example, East, West, Central, and so on.</span></span> <span data-ttu-id="abdfe-113">You assign these to customers and resources.</span><span class="sxs-lookup"><span data-stu-id="abdfe-113">You assign these to customers and resources.</span></span>  
* <span data-ttu-id="abdfe-114">Whether to display resource skills and zones, and whether to display a warning if someone chooses unqualified resource, or a resource that is not in the customer zone.</span><span class="sxs-lookup"><span data-stu-id="abdfe-114">Whether to display resource skills and zones, and whether to display a warning if someone chooses unqualified resource, or a resource that is not in the customer zone.</span></span>  

## <a name="to-set-up-skills"></a><span data-ttu-id="abdfe-115">To set up skills</span><span class="sxs-lookup"><span data-stu-id="abdfe-115">To set up skills</span></span>
1. <span data-ttu-id="abdfe-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Skills**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="abdfe-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Skills**, and then choose the related link.</span></span>  
2. <span data-ttu-id="abdfe-117">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="abdfe-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-skills-to-service-items-and-resources"></a><span data-ttu-id="abdfe-118">To assign skills to service items and resources</span><span class="sxs-lookup"><span data-stu-id="abdfe-118">To assign skills to service items and resources</span></span>
1. <span data-ttu-id="abdfe-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Items** or **Resources**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="abdfe-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Items** or **Resources**, and then choose the related link.</span></span>  
2. <span data-ttu-id="abdfe-120">Open the card for the service item or resource, and then choose one of the following:</span><span class="sxs-lookup"><span data-stu-id="abdfe-120">Open the card for the service item or resource, and then choose one of the following:</span></span>  
  
    * <span data-ttu-id="abdfe-121">For service items, choose **Resource Skills**.</span><span class="sxs-lookup"><span data-stu-id="abdfe-121">For service items, choose **Resource Skills**.</span></span>  
    * <span data-ttu-id="abdfe-122">For resources, choose **Skills**.</span><span class="sxs-lookup"><span data-stu-id="abdfe-122">For resources, choose **Skills**.</span></span>  

## <a name="to-set-up-zones"></a><span data-ttu-id="abdfe-123">To set up zones</span><span class="sxs-lookup"><span data-stu-id="abdfe-123">To set up zones</span></span>
1. <span data-ttu-id="abdfe-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Zones**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="abdfe-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Zones**, and then choose the related link.</span></span>  
2. <span data-ttu-id="abdfe-125">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="abdfe-125">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-zones-to-customers-and-resources"></a><span data-ttu-id="abdfe-126">To assign zones to customers and resources</span><span class="sxs-lookup"><span data-stu-id="abdfe-126">To assign zones to customers and resources</span></span> 
1. <span data-ttu-id="abdfe-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers** or **Resources**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="abdfe-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers** or **Resources**, and then choose the related link.</span></span>  
2. <span data-ttu-id="abdfe-128">Open the card for the service item or resource, and then choose one of the following:</span><span class="sxs-lookup"><span data-stu-id="abdfe-128">Open the card for the service item or resource, and then choose one of the following:</span></span>  
  
    * <span data-ttu-id="abdfe-129">For customers, choose a zone in the **Service Zone Code** field.</span><span class="sxs-lookup"><span data-stu-id="abdfe-129">For customers, choose a zone in the **Service Zone Code** field.</span></span>  
    * <span data-ttu-id="abdfe-130">For resources, choose the **Service Zones** action.</span><span class="sxs-lookup"><span data-stu-id="abdfe-130">For resources, choose the **Service Zones** action.</span></span>  

## <a name="to-specify-what-to-show-when-a-resource-is-chosen"></a><span data-ttu-id="abdfe-131">To specify what to show when a resource is chosen</span><span class="sxs-lookup"><span data-stu-id="abdfe-131">To specify what to show when a resource is chosen</span></span>
1. <span data-ttu-id="abdfe-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="abdfe-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Setup**, and then choose the related link.</span></span> 
2. <span data-ttu-id="abdfe-133">In the **Resource Skills Option** field, choose one of the options described in the following table.</span><span class="sxs-lookup"><span data-stu-id="abdfe-133">In the **Resource Skills Option** field, choose one of the options described in the following table.</span></span>  
  
    |<span data-ttu-id="abdfe-134">**Option**</span><span class="sxs-lookup"><span data-stu-id="abdfe-134">**Option**</span></span>|<span data-ttu-id="abdfe-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="abdfe-135">**Description**</span></span>|  
    |------------|-------------|  
    |<span data-ttu-id="abdfe-136">Code Shown</span><span class="sxs-lookup"><span data-stu-id="abdfe-136">Code Shown</span></span> | <span data-ttu-id="abdfe-137">Displays the code only.</span><span class="sxs-lookup"><span data-stu-id="abdfe-137">Displays the code only.</span></span>|  
    |<span data-ttu-id="abdfe-138">Warning Displayed</span><span class="sxs-lookup"><span data-stu-id="abdfe-138">Warning Displayed</span></span> | <span data-ttu-id="abdfe-139">Shows the information and displays a warning if you choose a resource that is not qualified.</span><span class="sxs-lookup"><span data-stu-id="abdfe-139">Shows the information and displays a warning if you choose a resource that is not qualified.</span></span>|  
    |<span data-ttu-id="abdfe-140">Not Used</span><span class="sxs-lookup"><span data-stu-id="abdfe-140">Not Used</span></span> | <span data-ttu-id="abdfe-141">Does not show this information.</span><span class="sxs-lookup"><span data-stu-id="abdfe-141">Does not show this information.</span></span>|  

## <a name="to-update-resource-capacity"></a><span data-ttu-id="abdfe-142">To update resource capacity</span><span class="sxs-lookup"><span data-stu-id="abdfe-142">To update resource capacity</span></span>  
<span data-ttu-id="abdfe-143">You may need to change the capacity of resources.</span><span class="sxs-lookup"><span data-stu-id="abdfe-143">You may need to change the capacity of resources.</span></span>  
  
1. <span data-ttu-id="abdfe-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Capacity**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="abdfe-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Capacity**, and then choose the related link.</span></span>  
2. <span data-ttu-id="abdfe-145">Choose the resource, and then choose the **Set Capacity** action.</span><span class="sxs-lookup"><span data-stu-id="abdfe-145">Choose the resource, and then choose the **Set Capacity** action.</span></span>  
3. <span data-ttu-id="abdfe-146">Make the changes, and then choose **Update Capacity**.</span><span class="sxs-lookup"><span data-stu-id="abdfe-146">Make the changes, and then choose **Update Capacity**.</span></span>  

## <a name="to-update-skills-for-items-service-items-or-service-item-groups"></a><span data-ttu-id="abdfe-147">To update skills for items, service items, or service item groups</span><span class="sxs-lookup"><span data-stu-id="abdfe-147">To update skills for items, service items, or service item groups</span></span>
<span data-ttu-id="abdfe-148">If you want to change the skill codes assigned to items, for example from **PC** to **PCS**, you can do so either for an item, service item, or for all items in a service item group.</span><span class="sxs-lookup"><span data-stu-id="abdfe-148">If you want to change the skill codes assigned to items, for example from **PC** to **PCS**, you can do so either for an item, service item, or for all items in a service item group.</span></span>  
  
1. <span data-ttu-id="abdfe-149">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items** or **Service Item**, or **Service Item Group**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="abdfe-149">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items** or **Service Item**, or **Service Item Group**, and then choose the related link.</span></span>  
2. <span data-ttu-id="abdfe-150">Choose the entity to update, and then choose the **Resource Skills** action.</span><span class="sxs-lookup"><span data-stu-id="abdfe-150">Choose the entity to update, and then choose the **Resource Skills** action.</span></span>  
3. <span data-ttu-id="abdfe-151">On the line with the code to be changed, in the **Skill Code** field, choose the relevant skill code.</span><span class="sxs-lookup"><span data-stu-id="abdfe-151">On the line with the code to be changed, in the **Skill Code** field, choose the relevant skill code.</span></span>  
4.  <span data-ttu-id="abdfe-152">If the item has associated service items, a dialogue box opens with the following two options:</span><span class="sxs-lookup"><span data-stu-id="abdfe-152">If the item has associated service items, a dialog box opens with the following two options:</span></span>  
  
    * <span data-ttu-id="abdfe-153">Change the skill codes to the selected value: Select this option if you want to replace the old skill code with the new one on all the related service items.</span><span class="sxs-lookup"><span data-stu-id="abdfe-153">Change the skill codes to the selected value: Select this option if you want to replace the old skill code with the new one on all the related service items.</span></span>  
    * <span data-ttu-id="abdfe-154">Delete the skill codes or update their relation: Select this option if you want to change the skill code on this item only.</span><span class="sxs-lookup"><span data-stu-id="abdfe-154">Delete the skill codes or update their relation: Select this option if you want to change the skill code on this item only.</span></span> <span data-ttu-id="abdfe-155">The skill code on the related service items will be reassigned, that is, the **Assigned From** field will be updated.</span><span class="sxs-lookup"><span data-stu-id="abdfe-155">The skill code on the related service items will be reassigned, that is, the **Assigned From** field will be updated.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="abdfe-156">See Also</span><span class="sxs-lookup"><span data-stu-id="abdfe-156">See Also</span></span>
[<span data-ttu-id="abdfe-157">How to: Allocate Resources</span><span class="sxs-lookup"><span data-stu-id="abdfe-157">How to: Allocate Resources</span></span>](service-how-to-allocate-resources.md)  
[<span data-ttu-id="abdfe-158">How to: Set Up Work Hours and Service Hours</span><span class="sxs-lookup"><span data-stu-id="abdfe-158">How to: Set Up Work Hours and Service Hours</span></span>](service-how-setup-work-service-hours.md)  
[<span data-ttu-id="abdfe-159">How to: Set Up Fault Reporting</span><span class="sxs-lookup"><span data-stu-id="abdfe-159">How to: Set Up Fault Reporting</span></span>](service-how-setup-fault-reporting.md)  
[<span data-ttu-id="abdfe-160">How to: Set Up Codes for Standard Services</span><span class="sxs-lookup"><span data-stu-id="abdfe-160">How to: Set Up Codes for Standard Services</span></span>](service-how-setup-service-coding.md)  
 


