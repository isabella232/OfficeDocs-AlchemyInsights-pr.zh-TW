---
title: 刪除 SharePoint 根網站
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: d33029b6fe333b38cee7dba66ba4a5044248f174
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768379"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="964df-102">刪除 SharePoint 根網站</span><span class="sxs-lookup"><span data-stu-id="964df-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="964df-103">**不支援** 刪除 SharePoint 根網站。</span><span class="sxs-lookup"><span data-stu-id="964df-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="964df-104">如果根網站已遭刪除，則在嘗試存取網站時，使用者會遇到「404 找不到檔案」的錯誤。</span><span class="sxs-lookup"><span data-stu-id="964df-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="964df-105">若要解決此問題，請從新的 SharePoint 系統管理中心還原網站，方法是移至[已刪除的網站](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)頁面，選取根網站，然後按一下 [還原]。</span><span class="sxs-lookup"><span data-stu-id="964df-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="964df-106">在還原根網站之後，請不要刪除根網站，而是從新的 SharePoint 系統管理中心使用[取代網站](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)功能。</span><span class="sxs-lookup"><span data-stu-id="964df-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="964df-107">如需詳細資訊，請參閱[現代化您的根網站](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="964df-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>