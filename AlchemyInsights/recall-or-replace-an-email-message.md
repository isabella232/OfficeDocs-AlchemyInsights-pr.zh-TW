---
title: 召回或取代電子郵件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509447"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>召回或取代 Microsoft 365 中的電子郵件

- 您**只能召回傳送給組織中人員的郵件**。 例如，如果郵件已傳送至 Gmail 位址，您就無法將其重新叫用。
- 您**只能召回從 Outlook 2016 傳送給電腦的郵件**。 如果使用者使用 Outlook for Mac 或 web 上的 Outlook 傳送郵件，您就無法將其重新叫用。
- 如果您是系統管理員，則可以**使用 PowerShell 來代表使用者重新叫用郵件**。 您無法從系統管理中心重新叫用郵件。 向內滾動至「搜尋並刪除組織中的電子郵件」，以取得詳細資訊。

**召回或取代您傳送的電子郵件**

1. 在 Outlook 視窗左側的 [資料夾] 窗格中，選擇 [送出的專案] 資料夾。
2. 開啟您要撤回的郵件。 您必須按兩下以開啟郵件。 選取郵件，使其出現在讀取窗格中，就不會讓您想起郵件。
3. 從 [郵件] 索引標籤中，選取 [**動作**  >  **撤回此郵件**]。
4. 選擇 [**刪除此郵件的未讀副本**] 或 [**刪除未讀取的副本並以新郵件取代**]，然後選取 **[確定]**。
5. 如果您要傳送取代郵件，請撰寫郵件，然後選取 [**傳送**]。
6. 郵件召回的成功或失敗取決於 Outlook 中的收件者設定。

如需詳細資訊，包括如何檢查召回，請參閱[召回或取代您傳送的電子](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)郵件。

***搜尋並刪除組織中的電子郵件***若要在您的組織中搜尋並刪除電子郵件訊息，當您是全域系統管理員時，它會是最簡單的方法。如果您不是全域系統管理員，則必須將您的帳戶新增至 eDiscovery 管理員角色群組，或「符合性搜尋管理」角色。 若要刪除郵件，您需要加入「組織管理」角色群組或「搜尋並清除」管理角色。 在[安全性 & 規範中心](https://protection.office.com/)指派這些角色的許可權。

1. [建立內容搜尋](https://docs.microsoft.com/microsoft-365/compliance/content-search)，以尋找要刪除的郵件。
2. [連線到安全性與合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。 

如果您使用的是 MFA，請參閱[使用多重要素驗證連線至 Microsoft 365 security & 合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)。 
