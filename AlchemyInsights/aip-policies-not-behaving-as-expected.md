---
title: AIP：原則的行為與預期不符
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
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821618"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP：原則的行為與預期不符

Azure 資訊保護：原則的行為與預期不符，請參閱下列不同原則問題的建議指導方針：

1. 如果您遇到視覺標記問題，請檢閱[何時套用視覺標記](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)。
2. 如果您遇到自動加上標籤的問題，請檢閱[如何設定適用於 Azure 資訊保護的自動與建議分類條件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) (部分機器翻譯) 以及[敏感資訊類型尋找項目](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) (部分機器翻譯)。
3. 如果您遇到原生/Pfile 保護的問題，請檢閱[檔案 API 設定](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration) (部分機器翻譯)。
4. 檢查您是否使用未正確設定的範圍原則：[如何使用有範圍的原則為特定使用者設定 Azure 資訊保護原則](https://docs.microsoft.com/azure/information-protection/configure-policy-scope) (部分機器翻譯)。
5. 如果在附加標籤文件時，Outlook 無法使用自動標籤，請確認 DRMEncryptProperty 並未按照以下所述定義：[安全性的 IRM 註冊表設定](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)。

如果您仍然遇到問題，請收集 Azure 資訊保護用戶端記錄，並將匯出的記錄附加到此票證。

1. 在 Outlook 中開啟 Office 文件或建立新的電子郵件。
2. 按一下 [保護/敏感度]  >  [說明和意見反應]。
3. 按一下 [匯出記錄]。
4. 將記錄儲存到您選擇的位置，然後將它們附加到此服務要求。

其他資源：

- [如何設定 Azure 資訊保護的視覺標記標籤](https://docs.microsoft.com/azure/information-protection/configure-policy-markings) (部分機器翻譯)
- [檢閱 Azure 資訊保護文件](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [在 Microsoft 365 應用程式中使用敏感度標籤](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps) (部分機器翻譯)

