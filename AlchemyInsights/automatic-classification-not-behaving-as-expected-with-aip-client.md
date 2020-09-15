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
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>自動分類的行為與 AIP 用戶端預期的行為不符

自動分類的行為未如預期，請使用下列建議的指導方針：

1. 如果您遇到自動加上標籤的問題，請參閱[如何設定適用於 Azure 資訊保護的自動與建議分類條件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) (部分機器翻譯) 以及[敏感資訊類型尋找項目](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) (部分機器翻譯)。
2. 檢查您是否使用未正確設定的範圍原則：[如何使用有範圍的原則為特定使用者設定 Azure 資訊保護原則](https://docs.microsoft.com/azure/information-protection/configure-policy-scope) (部分機器翻譯)。
3. 如果在附加標籤文件時，Outlook 無法使用自動標籤，請確認 `DRMEncryptProperty` 並未按照以下所述定義：[安全性的 IRM 註冊表設定](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)。
4. 如果您在 Azure 資訊保護原則中使用的是[內建資訊類型](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b)，請確認您的內容符合預期的格式。
5. 請確認標籤已正確設定 [自動]**** 或 [建議]****。 ([自動]**** 加上標籤適用於所有 Microsoft 365 應用程式，但 [建議]**** 可用於除了 Outlook 之外的所有 Microsoft 365 應用程式。)
6. 您不能對先前手動加上標籤，或先前以較高分類自動加上標籤的文件和電子郵件進行自動分類。  如需詳細資訊，請參閱[如何套用自動或建議標籤](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)。
7. 如果您仍然遇到問題，請收集 Azure 資訊保護用戶端記錄，並將匯出的記錄附加到您的支援票證。 若要匯出 Azure 資訊保護記錄：
    - 在 Outlook 中開啟 Office 文件或建立新的電子郵件。
    - 按一下 [保護/敏感度]****  >  [說明和意見反應]****。
    - 按一下 [匯出記錄]****。
    - 將記錄儲存到您選擇的位置，然後將它們附加到您的服務要求。

如需詳細資訊，請參閱：

- [如何設定適用於 Azure 資訊保護的自動與建議分類條件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) (部分機器翻譯)
- [使用 Azure 資訊保護的常見案例使用方法指南](https://docs.microsoft.com/azure/information-protection/how-to-guides) (部分機器翻譯)
- [檢閱 Azure 資訊保護文件](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [檢閱 Azure 資訊保護訂閱與功能](https://azure.microsoft.com/pricing/details/information-protection)
- [Azure 資訊保護需求](https://docs.microsoft.com/azure/information-protection/get-started/requirements) (部分機器翻譯)
- [Azure 資訊保護需求快速入門教學課程](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [下載 Azure 資訊保護用戶端](https://www.microsoft.com/download/details.aspx?id=53018)
