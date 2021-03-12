---
title: 存取拒絕郵件的疑難排解
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707945"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="87d99-102">在 Sharepoint/OneDrive 系統管理中心中存取拒絕郵件的疑難排解</span><span class="sxs-lookup"><span data-stu-id="87d99-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="87d99-103">如果您在嘗試流覽 Sharepoint/OneDrive 系統管理中心時收到「拒絕存取」訊息，請確定您已 [將授權指派給使用者](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。</span><span class="sxs-lookup"><span data-stu-id="87d99-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="87d99-104">如果使用者有授權，您也應確定已將其 [指派給系統管理員角色](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ，可存取系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="87d99-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="87d99-105">當使用者使用相同使用者主體名稱 (UPN) 進行刪除及重新建立時，也會發生此問題。</span><span class="sxs-lookup"><span data-stu-id="87d99-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="87d99-106">新帳戶是使用不同的 PUID (Passport 唯一識別碼) 值建立。</span><span class="sxs-lookup"><span data-stu-id="87d99-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="87d99-107">當使用者嘗試存取網站集合或其 OneDrive 時，使用者的 PUID 不正確。</span><span class="sxs-lookup"><span data-stu-id="87d99-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="87d99-108">第二個案例是以 Active Directory 組織單位 (OU) 進行目錄同步處理。</span><span class="sxs-lookup"><span data-stu-id="87d99-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="87d99-109">如果使用者已經登入 SharePoint，然後將其移至不同的 OU，並使用 SharePoint 進行 resynced，可能會發生此問題。</span><span class="sxs-lookup"><span data-stu-id="87d99-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="87d99-110">若要解決此問題，您應該使用本文中的步驟還原原始的 UPN，在 [Microsoft 365 中還原使用者](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="87d99-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="87d99-111">附注：如果您的 OneDrive 或 SharePoint 系統管理中心無法供之前有存取權的多個使用者使用，則可能會發生暫時的服務問題。</span><span class="sxs-lookup"><span data-stu-id="87d99-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="87d99-112">[檢查服務健康情況儀表板](https://portal.office.com/adminportal/home#/servicehealth)。</span><span class="sxs-lookup"><span data-stu-id="87d99-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


