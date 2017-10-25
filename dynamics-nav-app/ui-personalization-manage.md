---
title: Managing Personalisation as an Administrator
description: Learn how to customise the user interface to suit your way of working.
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e3d088c35efca4d62b7db1f0d44d5ef2958317d4
ms.contentlocale: en-nz
ms.lasthandoff: 10/16/2017

---
# <a name="managing-personalization-as-an-administrator"></a>Managing Personalisation as an Administrator
Users can personalise their workspace to suit their own preferences. As an administrator, you can control and manage personalisation by disabling the ability for users to personalise pages and clearing any page personalisations that users have made.

## <a name="disable-personalization-for-a-profile"></a>Disable personalisation for a profile
You can prevent all users that belong to a specific profile from being able to personalise their pages.
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.
2.  Select the profile in the list that you want to modify.
3.  Select the **Disable personalisation** check box, and then choose the **OK** button.

## <a name="clear-user-personalizations"></a>Clear user personalisations

Clearing page personalisation changes the page back to its original layout before any personalisation was made. There are two ways to clear the personalisations that users have made to pages: using the **Delete User Personalisation** page and using the **User Personalisation Card** page.

### <a name="clear-user-personalizations-by-using-the-delete-user-personalization-page"></a>Clear user personalisations by using the Delete User Personalisation page

The **Delete User Personalisation** page enables you to clear personalisation on a per-page, per-user basis.

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete User Personalisation**, and then choose the related link.

    The page lists all the pages that have been personalised and the user it belongs to.

    >[!NOTE]
    > A check mark in the **Legacy Personalisation** column indicates that the personalisation has been done strictly by using [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and/or it has been done in [!INCLUDE[nav_web_md](includes/nav_web_md.md)] prior to [!INCLUDE[navnow_md](includes/navnow_md.md)]. Users who try to personalise these pages by using the [!INCLUDE[nav_web_md](includes/nav_web_md.md)] are locked from doing so unless they choose to unlock the page. For more information, see [Why a page is locked from personalising](ui-personalization-locked.md).For more information about personalisation between the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and [!INCLUDE[nav_web_md](includes/nav_web_md.md)], see [Working with personalisation between the Dynamics NAV Windows and Web client](ui-personalization-overview.md#PersonalizationWinWeb).

2. Select the entry that you want to delete, and then choose the **Delete** action.

    The user will see the changes the next time they sign-in.

### <a name="clear-user-personalizations-by-using-the-user-personalization-card-page"></a>Clear user personalisations by using the User Personalisation Card page

The **User Personalisation Card** page enables you to clear the personalisation on all pages for specific user. This requires write permission to Table 2000000072 **Profile**.

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Personalisation**, and then choose the related link.

    The **User Personalisation** page lists all users who potentially have personalised pages. If you cannot find a user in the list, this means that they do not have any personalised pages.

2. Select the user from the list, and then choose the **Edit** action.

3.  On the **Actions** tab, choose **Clear Personalised Pages**.

    The user will see the changes the next time they sign-in.

## <a name="see-also"></a>See Also
[Personalisation Overview](ui-personalization-overview.md)  
[Personalising Your Workspace](ui-personalization-user.md)  
[Working with [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[How to: Change the Role Centre](change-role.md)  
