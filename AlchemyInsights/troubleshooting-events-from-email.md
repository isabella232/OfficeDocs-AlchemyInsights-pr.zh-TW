---
title: 疑難排解來自電子郵件的事件
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
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105343"
---
# <a name="troubleshooting-events-from-email"></a>疑難排解來自電子郵件的事件

1. 確認已為信箱啟用該功能：**Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. 然後查看「來自電子郵件的事件」記錄 **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. 在「來自電子郵件的事件」記錄中，找出與信箱中的項目相符的 InternetMessageId。  

4. TrustScore 會決定是否要新增該項目。 只有當 TrustScore = "Trusted" 時，才會新增事件。

TrustScore 是由位於郵件標頭中的 SPF、Dkim 或 Dmarc 內容所決定。

若要檢視這些內容：

**電腦版 Outlook**

- 開啟項目
- 檔案 -> 內容 -> 網際網路標頭

或

**MFCMapi**

- 導覽至收件匣中的項目
- 尋找 PR_TRANSPORT_MESSAGE_HEADERS_W

這些內容會在傳輸和路由期間決定並記錄。 如需進一步的疑難排解，您可能需要追蹤關於 SPF、DKIM 和 DMARC 中失敗的傳輸支援。