---
title: Yammer 中的通知
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: ff4c13560b9cbf283e5c6b92a259debdf96cca62
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/27/2020
ms.locfileid: "43911894"
---
# <a name="notifications-in-yammer"></a>Yammer 中的通知

若要提醒您相關交談中的新活動，[Yammer 會透過電子郵件傳送通知](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)，或在行動裝置上使用 Yammer，會透過推播通知。 根據預設，Yammer 會傳送通知給您網路中的許多活動類型。 使用者可以透過 Yammer 網站更新其電子郵件設定，並透過行動裝置應用程式設定推播通知。 

Yammer 已在 [Outlook 中新增支援互動式電子郵件](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420)。 部分電子郵件 (郵件複本) 將會在 Outlook 網頁版中變成互動式電子郵件。 未來更新會將此功能帶到其他版本的 Outlook。

**Yammer 中的通知類型**

- 電子郵件 (來自群組的更新、某人邀請您前往群組、您會在 [收件匣] 中收到一封郵件等等)
- 推播通知 (您會在被提及時傳送到行動裝置、在收件匣中收到郵件等等)
- 電腦版快顯視窗 (安裝 Yammer 電腦版應用程式時，系統會顯示名為「快顯」通知的使用者通知)。
- 鈴聲通知 (在 Yammer 網站內，使用者會看到不同事件的通知。 這些通知可能不一定與電子郵件或推播通知相關)。

更多[通知的詳細資訊](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)可供使用。

**管理通知**

使用者必須自行管理通知。 相關資訊可前往[如何啟用和停用 Yammer 電子郵件和行動裝置通知](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)了解。 

系統管理員無法代表使用者停用所有通知或控制通知。 系統管理員可以[控制電子郵件中的標誌，以及使用者是否需要確認電子郵件張貼的訊息](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer)。

**傳送給貴組織中多個使用者的電子郵件通知**

有時候 Yammer 會傳送一封電子郵件通知，而貴組織中的使用者收到的電子郵件數量超出預期。 如果您將通訊群組清單或其他類型的非個人電子郵件地址新增到 Yammer，就會發生這種情況。 無論是電子郵件地址屬於單一使用者，還是電子郵件地址，Yammer 都不知道，這會導致電子郵件傳送到多個收件者。 發生此問題時，您必須採取行動，以在 Yammer 中[使用該電子郵件位址暫停 (停用) 無效使用者](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)。 

若要降低發生此問題的幾率，您應該：

1. [針對 Yammer 強制執行 Office 365 身分識別](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)。
2. 封鎖外部寄件者將電子郵件傳送給您的組織，或將寄件者限制為已核准清單。

如果發生此問題：

1. 識別電子郵件的收件者，該電子郵件應符合 Yammer 中的使用者。 例如，all-in-sales@fabrikam.com 是一種用於所有銷售人員的 DL。 該 DL 可以從使用者收到的 Yammer 電子郵件中識別出來。
2. 使用 [[網路系統管理員] 中的停用 (暫停) 功能](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)，以暫停 all-in-sales@fabrikam.com 電子郵件地址的使用者。 暫停可以復原，因此比刪除更安全。 系統會在 90 天後自動刪除使用者。
3. 您也可以選擇檢閱[使用者匯出](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers)，以找出應該暫停的其他非使用者電子郵件地址。
