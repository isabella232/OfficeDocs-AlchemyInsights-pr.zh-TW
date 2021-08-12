---
title: 透過提供網路郵件識別碼提交電子郵件訊息
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1a6f9815a36cc267a815ff9757d713afed5d95aec4f7c537135c88cadf26cc51
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929908"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>透過提供網路郵件識別碼提交電子郵件訊息

1. 在 **新的提交** 快顯視窗中，選取 [ **電子郵件** 和 **網路消息識別碼**]。
2. 請遵循下列步驟，在 Outlook 中尋找電子郵件的郵件識別碼：
    1. 按兩下電子郵件以開啟它。
    1. 選取 [**檔**  >  **屬性**]。
    1. 開啟記事本或空白的 Word 檔，然後複製並貼上 [**網際網路標題**] 方塊中的內容，並將其貼到已開啟的檔中，以取得更好的知名度。
    1. 找出 **X-MS-Exchange-Organization-網路 Message-Id** ] 欄位。 在 **：** 之後的值是您提交所需的識別碼。
3. 在 **[** 收件者] 底下的 [垃圾郵件] 資料夾中進入此電子郵件的所有收件者，請選擇 [ **全選**]。 如果不是，請只選取報告問題的使用者。
4. 在 **提交的原因** 下，如果您選取 [ **應該已封鎖**]，請指定是否應該封鎖郵件為 **垃圾郵件**、 **網路釣魚** 或 **惡意** 代碼，然後選取 [ **提交**]。

若要深入瞭解，請參閱 how [to 提交可疑的垃圾郵件、網路釣魚、URLs 及檔案給 Microsoft 進行掃描](https://go.microsoft.com/fwlink/?linkid=2101479)。
