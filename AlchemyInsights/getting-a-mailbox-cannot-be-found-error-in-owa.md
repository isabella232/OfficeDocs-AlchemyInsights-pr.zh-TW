---
title: 126在 OWA 中找不到信箱錯誤？
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426653"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="15cff-102">在 web 上的 Outlook 中取得未找到信箱的錯誤？</span><span class="sxs-lookup"><span data-stu-id="15cff-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="15cff-103">如果您使用的是網頁型 Outlook，但找不到您要 **的信箱** ，表示您用來連線至網頁上的 outlook 的帳戶沒有 Exchange Online 授權，因此沒有信箱與帳戶相關聯。</span><span class="sxs-lookup"><span data-stu-id="15cff-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="15cff-104">您的系統管理員可以遵循下列步驟，將授權指派給您的帳戶：</span><span class="sxs-lookup"><span data-stu-id="15cff-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="15cff-105">開啟 [Microsoft 365 系統管理中心](https://portal.office.com/adminportal/home#/homepage)，移至 [**使用者**] 區段下的 [作用中 **使用者**]，然後選取看到錯誤的使用者。</span><span class="sxs-lookup"><span data-stu-id="15cff-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="15cff-106">在開啟的使用者頁面中，移至 [ **授權與應用程式** ] 區段中，選取適當的 **位置** 值，並指派包含 Exchange Online (的授權，以查看其詳細資料) 。</span><span class="sxs-lookup"><span data-stu-id="15cff-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="15cff-107">完成後，按一下 [儲存變更 **]**。</span><span class="sxs-lookup"><span data-stu-id="15cff-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="15cff-108">在某些情況下，如果授權已指派給使用者帳戶，移除並重新指派授權可協助解決問題，並在系統中正確布建：</span><span class="sxs-lookup"><span data-stu-id="15cff-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="15cff-109">檢查您的 M365 Exchange Online (及其他，如果您有任何) 訂閱是目前的，且最近未到期。</span><span class="sxs-lookup"><span data-stu-id="15cff-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="15cff-110">確定您的訂閱尚未到期，且已將有效的授權指派給使用者帳戶後，就可能需要24小時的時間才能進行授權的布建，所以您可能需要等待您的問題解決。</span><span class="sxs-lookup"><span data-stu-id="15cff-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="15cff-111">如需詳細資訊，請參閱 [指派及管理授權](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)。</span><span class="sxs-lookup"><span data-stu-id="15cff-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>