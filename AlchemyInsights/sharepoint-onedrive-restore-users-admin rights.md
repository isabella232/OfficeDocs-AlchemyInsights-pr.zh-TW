---
title: 疑難排解 OneDrive 商務網站的拒絕存取郵件
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670607"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="111a4-102">疑難排解 OneDrive 商務網站的拒絕存取郵件</span><span class="sxs-lookup"><span data-stu-id="111a4-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="111a4-103">當使用者使用相同使用者主體名稱 (UPN) 進行刪除及重新建立時，最常發生此問題。</span><span class="sxs-lookup"><span data-stu-id="111a4-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="111a4-104">新帳戶是使用不同的 PUID (Passport 唯一識別碼) 值建立。</span><span class="sxs-lookup"><span data-stu-id="111a4-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="111a4-105">當使用者嘗試存取網站集合或其 OneDrive 時，使用者的 PUID 不正確。</span><span class="sxs-lookup"><span data-stu-id="111a4-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="111a4-106">第二個案例是以 Active Directory 組織單位 (OU) 進行目錄同步處理。</span><span class="sxs-lookup"><span data-stu-id="111a4-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="111a4-107">如果使用者已經登入 SharePoint，然後將其移至不同的 OU，並使用 SharePoint 進行 resynced，可能會發生此問題。</span><span class="sxs-lookup"><span data-stu-id="111a4-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="111a4-108">若要解決此問題，您應該使用本文中的步驟還原原始的 UPN，在 [Microsoft 365 中還原使用者](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="111a4-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="111a4-109">如果您無法還原原始使用者，您應該使用這些步驟從 OneDrive 網站移除舊的使用者，並 [從 [使用者資訊] 清單中移除使用者]()。</span><span class="sxs-lookup"><span data-stu-id="111a4-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="111a4-110">完成之後，您可以依照下列步驟，確認使用者對 OneDrive 網站具有系統管理員許可權： [針對使用者的 OneDrive 新增系統管理員許可權。](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="111a4-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="111a4-111">如需許可權等級的詳細資訊，請參閱 [瞭解 SharePoint 中的許可權等級](https://docs.microsoft.com/sharepoint/understanding-permission-levels)一文。</span><span class="sxs-lookup"><span data-stu-id="111a4-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
