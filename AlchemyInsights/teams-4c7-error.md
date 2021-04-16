---
title: 團隊4c7 錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786660"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="b4fb5-102">Microsoft 小組中的4c7 錯誤</span><span class="sxs-lookup"><span data-stu-id="b4fb5-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="b4fb5-103">發生此錯誤的原因是 Microsoft 小組需要表單驗證。</span><span class="sxs-lookup"><span data-stu-id="b4fb5-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="b4fb5-104">當您部署 Active Directory Federation Services (AD FS) 時，預設不會啟用內部網路的表單驗證。</span><span class="sxs-lookup"><span data-stu-id="b4fb5-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="b4fb5-105">如果 Windows 整合式驗證失敗，系統會提示您使用表單驗證登入。</span><span class="sxs-lookup"><span data-stu-id="b4fb5-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="b4fb5-106">若要解決此問題，請在具有 Active Directory 本機複本的電腦上，使用 AD FS Microsoft Management Console (MMC) 嵌入式管理單元來啟用表單驗證。</span><span class="sxs-lookup"><span data-stu-id="b4fb5-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="b4fb5-107">若要執行此動作，請依照下列步驟執行：</span><span class="sxs-lookup"><span data-stu-id="b4fb5-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="b4fb5-108">在功能窗格中，流覽至 **驗證原則**。</span><span class="sxs-lookup"><span data-stu-id="b4fb5-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="b4fb5-109">在詳細資料窗格的 [ **動作** ] 下，選取 [ **編輯全域主要驗證**]。</span><span class="sxs-lookup"><span data-stu-id="b4fb5-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="b4fb5-110">在 [ **內部** 網路] 索引標籤上，選取 [ **表單驗證**]。</span><span class="sxs-lookup"><span data-stu-id="b4fb5-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="b4fb5-111">選取 **[確定** ( ] 或 [套用) ]。</span><span class="sxs-lookup"><span data-stu-id="b4fb5-111">Select **OK** (or **Apply**).</span></span>