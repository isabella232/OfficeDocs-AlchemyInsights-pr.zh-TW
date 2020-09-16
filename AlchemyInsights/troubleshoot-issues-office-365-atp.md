---
title: '疑難排解 Office 365 的問題「高級威脅防護 (ATP) '
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758056"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>疑難排解 Office 365 ATP 的問題

- **請注意電子郵件傳遞是否延遲**？ 嘗試針對您的 ATP 安全附件原則使用動態傳遞選項。 這樣可避免電子郵件傳遞延遲，同時也會防止收件者受到惡意檔案的傳遞。
- **您是否想要報告誤報或漏報**？ 使用此連結提交您的檔案進行分析： [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **您是否知道您可以為組織中的人員所傳送的電子郵件啟用 ATP 安全連結保護**？ 請遵循下列步驟：
    1. 移至 https://protection.office.com 並登入。
    2. 移至**威脅管理**  >  **原則**  >  **安全連結**。
    3. 在 [套用至特定收件者 **的原則**] 底下，編輯 (或新增) 原則。
    4. 選取 **[套用安全連結] 至組織內所傳送的郵件**。
    5. 儲存原則，並允許大約30分鐘的變更，以透過您的資料中心來運作。
- 若要取得其他有關 ATP 的說明，請參閱 [Office 365 Advanced 威脅防護](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)。