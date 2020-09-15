---
title: 自動分類的行為與 AIP 用戶端預期的行為不符
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
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715192"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a><span data-ttu-id="d123e-102">自動分類的行為與 AIP 用戶端預期的行為不符</span><span class="sxs-lookup"><span data-stu-id="d123e-102">Automatic classification not behaving as expected with the AIP client</span></span>

<span data-ttu-id="d123e-103">自動分類的行為未如預期，請使用下列建議的指導方針：</span><span class="sxs-lookup"><span data-stu-id="d123e-103">Automatic classification not behaving as expected, use the following recommended guidelines:</span></span>

1. <span data-ttu-id="d123e-104">如果您遇到自動加上標籤的問題，請參閱[如何設定適用於 Azure 資訊保護的自動與建議分類條件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) (部分機器翻譯) 以及[敏感資訊類型尋找項目](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="d123e-104">If you are having issues with automatic labeling, see [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
2. <span data-ttu-id="d123e-105">檢查您是否使用未正確設定的範圍原則：[如何使用有範圍的原則為特定使用者設定 Azure 資訊保護原則](https://docs.microsoft.com/azure/information-protection/configure-policy-scope) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="d123e-105">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
3. <span data-ttu-id="d123e-106">如果在附加標籤文件時，Outlook 無法使用自動標籤，請確認 `DRMEncryptProperty` 並未按照以下所述定義：[安全性的 IRM 註冊表設定](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)。</span><span class="sxs-lookup"><span data-stu-id="d123e-106">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that `DRMEncryptProperty` isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>
4. <span data-ttu-id="d123e-107">如果您在 Azure 資訊保護原則中使用的是[內建資訊類型](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b)，請確認您的內容符合預期的格式。</span><span class="sxs-lookup"><span data-stu-id="d123e-107">If you used the [built-in information types](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) for your Azure Information Protection policy, verify that your content matches the expected format.</span></span>
5. <span data-ttu-id="d123e-108">請確認標籤已正確設定 [自動]\*\*\*\* 或 [建議]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="d123e-108">Verify that the label is appropriately configured for **Automatic** or **Recommended**.</span></span> <span data-ttu-id="d123e-109">([自動]\*\*\*\* 加上標籤適用於所有 Microsoft 365 應用程式，但 [建議]\*\*\*\* 可用於除了 Outlook 之外的所有 Microsoft 365 應用程式。)</span><span class="sxs-lookup"><span data-stu-id="d123e-109">(**Automatic** labeling is available for all Microsoft 365 apps, whereas **Recommended** is available for all Microsoft 365 apps except for Outlook.)</span></span>
6. <span data-ttu-id="d123e-110">您不能對先前手動加上標籤，或先前以較高分類自動加上標籤的文件和電子郵件進行自動分類。</span><span class="sxs-lookup"><span data-stu-id="d123e-110">You cannot use automatic classification for documents and emails that were previously manually labeled or previously automatically labeled with a higher classification.</span></span>  <span data-ttu-id="d123e-111">如需詳細資訊，請參閱[如何套用自動或建議標籤](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)。</span><span class="sxs-lookup"><span data-stu-id="d123e-111">For more information, see: [How automatic or recommended labels are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).</span></span>
7. <span data-ttu-id="d123e-112">如果您仍然遇到問題，請收集 Azure 資訊保護用戶端記錄，並將匯出的記錄附加到您的支援票證。</span><span class="sxs-lookup"><span data-stu-id="d123e-112">If you are still experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to your support ticket.</span></span> <span data-ttu-id="d123e-113">若要匯出 Azure 資訊保護記錄：</span><span class="sxs-lookup"><span data-stu-id="d123e-113">To export Azure Information Protection logs:</span></span>
    - <span data-ttu-id="d123e-114">在 Outlook 中開啟 Office 文件或建立新的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="d123e-114">Open an Office document or create a new email in Outlook.</span></span>
    - <span data-ttu-id="d123e-115">按一下 [保護/敏感度]\*\*\*\*  >  [說明和意見反應]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="d123e-115">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
    - <span data-ttu-id="d123e-116">按一下 [匯出記錄]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="d123e-116">Click **Export Logs**.</span></span>
    - <span data-ttu-id="d123e-117">將記錄儲存到您選擇的位置，然後將它們附加到您的服務要求。</span><span class="sxs-lookup"><span data-stu-id="d123e-117">Save the logs to your choice of location, and attach them to your service request.</span></span>

<span data-ttu-id="d123e-118">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="d123e-118">For additional information, see:</span></span>

- <span data-ttu-id="d123e-119">[如何設定適用於 Azure 資訊保護的自動與建議分類條件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="d123e-119">[How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)</span></span>
- <span data-ttu-id="d123e-120">[使用 Azure 資訊保護的常見案例使用方法指南](https://docs.microsoft.com/azure/information-protection/how-to-guides) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="d123e-120">[How-to guides for common scenarios that use Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)</span></span>
- [<span data-ttu-id="d123e-121">檢閱 Azure 資訊保護文件</span><span class="sxs-lookup"><span data-stu-id="d123e-121">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d123e-122">檢閱 Azure 資訊保護訂閱與功能</span><span class="sxs-lookup"><span data-stu-id="d123e-122">Review Azure Information Protection subscriptions and features</span></span>](https://azure.microsoft.com/pricing/details/information-protection)
- <span data-ttu-id="d123e-123">[Azure 資訊保護需求](https://docs.microsoft.com/azure/information-protection/get-started/requirements) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="d123e-123">[Requirements for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span></span>
- [<span data-ttu-id="d123e-124">Azure 資訊保護需求快速入門教學課程</span><span class="sxs-lookup"><span data-stu-id="d123e-124">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="d123e-125">下載 Azure 資訊保護用戶端</span><span class="sxs-lookup"><span data-stu-id="d123e-125">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
