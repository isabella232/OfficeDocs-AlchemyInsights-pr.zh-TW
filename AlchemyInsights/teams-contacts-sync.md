---
title: Teams 連絡人同步
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
- "9004610"
- "11540"
ms.openlocfilehash: 36273e998bbf97e261dbaa49b3b57aab17216e9f0e9bd29c5d2b9f6c0d9803e4
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900755"
---
# <a name="teams-contacts-sync"></a>Teams 連絡人同步

Teams 會使用貴組織 Active Directory 中的連絡人，以及新增至使用者的 Outlook 預設資料夾的連絡人。 如果連絡人未顯示在 Microsoft Teams 中，請嘗試以下步驟：

**注意：** 如果最近更新了一個或多個連絡人的資訊，則同步連絡人最多需要 48 小時。

1. 登出 Teams 並重新啟動。 檢查是否顯示連絡人。
1. 清除 Teams 快取：
    1. 瀏覽至 **%appdata%\Microsoft\Teams**。
    1. 刪除資料夾的內容。
    1. 重新啟動電腦，然後啟動 Teams。
1. 如果連絡人在 Outlook 中，請確保將其新增至連絡人清單。 在 Outlook 中，從網址列中選取 **[檔案]**，然後選取 **[新增至連絡人]**。
1. 請確保使用者的 Exchange 信箱是在線上託管 (非內部部署)。 如需詳細資訊，請參閱 [Exchange 和 Microsoft Teams 如何互動](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)。
1. 請確保連絡人的電話號碼已新增到連絡人資訊中。
1. 在 [搜尋] 列中搜尋連絡人的電子郵件。 您可以擷取連絡人清單同步的連絡人。
