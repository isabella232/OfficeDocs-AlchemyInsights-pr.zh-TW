---
title: AIP：頁首及頁尾不會如預期顯示
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4541"
ms.openlocfilehash: 5f50fc1d38618017bca61b4e9290d9893983534e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821690"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="e9023-102">AIP：頁首及頁尾不會如預期顯示</span><span class="sxs-lookup"><span data-stu-id="e9023-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="e9023-103">如果您遇到無法如預期顯示視覺標記的問題，請查看下列指導方針：</span><span class="sxs-lookup"><span data-stu-id="e9023-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="e9023-104">請確認您已參閱 [[何時會套用視覺標記]](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)。</span><span class="sxs-lookup"><span data-stu-id="e9023-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="e9023-105">針對 Office 標籤，請參閱 [Office 365 何時會套用內容標記和加密](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)。</span><span class="sxs-lookup"><span data-stu-id="e9023-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="e9023-106">如果您想要移除現有的頁首/頁尾，請參閱 [從其他標籤解決方案移除頁首及頁尾](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)。</span><span class="sxs-lookup"><span data-stu-id="e9023-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="e9023-107">如果您仍會發生此問題，請收集 Azure 資訊保護用戶端記錄，並將匯出的記錄附加到此票證。</span><span class="sxs-lookup"><span data-stu-id="e9023-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="e9023-108">**匯出 Azure 資訊保護記錄**</span><span class="sxs-lookup"><span data-stu-id="e9023-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="e9023-109">在 Outlook 中開啟 Office 文件或建立新的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="e9023-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="e9023-110">按一下 [保護/敏感度]  >  [說明和意見反應]。</span><span class="sxs-lookup"><span data-stu-id="e9023-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="e9023-111">按一下 [匯出記錄]。</span><span class="sxs-lookup"><span data-stu-id="e9023-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="e9023-112">將記錄儲存到您選擇的位置，然後將它們附加到此服務要求。</span><span class="sxs-lookup"><span data-stu-id="e9023-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="e9023-113">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="e9023-113">For additional information, see:</span></span>

- <span data-ttu-id="e9023-114">[如何設定 Azure 資訊保護的視覺標記標籤](https://docs.microsoft.com/azure/information-protection/configure-policy-markings) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="e9023-114">[How to configure a label for visual markings for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)</span></span>
- [<span data-ttu-id="e9023-115">檢閱 Azure 資訊保護文件</span><span class="sxs-lookup"><span data-stu-id="e9023-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- <span data-ttu-id="e9023-116">[Azure 資訊保護需求](https://docs.microsoft.com/azure/information-protection/get-started/requirements) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="e9023-116">[Requirements for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span></span>
- [<span data-ttu-id="e9023-117">Azure 資訊保護需求快速入門教學課程</span><span class="sxs-lookup"><span data-stu-id="e9023-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="e9023-118">下載 Azure 資訊保護用戶端</span><span class="sxs-lookup"><span data-stu-id="e9023-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
