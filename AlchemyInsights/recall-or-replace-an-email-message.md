---
title: 回收或取代的電子郵件訊息
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 6e66b5d60fe9ac66c2f2f8f7e99e753652c3a59e
ms.sourcegitcommit: bcb2612ab8ba2aee5165e3912dca95cc1bdd09f4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/16/2019
ms.locfileid: "34096438"
---
# <a name="recall-or-replace-an-email-message"></a>回收或取代的電子郵件訊息

- 您可以**只重新叫用郵件，傳送給您組織中的人員**。 如果郵件已傳送到 Gmail 地址，例如，您無法恢復它。
- 您可以**只會重新叫用從電腦版 Outlook 2016 送出的郵件**。 如果使用者傳送郵件，使用 Mac 版 Outlook 或網頁型 Outlook，您就無法再回收。
- 如果您是系統管理員，您還可以**代表使用者藉由使用 PowerShell 重新叫用郵件**。 您無法回收從管理中心的郵件。 向下 」 搜尋並刪除電子郵件組織中的 「 捲動如需詳細資訊。

***回收或取代您傳送電子郵件訊息***
1. 在 [Outlook 視窗左側的 [資料夾] 窗格中，選擇 [寄件備份] 資料夾。
2. 開啟您想要回收的郵件。 您必須按兩下以開啟郵件。 選取郵件，讓它顯示在讀取窗格中，將不允許您回收郵件。
3. 從 [郵件] 索引標籤中，選取 [**動作** > **回收這封郵件**。
4. 選擇 [**刪除此郵件未讀取**或**刪除未閱讀的郵件，並取代為新郵件**，然後選取 **[確定]**。
5. 如果您正在傳送替換訊息，撰寫郵件，然後選取 [**傳送**]。
6. 成功或失敗的訊息重新叫用取決於 Outlook 中的收件者的設定。 

如需詳細資訊，包括如何檢查重新叫用，請參閱[重新叫用] 或 [取代您傳送電子郵件訊息](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)。

***搜尋並刪除電子郵件組織中***若要搜尋並刪除貴組織中的電子郵件訊息，它是最簡單如果您是全域系統管理員。如果您不是全域系統管理員，您必須將帳戶新增至 eDiscovery 管理員角色群組時，或 「 符合性搜尋管理 」 角色。 若要刪除的郵件，您需要加入 「 組織管理 」 角色群組或 「 搜尋及清除的 「 管理 」 角色。 [安全性 & 合規性中心](https://protection.office.com/)中指派給這些角色的權限。

1. [建立內容搜尋](https://docs.microsoft.com/en-us/office365/securitycompliance/content-search)來尋找要刪除的郵件。
2. [連接到安全性 & 合規性中心 PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。 

如果您正在使用 MFA，請參閱 < <b0>Connect to Office 365 安全性 &amp; 合規性中心 PowerShell 中使用多重要素驗證</b0>。 