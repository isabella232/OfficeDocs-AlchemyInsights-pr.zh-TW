---
title: AIP 掃描器：安裝及設定
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
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686633"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="6635e-102">AIP 掃描器：安裝及設定</span><span class="sxs-lookup"><span data-stu-id="6635e-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="6635e-103">**若要安裝 AIP 掃描器，請遵循建議的指導方針**：</span><span class="sxs-lookup"><span data-stu-id="6635e-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="6635e-104">如果您正在升級但未執行全新安裝，請確保已遵循[升級 Azure 資訊保護掃描器](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)的指導方針，對於整合標籤用戶端，請參閱[升級 Azure 資訊保護掃描器](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)。</span><span class="sxs-lookup"><span data-stu-id="6635e-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="6635e-105">驗證您是否符合[防火牆和網絡基礎結構設定需求](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)。</span><span class="sxs-lookup"><span data-stu-id="6635e-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="6635e-106">請確保您的[原則已設定](https://docs.microsoft.com/azure/information-protection/configure-policy)為自動套用標籤，或在原則中具有預設標籤。</span><span class="sxs-lookup"><span data-stu-id="6635e-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="6635e-107">確保為標籤/保護設定了相關的檔案類型，如 [Azure 資訊保護用戶端支持的檔案類型](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)中所述。</span><span class="sxs-lookup"><span data-stu-id="6635e-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="6635e-108">此外，如果您想要變更預設行為，請遵循以下指導方針： [變更檔案預設保護等級](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)。</span><span class="sxs-lookup"><span data-stu-id="6635e-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="6635e-109">驗證設定為運行掃描程式服務的使用者帳戶是否具有所有設已定存儲庫的存取權限。</span><span class="sxs-lookup"><span data-stu-id="6635e-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="6635e-110">如仍遇到問題，請匯出掃描器記錄並將其新增到您的支援票證。</span><span class="sxs-lookup"><span data-stu-id="6635e-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="6635e-111">**匯出 Azure 資訊保護掃描器記錄**</span><span class="sxs-lookup"><span data-stu-id="6635e-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="6635e-112">瀏覽到運行掃描程式服務的使用者內容下的 %localappdata%\Microsoft\MSIP。</span><span class="sxs-lookup"><span data-stu-id="6635e-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="6635e-113">壓縮 MSIP 資料夾下的所有內容。</span><span class="sxs-lookup"><span data-stu-id="6635e-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="6635e-114">將記錄儲存到您選擇的位置，然後將它們附加到您的服務要求。</span><span class="sxs-lookup"><span data-stu-id="6635e-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="6635e-115">您也可以使用 [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)。</span><span class="sxs-lookup"><span data-stu-id="6635e-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="6635e-116">**如需詳細資訊，請參閱**：</span><span class="sxs-lookup"><span data-stu-id="6635e-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="6635e-117">部署 Azure 資訊保護掃描器以自動分類和保護檔案</span><span class="sxs-lookup"><span data-stu-id="6635e-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="6635e-118">指定和使用 AIPAuthentication 的權杖參數</span><span class="sxs-lookup"><span data-stu-id="6635e-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="6635e-119">運行搜索循環並查看掃描器報告</span><span class="sxs-lookup"><span data-stu-id="6635e-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="6635e-120">檢閱 Azure 資訊保護文件</span><span class="sxs-lookup"><span data-stu-id="6635e-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- <span data-ttu-id="6635e-121">[Azure 資訊保護需求](https://docs.microsoft.com/azure/information-protection/get-started/requirements) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="6635e-121">[Requirements for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span></span>
- [<span data-ttu-id="6635e-122">下載 Azure 資訊保護用戶端</span><span class="sxs-lookup"><span data-stu-id="6635e-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
