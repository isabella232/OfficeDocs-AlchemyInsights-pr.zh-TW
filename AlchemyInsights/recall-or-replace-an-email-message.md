---
title: 撤回或取代電子郵件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 170fbd632f0289a45d9497ac26fbe7f90cf88318
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35356588"
---
# <a name="recall-or-replace-an-email-message"></a>撤回或取代電子郵件

- 您**只能撤回傳送給組織中的人員的郵件**。 如果郵件已傳送至 Gmail 位址, 例如, 您無法撤回。
- 您**只能對電腦撤回從 Outlook 2016 傳送的郵件**。 如果使用者使用 Outlook for Mac 或網頁版 Outlook 傳送訊息, 您就無法撤回該郵件。
- 如果您是系統管理員, 您可以**使用 PowerShell 來代表使用者撤回郵件**。 您無法從系統管理中心撤回郵件。 向下滾動至 [在您的組織中搜尋並刪除電子郵件], 以取得詳細資訊。

***撤回或取代您傳送的電子郵件***

1. 在 Outlook 視窗左邊的資料夾窗格中, 選擇 [寄件備份] 資料夾。
2. 開啟您要撤回的郵件。 您必須按兩下以開啟郵件。 選取郵件, 使其出現在讀取窗格中, 並不會讓您撤回郵件。
3. 從 [郵件] 索引標籤中, 選取 [**動作** > **撤回此郵件**]。
4. 選擇 [**刪除此郵件的未讀取副本**] 或 [**刪除未讀取的副本, 並以新郵件取代**], 然後選取 **[確定]**。
5. 如果您要傳送取代郵件, 請撰寫郵件, 然後選取 [**傳送**]。
6. 郵件撤回的成功或失敗取決於 Outlook 中的收件者的設定。

如需詳細資訊, 包括如何檢查召回, 請參閱[撤回或取代您傳送的電子](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)郵件。

***在您的組織中搜尋並刪除電子郵件***若要在您的組織中搜尋並刪除電子郵件, 最簡單的情況是您是全域系統管理員。如果您不是全域系統管理員, 您的帳戶必須新增至 eDiscovery 管理員角色群組或符合性搜尋管理角色。 若要刪除郵件, 您必須加入「組織管理」角色群組或「搜尋」和「清除管理」角色。 這些角色的許可權會指派在[安全性 & 合規性中心](https://protection.office.com/)內。

1. [建立內容搜尋](https://docs.microsoft.com/office365/securitycompliance/content-search), 以尋找要刪除的郵件。
2. [連接至安全性 & 規範中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。 

如果您使用的是 MFA, 請參閱[Connect To Office 365 Security & 合規性中心 PowerShell 使用多重要素驗證](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)。 
