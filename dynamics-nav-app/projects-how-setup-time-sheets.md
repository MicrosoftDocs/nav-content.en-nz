---
title: 'How to: Set Up Timesheets'
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 6cbacce79ce185d6ed00ea8383259d1b28f9e11b
ms.contentlocale: en-nz
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-time-sheets"></a><span data-ttu-id="9768a-102">How to: Set Up Time Sheets</span><span class="sxs-lookup"><span data-stu-id="9768a-102">How to: Set Up Time Sheets</span></span>
<span data-ttu-id="9768a-103">Time sheets in Dynamics NAV handle time registration in weekly increments of seven days.</span><span class="sxs-lookup"><span data-stu-id="9768a-103">Time sheets in Dynamics NAV handle time registration in weekly increments of seven days.</span></span> <span data-ttu-id="9768a-104">You use them to track the time used on jobs, and you can use them to record simple resource time registration.</span><span class="sxs-lookup"><span data-stu-id="9768a-104">You use them to track the time used on jobs, and you can use them to record simple resource time registration.</span></span> <span data-ttu-id="9768a-105">Before you can use time sheets, you must specify how you want them to be set up and configured.</span><span class="sxs-lookup"><span data-stu-id="9768a-105">Before you can use time sheets, you must specify how you want them to be set up and configured.</span></span>

<span data-ttu-id="9768a-106">After you have set up how your organisation will use time sheets, you can specify if and how time sheets are approved.</span><span class="sxs-lookup"><span data-stu-id="9768a-106">After you have set up how your organization will use time sheets, you can specify if and how time sheets are approved.</span></span> <span data-ttu-id="9768a-107">Depending on the needs of your organisation, you can designate:</span><span class="sxs-lookup"><span data-stu-id="9768a-107">Depending on the needs of your organization, you can designate:</span></span>

- <span data-ttu-id="9768a-108">One or more users as the time sheet administrator and approver for all time sheets.</span><span class="sxs-lookup"><span data-stu-id="9768a-108">One or more users as the time sheet administrator and approver for all time sheets.</span></span>
- <span data-ttu-id="9768a-109">A time sheet approver for each resource.</span><span class="sxs-lookup"><span data-stu-id="9768a-109">A time sheet approver for each resource.</span></span>

<span data-ttu-id="9768a-110">When you have set up time sheets, you can create time sheets for resources, assign them to job planning lines, and post time sheet lines.</span><span class="sxs-lookup"><span data-stu-id="9768a-110">When you have set up time sheets, you can create time sheets for resources, assign them to job planning lines, and post time sheet lines.</span></span> <span data-ttu-id="9768a-111">For more information, see [How to: Use Time Sheets](projects-how-use-time-sheets.md).</span><span class="sxs-lookup"><span data-stu-id="9768a-111">For more information, see [How to: Use Time Sheets](projects-how-use-time-sheets.md).</span></span>

## <a name="to-set-up-general-information-for-time-sheets"></a><span data-ttu-id="9768a-112">To set up general information for time sheets</span><span class="sxs-lookup"><span data-stu-id="9768a-112">To set up general information for time sheets</span></span>  

1. <span data-ttu-id="9768a-113">In the top right corner, choose the **Search for Page or Report** icon, enter **Resources Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9768a-113">In the top right corner, choose the **Search for Page or Report** icon, enter **Resources Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9768a-114">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="9768a-114">Fill in the fields as necessary.</span></span> <span data-ttu-id="9768a-115">Choose a field to read a short description of the field or link to more information.</span><span class="sxs-lookup"><span data-stu-id="9768a-115">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="9768a-116">For the **Time Sheet by Job Approval** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="9768a-116">For the **Time Sheet by Job Approval** field, select one of the following options.</span></span>

|<span data-ttu-id="9768a-117">Option</span><span class="sxs-lookup"><span data-stu-id="9768a-117">Option</span></span> |<span data-ttu-id="9768a-118">Description</span><span class="sxs-lookup"><span data-stu-id="9768a-118">Description</span></span>|
|---|---|
|<span data-ttu-id="9768a-119">**Never**</span><span class="sxs-lookup"><span data-stu-id="9768a-119">**Never**</span></span>|<span data-ttu-id="9768a-120">The user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="9768a-120">The user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span>|
|<span data-ttu-id="9768a-121">**Always**</span><span class="sxs-lookup"><span data-stu-id="9768a-121">**Always**</span></span>|<span data-ttu-id="9768a-122">The user in the **Person Responsible** field on the job card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="9768a-122">The user in the **Person Responsible** field on the job card approves the time sheet.</span></span>|
|<span data-ttu-id="9768a-123">**Machine Only**´</span><span class="sxs-lookup"><span data-stu-id="9768a-123">**Machine Only**´</span></span>|<span data-ttu-id="9768a-124">If the machine time sheet is linked with a job, then the user in the **Person Responsible** field on the job card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="9768a-124">If the machine time sheet is linked with a job, then the user in the **Person Responsible** field on the job card approves the time sheet.</span></span> <span data-ttu-id="9768a-125">If the machine time sheet is linked with a resource, then the user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="9768a-125">If the machine time sheet is linked with a resource, then the user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span>

