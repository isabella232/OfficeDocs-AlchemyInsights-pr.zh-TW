---
title: Outlook 桌面回收] 或 [取代電子郵件訊息
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389661"
---
# <a name="recall-or-replace-an-email-message"></a>回收或取代的電子郵件訊息

- 身為系統管理員，您還可以**代表使用者使用 PowerShell 重新叫用郵件**。 您無法回收從管理中心的郵件。
- 您可以**只重新叫用郵件，傳送給您組織中的人員**。 如果郵件已傳送到 Gmail 地址，例如，您無法恢復它。
- 您可以**只會重新叫用從 Outlook 2016 在 PC 上傳送的郵件**。 如果使用者傳送郵件，使用 Mac 版 Outlook 或網頁型 Outlook，您就無法再回收。

若要恢復或取代的電子郵件訊息：

1. 在 [Outlook 視窗左側的 [資料夾] 窗格中，選取 [寄件備份] 資料夾。
1. 連按兩下您想要回收以開啟的郵件。
1. 選取 [**郵件**] 索引標籤，然後選取 [**動作** > **回收這封郵件**。
1. 選取 [**刪除此郵件未讀取**或**刪除未閱讀的郵件，並取代為新的郵件**]，然後選取 **[確定]**。
1. 如果您正在傳送替換訊息，撰寫郵件，，，，然後選取 [**傳送**。
1. 成功或失敗的訊息重新叫用取決於 Outlook 中的收件者的設定。 若要查看重新叫用的步驟，請參閱[這篇文章](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)。

搜尋並刪除您的組織中的電子郵件

- 如果您不是全域系統管理員，您的帳戶必須新增至 eDiscovery 管理員 」 角色或符合性搜尋來搜尋郵件的管理角色。 若要刪除的郵件，您需要加入 「 組織管理 」 角色群組或 「 搜尋及清除的 「 管理 」 角色。 在[安全性與合規性中心](https://go.microsoft.com/fwlink/?linkid=2083731)指派這些角色的權限。
- [建立內容搜尋](https://docs.microsoft.com/office365/securitycompliance/content-search)來尋找要刪除的郵件。
- [連接到安全性與合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。

如果您使用多重要素驗證，請參閱 < <b0>Connect to Office 365 安全性與合規性中心 PowerShell 中使用多重要素驗證</b0>。