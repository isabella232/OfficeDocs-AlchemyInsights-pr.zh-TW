---
title: AIP：頁首及頁尾不會如預期顯示
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
- "9002266"
- "4541"
ms.openlocfilehash: 811a48587272776c8ece5e654a921c15cf52af5f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696539"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="4dd5d-102">AIP：頁首及頁尾不會如預期顯示</span><span class="sxs-lookup"><span data-stu-id="4dd5d-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="4dd5d-103">如果您遇到無法如預期顯示視覺標記的問題，請查看下列指導方針：</span><span class="sxs-lookup"><span data-stu-id="4dd5d-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="4dd5d-104">請確認您已參閱 [[何時會套用視覺標記]](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)。</span><span class="sxs-lookup"><span data-stu-id="4dd5d-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="4dd5d-105">針對 Office 標籤，請參閱 [Office 365 何時會套用內容標記和加密](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)。</span><span class="sxs-lookup"><span data-stu-id="4dd5d-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="4dd5d-106">如果您想要移除現有的頁首/頁尾，請參閱 [從其他標籤解決方案移除頁首及頁尾](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)。</span><span class="sxs-lookup"><span data-stu-id="4dd5d-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="4dd5d-107">如果您仍會發生此問題，請收集 Azure 資訊保護用戶端記錄，並將匯出的記錄附加到此票證。</span><span class="sxs-lookup"><span data-stu-id="4dd5d-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="4dd5d-108">**匯出 Azure 資訊保護記錄**</span><span class="sxs-lookup"><span data-stu-id="4dd5d-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="4dd5d-109">在 Outlook 中開啟 Office 文件或建立新的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="4dd5d-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="4dd5d-110">按一下 [保護/敏感度]\*\*\*\*  >  [說明和意見反應]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="4dd5d-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="4dd5d-111">按一下 [匯出記錄]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="4dd5d-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="4dd5d-112">將記錄儲存到您選擇的位置，然後將它們附加到此服務要求。</span><span class="sxs-lookup"><span data-stu-id="4dd5d-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="4dd5d-113">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="4dd5d-113">For additional information, see:</span></span>

- <span data-ttu-id="4dd5d-114">[如何設定 Azure 資訊保護的視覺標記標籤](https://docs.microsoft.com/azure/information-protection/configure-policy-markings) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="4dd5d-114">[How to configure a label for visual markings for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)</span></span>
- [<span data-ttu-id="4dd5d-115">檢閱 Azure 資訊保護文件</span><span class="sxs-lookup"><span data-stu-id="4dd5d-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- <span data-ttu-id="4dd5d-116">[Azure 資訊保護需求](https://docs.microsoft.com/azure/information-protection/get-started/requirements) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="4dd5d-116">[Requirements for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span></span>
- [<span data-ttu-id="4dd5d-117">Azure 資訊保護需求快速入門教學課程</span><span class="sxs-lookup"><span data-stu-id="4dd5d-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="4dd5d-118">下載 Azure 資訊保護用戶端</span><span class="sxs-lookup"><span data-stu-id="4dd5d-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
