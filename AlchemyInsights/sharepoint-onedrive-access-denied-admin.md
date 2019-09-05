---
title: 針對 「 拒絕存取 」 訊息進行疑難排解
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751267"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="4f1a0-102">疑難排解 Sharepoint/OneDrive 系統管理中心中的 「 拒絕存取 」 訊息</span><span class="sxs-lookup"><span data-stu-id="4f1a0-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="4f1a0-103">如果您會收到拒絕存取訊息嘗試瀏覽至 Sharepoint/OneDrive 系統管理中心時，請確定該您[指派授權給使用者](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)。</span><span class="sxs-lookup"><span data-stu-id="4f1a0-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="4f1a0-104">如果使用者擁有授權，您也應該要確定他們已[指派給系統管理員角色](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)可以存取系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="4f1a0-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="4f1a0-105">當使用者是刪除並重新建立具有相同使用者主體名稱 (UPN)，也會發生這個問題。</span><span class="sxs-lookup"><span data-stu-id="4f1a0-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4f1a0-106">使用不同的 PUID （Passport 唯一識別碼） 值，會建立新的帳戶。</span><span class="sxs-lookup"><span data-stu-id="4f1a0-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4f1a0-107">當使用者嘗試存取網站集合或其 OneDrive 時，使用者會有不正確的 PUID。</span><span class="sxs-lookup"><span data-stu-id="4f1a0-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4f1a0-108">第二個案例牽涉到目錄同步處理與 Active Directory 組織單位 (OU)。</span><span class="sxs-lookup"><span data-stu-id="4f1a0-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4f1a0-109">如果使用者有已登入至 SharePoint]，然後會移至不同的 OU 和 resynced 與 SharePoint，否則可能會發生這個問題。</span><span class="sxs-lookup"><span data-stu-id="4f1a0-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="4f1a0-110">若要解決此問題，您應還原原始的 UPN 與在文章中，[將還原的使用者在 Office 365 中](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)的步驟。</span><span class="sxs-lookup"><span data-stu-id="4f1a0-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="4f1a0-111">附註： 如果無法使用先前持有存取的多個使用者的 OneDrive 或 SharePoint 系統管理員中心，有可能是暫時的服務問題。</span><span class="sxs-lookup"><span data-stu-id="4f1a0-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="4f1a0-112">[檢查服務健康狀況儀表板](https://portal.office.com/adminportal/home#/servicehealth)。</span><span class="sxs-lookup"><span data-stu-id="4f1a0-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