## <a name="to-assign-a-time-sheet-administrator"></a><span data-ttu-id="9768a-126">To assign a time sheet administrator</span><span class="sxs-lookup"><span data-stu-id="9768a-126">To assign a time sheet administrator</span></span>  

1. <span data-ttu-id="9768a-127">In the top right corner, choose the **Search for Page or Report** icon, enter **User Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9768a-127">In the top right corner, choose the **Search for Page or Report** icon, enter **User Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9768a-128">Add a new user, if the user list does not include the person who you want to be the time sheet administrator.</span><span class="sxs-lookup"><span data-stu-id="9768a-128">Add a new user, if the user list does not include the person who you want to be the time sheet administrator.</span></span> <span data-ttu-id="9768a-129">For more information, please contact your administrator.</span><span class="sxs-lookup"><span data-stu-id="9768a-129">For more information, please contact your administrator.</span></span>  
3. <span data-ttu-id="9768a-130">Select a user to be a time sheet administrator, and then select the **Time Sheet Admin.**</span><span class="sxs-lookup"><span data-stu-id="9768a-130">Select a user to be a time sheet administrator, and then select the **Time Sheet Admin.**</span></span> <span data-ttu-id="9768a-131">check box.</span><span class="sxs-lookup"><span data-stu-id="9768a-131">check box.</span></span>  

<span data-ttu-id="9768a-132">**Tip**: It is recommended that you designate only one user to be the time sheet administrator for a company.</span><span class="sxs-lookup"><span data-stu-id="9768a-132">**Tip**: It is recommended that you designate only one user to be the time sheet administrator for a company.</span></span> <span data-ttu-id="9768a-133">In the following procedure, you set up a time sheet owner and approver where the time sheet approver is assigned for each resource.</span><span class="sxs-lookup"><span data-stu-id="9768a-133">In the following procedure, you set up a time sheet owner and approver where the time sheet approver is assigned for each resource.</span></span>  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a><span data-ttu-id="9768a-134">To assign a time sheets owner and approver</span><span class="sxs-lookup"><span data-stu-id="9768a-134">To assign a time sheets owner and approver</span></span>  

1. <span data-ttu-id="9768a-135">In the top right corner, choose the **Search for Page or Report** icon, enter **Resources**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9768a-135">In the top right corner, choose the **Search for Page or Report** icon, enter **Resources**, and then choose the related link.</span></span>
2. <span data-ttu-id="9768a-136">Select the resource for which you want to set up the ability to use time sheets, and then select the **Use Time Sheet** check box.</span><span class="sxs-lookup"><span data-stu-id="9768a-136">Select the resource for which you want to set up the ability to use time sheets, and then select the **Use Time Sheet** check box.</span></span>  
3. <span data-ttu-id="9768a-137">In the **Time Sheet Owner User ID** field, enter the ID of the owner of the time sheet.</span><span class="sxs-lookup"><span data-stu-id="9768a-137">In the **Time Sheet Owner User ID** field, enter the ID of the owner of the time sheet.</span></span> <span data-ttu-id="9768a-138">The owner can enter time usage on a time sheet and submit it for approval.</span><span class="sxs-lookup"><span data-stu-id="9768a-138">The owner can enter time usage on a time sheet and submit it for approval.</span></span> <span data-ttu-id="9768a-139">In general, when the resource is a person, that person is also the owner.</span><span class="sxs-lookup"><span data-stu-id="9768a-139">In general, when the resource is a person, that person is also the owner.</span></span>  
4. <span data-ttu-id="9768a-140">In the **Time Sheet Approver User ID** field, enter the ID of the approver of the time sheet.</span><span class="sxs-lookup"><span data-stu-id="9768a-140">In the **Time Sheet Approver User ID** field, enter the ID of the approver of the time sheet.</span></span> <span data-ttu-id="9768a-141">The approver can approve, reject, or reopen a time sheet.</span><span class="sxs-lookup"><span data-stu-id="9768a-141">The approver can approve, reject, or reopen a time sheet.</span></span>  

<span data-ttu-id="9768a-142">**Note**: You cannot change the ID of the time sheet approver if there are time sheets that have not yet been processed and have the status of **Submitted** or **Open**.</span><span class="sxs-lookup"><span data-stu-id="9768a-142">**Note**: You cannot change the ID of the time sheet approver if there are time sheets that have not yet been processed and have the status of **Submitted** or **Open**.</span></span>

## <a name="see-also"></a><span data-ttu-id="9768a-143">See Also</span><span class="sxs-lookup"><span data-stu-id="9768a-143">See Also</span></span>
[<span data-ttu-id="9768a-144">Set Up Project Management</span><span class="sxs-lookup"><span data-stu-id="9768a-144">Set Up Project Management</span></span>](projects-setup-projects.md)  
[<span data-ttu-id="9768a-145">Manage Projects</span><span class="sxs-lookup"><span data-stu-id="9768a-145">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="9768a-146">Finance</span><span class="sxs-lookup"><span data-stu-id="9768a-146">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="9768a-147">[Manage Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="9768a-147">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="9768a-148">[Manage Sales](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="9768a-148">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="9768a-149">Work With Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="9768a-149">Work With Dynamics NAV</span></span>](ui-work-product.md)  

