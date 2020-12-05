---
title: Microsoft Edge 中的 Azure 功能無法正常運作時要執行的動作
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576409"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="8f95c-102">Microsoft Edge 中的 Azure 功能無法正常運作時要執行的動作</span><span class="sxs-lookup"><span data-stu-id="8f95c-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="8f95c-103">Microsoft Edge 具有與安全性區域相關的 [已知問題](https://go.microsoft.com/fwlink/?linkid=2140608) ，而且可能會影響 Azure 使用者登入 Windows 系統管理中心的方式。</span><span class="sxs-lookup"><span data-stu-id="8f95c-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="8f95c-104">如果您在使用 Microsoft Edge Azure 功能時發生問題，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="8f95c-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="8f95c-105">在 [ **開始** ] 功能表中，搜尋 [ **網際網路選項** ]，然後選取。</span><span class="sxs-lookup"><span data-stu-id="8f95c-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="8f95c-106">在 [ **網際網路屬性** ] 對話方塊中，移至 [ **安全性** ] 索引標籤。</span><span class="sxs-lookup"><span data-stu-id="8f95c-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="8f95c-107">選取 [ **信任的網站** ] 區域，然後選取 [ **網站** ] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="8f95c-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="8f95c-108">在 [ **信任的網站** ] 對話方塊中，新增您的閘道 URL 以及 [https://login.microsoftonline.com](https://login.microsoftonline.com) 和 [https://login.live.com](https://login.live.com) ，然後選取 [ **關閉**]。</span><span class="sxs-lookup"><span data-stu-id="8f95c-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="8f95c-109">在 [ **網際網路屬性** ] 對話方塊中，移至 [ **隱私權** ] 索引標籤。</span><span class="sxs-lookup"><span data-stu-id="8f95c-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="8f95c-110">在 [ **彈出** 視窗封鎖程式] 區段中，選取 [ **設定**]。</span><span class="sxs-lookup"><span data-stu-id="8f95c-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="8f95c-111">在開啟的對話方塊中，新增您的閘道 URL 以及 [https://login.microsoftonline.com](https://login.microsoftonline.com) 和 [https://login.live.com](https://login.live.com) ，然後選取 [ **關閉**]。</span><span class="sxs-lookup"><span data-stu-id="8f95c-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
