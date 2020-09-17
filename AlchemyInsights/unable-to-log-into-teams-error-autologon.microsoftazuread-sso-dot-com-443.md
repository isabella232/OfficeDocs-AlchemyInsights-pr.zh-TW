---
title: 由於錯誤 autologon.microsoftazuread-sso.com:443，無法登入 Teams
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 649124db135805d8101b43dbead63860d36853ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799951"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="94c9d-102">由於錯誤 autologon.microsoftazuread-sso.com:443，無法登入 Teams</span><span class="sxs-lookup"><span data-stu-id="94c9d-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="94c9d-103">如果將無縫 SSO 啟用為 O365 驗證，則可能需要將 URL “autologon.microsoftazuread-sso.com” 新增至內部網路網站。</span><span class="sxs-lookup"><span data-stu-id="94c9d-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="94c9d-104">如果已將它新增到信任的網站，且正在使用無縫 SSO，應將它從信任的網站中移除。</span><span class="sxs-lookup"><span data-stu-id="94c9d-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="94c9d-105">請參閱[無縫 SSO 疑難排解檢查清單](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)。</span><span class="sxs-lookup"><span data-stu-id="94c9d-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="94c9d-106">請按照下列步驟，將 URL 新增至內部網路網站清單：</span><span class="sxs-lookup"><span data-stu-id="94c9d-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="94c9d-107">按一下 [開始]\*\*\*\* 按鈕來開啟 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="94c9d-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="94c9d-108">在 [搜尋] 方塊中，輸入 [Internet Explorer]，然後在結果清單中按一下 [Internet Explorer]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="94c9d-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="94c9d-109">按一下 [工具]\*\*\*\*，然後按一下 [網際網路選項]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="94c9d-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="94c9d-110">按一下 [安全性]\*\*\*\* 索引標籤。</span><span class="sxs-lookup"><span data-stu-id="94c9d-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="94c9d-111">現在，按一下 [本機內部網路網站]\*\*\*\* 然後按一下 [網站]\*\*\*\* 按鈕，然後按 [進階]\*\*\*\* 按鈕。</span><span class="sxs-lookup"><span data-stu-id="94c9d-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="94c9d-112">輸入網站 URL，然後按一下 [新增]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="94c9d-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="94c9d-113">完成後，按一下 [關閉]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="94c9d-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="94c9d-114">如需詳細資訊，請參閱[在 O365 中部署無縫 SSO 的文件](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (包含原則式程序，以在步驟 3 中將 URL 新增至內部網路網站)。</span><span class="sxs-lookup"><span data-stu-id="94c9d-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
