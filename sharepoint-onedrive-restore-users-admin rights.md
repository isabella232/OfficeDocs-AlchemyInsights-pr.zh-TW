---
title: 讓使用者能夠存取 SharePoint 和 OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715203"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="17332-102">讓使用者能夠存取 SharePoint 和 OneDrive</span><span class="sxs-lookup"><span data-stu-id="17332-102">Give users access to SharePoint and OneDrive</span></span>

<p><span data-ttu-id="17332-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">當使用者是刪除並重新建立具有相同使用者主體名稱 (UPN)，最常就會發生此問題。使用不同的 PUID （Passport 唯一識別碼） 值，會建立新的帳戶。當使用者嘗試存取網站集合或其 OneDrive 時，使用者會有不正確的 PUID。第二個案例牽涉到目錄同步處理與 Active Directory 組織單位 (OU)。如果使用者有已登入至 SharePoint]，然後會移至不同的 OU 和 resynced 與 SharePoint，否則可能會發生這個問題。</span></span><span class="sxs-lookup"><span data-stu-id="17332-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN). The new account is created by using a different PUID (Passport Unique ID) value. When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID. A second scenario involves directory synchronization with an Active Directory organizational unit (OU). If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span></span></p> <p><span data-ttu-id="17332-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">若要解決此問題，您應該可以還原原始的 UPN 與此文章中的步驟<a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">還原 Office 365 中的使用者。</a></span></span><span class="sxs-lookup"><span data-stu-id="17332-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">To resolve this issue you should restore the original UPN with the steps in the article, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">Restore a user in Office 365.</a></span></span></span></p> <p><span data-ttu-id="17332-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">完成此工作後，您可以確認使用者具有 OneDrive 網站系統管理員權限依照下列步驟以<a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">新增管理員的使用者的 onedrive。</a></span></span><span class="sxs-lookup"><span data-stu-id="17332-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">Add admin's for a user's OneDrive.</a></span></span></span></p> <p><span data-ttu-id="17332-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">如需有關權限層級的詳細資訊，請參閱此文章<a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">了解在 SharePoint 中的權限等級。</a>&nbsp;</span></span><span class="sxs-lookup"><span data-stu-id="17332-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on permission levels, see the article, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">Understanding permission levels in SharePoint.</a>&nbsp;</span></span></span></p>
