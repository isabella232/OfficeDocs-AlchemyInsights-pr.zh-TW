---
title: 如何在 Outlook 中為 Windows 新增或移除代理人
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: 8db800d5c23b4cc2057f94abaf357082914143d3
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329016"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>如何在 Outlook 中為 Windows 新增或移除代理人

若要在 Outlook 中為 Windows 新增代理人： 

1. 按一下 [檔案] 索引卷 **標，然後** 選擇 [**帳戶設定**]，然後選擇 [**委派存取**]。
2. 按一下 [ **新增**]。 如果 [**新增**] 不出現，Outlook 和 Exchange 之間可能不存在作用中的連線。 Outlook 狀態列會顯示連接狀態。
3. 輸入您想要指定為代理人的人員名稱，或在搜尋結果清單中選擇名稱。

    **附注**：代理人必須是組織的 Exchange 全域通訊清單 (GAL) 中的人員。
4. 按一下 [ **新增** ]，然後按一下 **[確定]**。
5. 在 [**委派許可權**] 對話方塊中，接受預設許可權設定，或選取 [Exchange 資料夾的自訂訪問層級]。

    - 若代理人只需要處理會議邀請與回應的許可權，則預設許可權設定（例如代理人）會 **接收傳送給我的會議相關郵件的副本** 。 [ **收件** 匣] 許可權設定可保留 [ **無**]。 會議邀請和回應會直接移至代理人的收件匣。

    **附注**：依預設，授與代理人 **(可以讀取、建立及修改** [行事 **曆** ] 資料夾的專案) 許可權。 當代理人代表您回應會議時，它會自動新增至您的 [行事 **曆** ] 資料夾。

5. 若要傳送郵件以通知代理人已變更的許可權，請選取 [ **自動傳送郵件給代理人摘要這些許可權** ] 核取方塊。
6. 如有需要，請選取 [ **代理人可以查看我的私人性質專案** ] 核取方塊。

    **重要**：此設定會影響所有 Exchange 資料夾。 這包括所有郵件、連絡人、行事曆、Tasks、記事及日誌資料夾。 沒有任何方法可以只授與指定資料夾中私人專案的存取權。

7. 選擇 [確定]。

    **附注**：
    - 以「代理傳送者」許可權傳送的郵件會在 [ **寄件者**] 旁邊包括代理人和您的名稱。 當郵件以「以傳送方式傳送」許可權傳送時，只會出現您的名稱。
    - 一旦您新增某人做為代理人，便可將您的 Exchange 信箱新增至其 Outlook 設定檔。 如需相關指示，請參閱 [管理其他人的郵件和行事曆專案](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)。

若要在 Windows 中移除 Outlook 的代理人：

1. 按一下 **[檔案** ] 索引標籤。
2. 按一下 [**帳戶設定**，然後按 **代理存取**。
3. 選擇您要變更許可權的代理人名稱，然後按一下 [ **移除** ] 後再按一下 **[確定]**。
