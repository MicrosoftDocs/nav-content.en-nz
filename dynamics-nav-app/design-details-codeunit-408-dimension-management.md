---
title: Design Details - Codeunit 408 Dimension Management
description: Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.
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
ms.openlocfilehash: aabc2ce0f52d4a551cf47ae0b82e3482936ddeab
ms.contentlocale: en-nz
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="23d11-103">Design Details: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="23d11-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="23d11-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span><span class="sxs-lookup"><span data-stu-id="23d11-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="23d11-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span><span class="sxs-lookup"><span data-stu-id="23d11-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="23d11-106">Many functions are deleted because there is no need for copying between dimension tables.</span><span class="sxs-lookup"><span data-stu-id="23d11-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="23d11-107">Modified Functions</span><span class="sxs-lookup"><span data-stu-id="23d11-107">Modified Functions</span></span>  

|<span data-ttu-id="23d11-108">Function Name</span><span class="sxs-lookup"><span data-stu-id="23d11-108">Function Name</span></span>|<span data-ttu-id="23d11-109">Modification Description</span><span class="sxs-lookup"><span data-stu-id="23d11-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="23d11-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="23d11-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="23d11-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span><span class="sxs-lookup"><span data-stu-id="23d11-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="23d11-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="23d11-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="23d11-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="23d11-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="23d11-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="23d11-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="23d11-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="23d11-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="23d11-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="23d11-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="23d11-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="23d11-117">CheckDimValueComb</span></span>|<span data-ttu-id="23d11-118">Delete.</span><span class="sxs-lookup"><span data-stu-id="23d11-118">Delete.</span></span> <span data-ttu-id="23d11-119">All usage should be changed to CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="23d11-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="23d11-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="23d11-120">GetDefaultDim</span></span>|<span data-ttu-id="23d11-121">Modify to return an integer Dimension Set ID instead of a set of records.</span><span class="sxs-lookup"><span data-stu-id="23d11-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="23d11-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="23d11-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="23d11-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="23d11-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="23d11-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="23d11-126">Modify to work with DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="23d11-127">Deleted Functions</span><span class="sxs-lookup"><span data-stu-id="23d11-127">Deleted Functions</span></span>  
 <span data-ttu-id="23d11-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span><span class="sxs-lookup"><span data-stu-id="23d11-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="23d11-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="23d11-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="23d11-130">If you have customisations that use one or more of the functions, you must upgrade that code accordingly.</span><span class="sxs-lookup"><span data-stu-id="23d11-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="23d11-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="23d11-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="23d11-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="23d11-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="23d11-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="23d11-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="23d11-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="23d11-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="23d11-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="23d11-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-136">InsertDocDim</span></span>  

 <span data-ttu-id="23d11-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="23d11-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="23d11-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="23d11-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="23d11-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="23d11-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="23d11-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="23d11-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="23d11-141">InsertServContractDim</span></span>  

 <span data-ttu-id="23d11-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="23d11-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="23d11-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="23d11-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="23d11-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-144">GetDocDim</span></span>  

 <span data-ttu-id="23d11-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-145">GetProdDocDim</span></span>  

 <span data-ttu-id="23d11-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="23d11-146">TypeToTableID1</span></span>  

 <span data-ttu-id="23d11-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="23d11-147">TypeToTableID2</span></span>  

 <span data-ttu-id="23d11-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="23d11-148">TypeToTableID3</span></span>  

 <span data-ttu-id="23d11-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="23d11-149">TypeToTableID4</span></span>  

 <span data-ttu-id="23d11-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="23d11-150">TypeToTableID5</span></span>  

 <span data-ttu-id="23d11-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="23d11-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-152">DeleteDocDim</span></span>  

 <span data-ttu-id="23d11-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="23d11-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="23d11-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="23d11-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="23d11-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="23d11-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="23d11-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="23d11-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="23d11-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="23d11-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="23d11-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-160">ShowDocDim</span></span>  

 <span data-ttu-id="23d11-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-161">SaveDocDim</span></span>  

 <span data-ttu-id="23d11-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="23d11-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="23d11-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="23d11-164">ShowTempDim</span></span>  

 <span data-ttu-id="23d11-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="23d11-165">SaveTempDim</span></span>  

 <span data-ttu-id="23d11-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="23d11-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="23d11-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="23d11-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="23d11-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="23d11-168">SaveServContractDim</span></span>  

 <span data-ttu-id="23d11-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="23d11-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="23d11-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="23d11-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="23d11-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="23d11-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="23d11-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="23d11-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="23d11-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="23d11-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="23d11-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="23d11-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="23d11-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="23d11-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="23d11-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="23d11-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="23d11-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="23d11-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="23d11-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="23d11-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="23d11-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="23d11-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="23d11-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="23d11-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="23d11-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="23d11-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="23d11-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="23d11-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="23d11-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="23d11-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="23d11-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="23d11-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="23d11-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="23d11-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="23d11-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="23d11-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="23d11-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="23d11-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="23d11-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="23d11-198">TestDimValue</span></span>  

 <span data-ttu-id="23d11-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="23d11-199">TestNewDimValue</span></span>  

 <span data-ttu-id="23d11-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="23d11-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="23d11-201">(Delete because the ItemBudgetDim Table is deleted.)</span><span class="sxs-lookup"><span data-stu-id="23d11-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="23d11-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="23d11-202">GetServContractDim</span></span>  

 <span data-ttu-id="23d11-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="23d11-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="23d11-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="23d11-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="23d11-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="23d11-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="23d11-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="23d11-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="23d11-207">See Also</span><span class="sxs-lookup"><span data-stu-id="23d11-207">See Also</span></span>
 <span data-ttu-id="23d11-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="23d11-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="23d11-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="23d11-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="23d11-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="23d11-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 <span data-ttu-id="23d11-211">[Design Details: Table Structure](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="23d11-211">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 [<span data-ttu-id="23d11-212">Design Details: Code Examples of Changed Patterns in Modifications</span><span class="sxs-lookup"><span data-stu-id="23d11-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)

