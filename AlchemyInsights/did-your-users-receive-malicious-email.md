---
title: 您的使用者是否收到惡意電子郵件
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 608e2226c055f58ecf4f62e3c913106a6d319190ed6b317508e41514c12ba5d0
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893394"
---
# <a name="did-your-users-receive-malicious-email"></a>您的使用者是否收到惡意電子郵件?

您現在可以使用 [Microsoft 365 Defender 入口網站提交](https://sip.security.microsoft.com/reportsubmission?viewid=admin)，將惡意電子郵件回報給 Microsoft。

系統會掃描 [管理員提交](https://security.microsoft.com/reportsubmission?viewid=admin) 中所提交的郵件，然後下列結果將顯示在詳細資料飛出視窗中：

- 寄件者在傳遞電子郵件時，電子郵件驗證是否失敗。
- 任何有關可能會影響或覆寫郵件決策的原則點擊的資訊。
- 目前的引爆結果，查看郵件中所含的 URL 或檔案是否惡意。
- 來自評級員 的意見反應

如果發現覆寫，則應該會在幾分鐘內完成重新掃描。如果電子郵件驗證中沒有任何問題，或傳遞不受覆寫影響，則評級員的意見反應可能需要多達一天的時間。

如果您不同意郵件、URL 或檔案上的最終決策 (封鎖與未封鎖)，請在一天后重新提交該郵件。 當您再次提交郵件後，決策變更的可能性相當高。

同時，您可以依照[本文](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)中的指示，從使用者的收件匣中移除惡意電子郵件。

- 擁有 Microsoft Defender for Office 365 的客戶可以：
  - 使用 [威脅總管 [尋找] 並 [刪除可疑的電子郵件]](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [使用安全連結封鎖存取](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links)惡意 URL
  - 追蹤已點擊和已存取惡意 URL 的使用者：[查看網路釣魚 URL，然後點擊決策資料](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - 手動 [啟動 [自動化調查]](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

請按照[防範惡意 URL 和檔案](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)中的指示來保護自己免受惡意檔案和 URL 的攻擊。
