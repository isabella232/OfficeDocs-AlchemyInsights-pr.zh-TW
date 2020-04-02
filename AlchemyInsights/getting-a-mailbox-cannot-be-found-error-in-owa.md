---
title: 126在 OWA 中找不到信箱錯誤？
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: e061ad6b74b27e3f0d597586cb2c8e31b8fa5d23
ms.sourcegitcommit: 83c644c35c2700dc515f091c8f41f9c283b89967
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/02/2020
ms.locfileid: "43105230"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="801ac-102">在 web 上的 Outlook 中取得未找到信箱的錯誤？</span><span class="sxs-lookup"><span data-stu-id="801ac-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="801ac-103">如果您使用的是網頁型 Outlook，但找不到您要**的信箱**，表示您用來連線至網頁上的 outlook 的帳戶沒有 Exchange Online 授權，因此沒有信箱與帳戶相關聯。</span><span class="sxs-lookup"><span data-stu-id="801ac-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="801ac-104">您的系統管理員可以遵循下列步驟，將授權指派給您的帳戶：</span><span class="sxs-lookup"><span data-stu-id="801ac-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="801ac-105">開啟[Microsoft 365 系統管理中心](https://portal.office.com/adminportal/home#/homepage)，移至 [**使用者**] 區段下的 [作用中**使用者**]，然後選取看到錯誤的使用者。</span><span class="sxs-lookup"><span data-stu-id="801ac-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="801ac-106">在開啟的使用者頁面中，移至 [**授權與應用程式**] 區段中，選取適當的**位置**值，並指派包含 Exchange Online 的授權（展開授權以查看其詳細資料）。</span><span class="sxs-lookup"><span data-stu-id="801ac-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="801ac-107">完成後，按一下 [**儲存變更**]。</span><span class="sxs-lookup"><span data-stu-id="801ac-107">When you're finished, click **Save changes**.</span></span>
