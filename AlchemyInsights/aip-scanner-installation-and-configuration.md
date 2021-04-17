---
title: AIP 掃描器：安裝及設定
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821654"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP 掃描器：安裝及設定

**若要安裝 AIP 掃描器，請遵循建議的指導方針**：

1. 如果您正在升級但未執行全新安裝，請確保已遵循[升級 Azure 資訊保護掃描器](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)的指導方針，對於整合標籤用戶端，請參閱[升級 Azure 資訊保護掃描器](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)。
2. 驗證您是否符合[防火牆和網絡基礎結構設定需求](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)。
3. 請確保您的[原則已設定](https://docs.microsoft.com/azure/information-protection/configure-policy)為自動套用標籤，或在原則中具有預設標籤。
4. 確保為標籤/保護設定了相關的檔案類型，如 [Azure 資訊保護用戶端支持的檔案類型](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)中所述。 此外，如果您想要變更預設行為，請遵循以下指導方針： [變更檔案預設保護等級](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)。
5. 驗證設定為運行掃描程式服務的使用者帳戶是否具有所有設已定存儲庫的存取權限。
6. 如仍遇到問題，請匯出掃描器記錄並將其新增到您的支援票證。

**匯出 Azure 資訊保護掃描器記錄**

1. 瀏覽到運行掃描程式服務的使用者內容下的 %localappdata%\Microsoft\MSIP。
2. 壓縮 MSIP 資料夾下的所有內容。
3. 將記錄儲存到您選擇的位置，然後將它們附加到您的服務要求。
4. 您也可以使用 [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)。

**如需詳細資訊，請參閱**：
- [部署 Azure 資訊保護掃描器以自動分類和保護檔案](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [指定和使用 AIPAuthentication 的權杖參數](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [運行搜索循環並查看掃描器報告](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [檢閱 Azure 資訊保護文件](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure 資訊保護需求](https://docs.microsoft.com/azure/information-protection/get-started/requirements) (部分機器翻譯)
- [下載 Azure 資訊保護用戶端](https://www.microsoft.com/download/details.aspx?id=53018)
