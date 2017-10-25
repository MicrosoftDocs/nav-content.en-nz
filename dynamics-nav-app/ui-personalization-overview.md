---
title: Personalising Your Workspace - Overview
description: Learn how to customise the user interface to suit your way of working.
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 04334d3bb50b37b9643b848ca4f59b015f03ad04
ms.contentlocale: en-nz
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace---overview"></a>Personalising Your Workspace - Overview
You can customise, or *personalise*, your workspace to suit your work and preferences by changing the layout of pages so that they display only the information you need, where you need it. The personalisation changes that you make will only affect what you see, not what other users see.

You can personalise your workspace by using the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. The personlization changes that you make will also be seen in the [!INCLUDE[nav_phone_md](includes/nav_phone_md.md)] and [!INCLUDE[nav_web_md](includes/nav_phone_md.md)].
  
> [!NOTE]  
> The administrator in your company may have already customised your user interface to a role-specific layout for all users who have the same profile as you and use the same Role Centre. Personalisations that you make to your workspace are saved under your user account, so they will be preserved even if an administrator rolls out a new set of role-specific layouts in your company. For more information, see [Configuring the User Interface](admin-configure-user-interface.md).

## <a name="comparing-personalization-in-the-dynamics-nav-windows-and-web-clients"></a>Comparing personalisation in the Dynamics NAV Windows and Web clients
Depending on the page, you can personalise many parts of the user interface, such as what fields or columns are shown and where they are placed, what actions are included on the ribbon, and more. Many of these things you can do in both the Windows client and Web client. The following table provides an overview of the personalisation capabilities in each client.

|  Personalise  ||  Windows client  |  Web client  |
|---------------|-|------------------|--------------|
|Fields in FastTabs||||
||Add, move, remove |x|x|
||Show in collapsed header|x||
||Hide under **Show more fields** action|x||
|Lists or document lines ||||
||Add, move, remove columns  |x|x|
||Add, move, remove freeze pane  |x|x|
|FactBoxes|||
||Move, remove|x|x|
||Add|x||
||Add, move, remove fields|x|x|
|Cues||||
||Move, remove|x|x|
||Add |x||
|Charts||||
||Move, remove|x|x|
||Add|x| |
|Ribbon and actions||x||
|Navigation Pane||x||

Another difference is that when personalising by using the Windows client, you can have various personalised versions of the same page, based on different access points to the page. For example, the **Sales Orders** page personalised to look different when it is opened from the **Customer Card** page than when it is opened from the **Sales Order Processor Role Centre** page. When you personalise a page by using the Web client, there is only one personalised version per page, so the changes will be seen in the page no matter where you open it from.

##  <a name="PersonalizationWinWeb"></a>Working with personalisation between the Dynamics NAV Windows and Web client
Before you start personalising pages, it is important to understand how the personalisation between the Window client and Web client works. If you will only ever use either the Windows client or the Web client, this information is not so relevant. However, it becomes important if you begin to personalise pages using both clients or when transitioning from using the Windows client to using the Web client permanently.  

-   If you use the Windows client to personalise a specific page from the start, you will also see the personalisation changes to the page in the [!INCLUDE[nav_web_md](includes/nav_web_md.md)] as well.

-   As long as you continue to use the Windows client to personalise the page, any personalisation changes you make, will also take effect on the page in the Web client.

-   However, as soon as you start to personalise the page by using the Web client, the personalisation for that page becomes separate between the two clients, and you will have a personalised version for each client. In the Web client, the previous personalisations on the page are cleared, which means that the page will return to its original layout, and you will essentially start personalising the page from scratch. The previous personalisations in the Windows client are unchanged.

- From this point on, you will personalise the page in the Windows and Web client independent of each other, which means the page can potentially look different in each client. The Phone and Tablet clients will show the same page personalisations as the Web client.  

> [!Tip]  
>If you open the **Delete User Personalisation** page, you can see all the pages that have been personalised by each user. The **Legacy Personalisation** column gives you an indication as to whether the personalisation was done in the Windows client or Web client. If there is a check mark in the column, the personalisation was done in the Windows client (or in the Web client prior to [!INCLUDE[navnow_md](includes/navnow_md.md)]).

## <a name="see-also"></a>See Also
[Personalising Your Workspace in the Dynamics NAV Windows Client](ui-personalization-windows-client.md)  
[Personalising Your Workspace in the Dynamics NAV Web Client](ui-personalization-user.md)  
[Managing Personalisation](ui-personalization-manage.md)  
[Customising Dynamics NAV](ui-customizing-overview.md)  

