---
title: Outlook 桌面召回或取代電子郵件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663981"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>召回或取代 Outlook 電子郵件

- 作為管理員，您可以 **代表使用者使用 PowerShell 撤回郵件**。 您無法從系統管理中心重新叫用郵件。
- 您 **只能召回傳送給組織中人員的郵件**。 例如，如果郵件已傳送至 Gmail 位址，您就無法將其重新叫用。
- 您 **只能撤銷從電腦上的 Outlook 2016 傳送的郵件**。 如果使用者使用 Outlook for Mac 或 web 上的 Outlook 傳送郵件，您就無法將其重新叫用。

若要撤回或取代電子郵件：

1. 在 Outlook 視窗左側的 [資料夾] 窗格中，選取 [寄件備份] 資料夾。
1. 按兩下您要重新開啟的郵件。
1. 選取 [**郵件**] 索引標籤，然後選取 [**動作**] [重新  >  **叫用此郵件**]。
1. 選取 [ **刪除此郵件的未讀副本** ] 或 [ **刪除未讀取的副本並以新郵件取代**]，然後選取 **[確定]**。
1. 如果您正在傳送取代郵件，請撰寫郵件，然後選取 [ **傳送**]。
1. 郵件召回的成功或失敗取決於 Outlook 中收件者的設定。 如需檢查重新叫用的步驟，請參閱 [本文](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)。

搜尋並刪除組織中的電子郵件

- 如果您不是全域系統管理員，則必須將您的帳戶新增至「eDiscovery 管理員」角色或「符合性搜尋管理」角色，才能搜尋郵件。 若要刪除郵件，您需要加入「組織管理」角色群組或「搜尋並清除」管理角色。 在 [ [安全性與合規性中心](https://go.microsoft.com/fwlink/?linkid=2083731)] 中指派這些角色的許可權。
- [建立內容搜尋](https://docs.microsoft.com/microsoft-365/compliance/content-search) ，以尋找要刪除的郵件。
- [連接到安全性與合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。

如果您使用的是多重要素驗證，請參閱 [使用多重要素驗證連線至 Microsoft 365 安全性與合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)。