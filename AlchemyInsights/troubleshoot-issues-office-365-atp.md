---
title: 疑難排解 Office 365 高級威脅防護（ATP）的問題
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511103"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>疑難排解 Office 365 ATP 的問題

- **請注意電子郵件傳遞是否延遲**？ 嘗試針對您的 ATP 安全附件原則使用動態傳遞選項。 這樣可避免電子郵件傳遞延遲，同時也會防止收件者受到惡意檔案的傳遞。
- **您是否想要報告誤報或漏報**？ 使用此連結提交您的檔案進行分析：[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **您是否知道您可以為組織中的人員所傳送的電子郵件啟用 ATP 安全連結保護**？ 請遵循下列步驟：
    1. 移至 https://protection.office.com 並登入。
    2. 移至**威脅管理**  >  **原則**  >  **安全連結**。
    3. 在 [套用**至特定**收件者的原則] 底下，編輯（或新增）原則。
    4. 選取 **[套用安全連結] 至組織內所傳送的郵件**。
    5. 儲存原則，並允許大約30分鐘的變更，以透過您的資料中心來運作。
- 若要取得其他有關 ATP 的說明，請參閱[Office 365 Advanced 威脅防護](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)。