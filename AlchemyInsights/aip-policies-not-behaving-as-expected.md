---
title: AIP：原則的行為與預期不符
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 91308850c06485bdd11e81bd130770aefb247118
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580756"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="2898c-102">AIP：原則的行為與預期不符</span><span class="sxs-lookup"><span data-stu-id="2898c-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="2898c-103">Azure 資訊保護：原則的行為與預期不符，請參閱下列不同原則問題的建議指導方針：</span><span class="sxs-lookup"><span data-stu-id="2898c-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="2898c-104">如果您遇到視覺標記問題，請檢閱[何時套用視覺標記](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)。</span><span class="sxs-lookup"><span data-stu-id="2898c-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="2898c-105">如果您遇到自動加上標籤的問題，請檢閱[如何設定適用於 Azure 資訊保護的自動與建議分類條件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) (部分機器翻譯) 以及[敏感資訊類型尋找項目](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="2898c-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="2898c-106">如果您遇到原生/Pfile 保護的問題，請檢閱[檔案 API 設定](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="2898c-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="2898c-107">檢查您是否使用未正確設定的範圍原則：[如何使用有範圍的原則為特定使用者設定 Azure 資訊保護原則](https://docs.microsoft.com/azure/information-protection/configure-policy-scope) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="2898c-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="2898c-108">如果在附加標籤文件時，Outlook 無法使用自動標籤，請確認 DRMEncryptProperty 並未按照以下所述定義：[安全性的 IRM 註冊表設定](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)。</span><span class="sxs-lookup"><span data-stu-id="2898c-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="2898c-109">如果您仍然遇到問題，請收集 Azure 資訊保護用戶端記錄，並將匯出的記錄附加到此票證。</span><span class="sxs-lookup"><span data-stu-id="2898c-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="2898c-110">在 Outlook 中開啟 Office 文件或建立新的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="2898c-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="2898c-111">按一下 [保護/敏感度]\*\*\*\*  >  [說明和意見反應]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="2898c-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="2898c-112">按一下 [匯出記錄]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="2898c-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="2898c-113">將記錄儲存到您選擇的位置，然後將它們附加到此服務要求。</span><span class="sxs-lookup"><span data-stu-id="2898c-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="2898c-114">其他資源：</span><span class="sxs-lookup"><span data-stu-id="2898c-114">Additional resources:</span></span>

- <span data-ttu-id="2898c-115">[如何設定 Azure 資訊保護的視覺標記標籤](https://docs.microsoft.com/azure/information-protection/configure-policy-markings) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="2898c-115">[How to configure a label for visual markings for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)</span></span>
- [<span data-ttu-id="2898c-116">檢閱 Azure 資訊保護文件</span><span class="sxs-lookup"><span data-stu-id="2898c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- <span data-ttu-id="2898c-117">[在 Microsoft 365 應用程式中使用敏感度標籤](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="2898c-117">[Use sensitivity labels in Microsoft 365 apps](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)</span></span>

