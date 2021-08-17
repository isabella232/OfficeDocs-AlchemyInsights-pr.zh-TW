---
title: 封鎖使用者建立的電子郵件簽名
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: ad743cea4b8735b35b90bd5bf3d0b5b933184ed82858e828a68beb2ca2f8270c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54103543"
---
# <a name="block-user-made-email-signatures"></a>封鎖使用者建立的電子郵件簽名

下列解決方案只適用于 Outlook 網頁版中建立的電子郵件簽名。 如果您有內部部署 Exchange Server，您只能在 Outlook 應用程式中封鎖簽名。

1. 在系統管理中心中，選擇 [系統 **管理中心**]  >  **Exchange**。
2. 按一下 [**許可權**]  >  **Outlook Web App 原則**。
3. 選取原則，然後按一下鉛筆圖示進行編輯。
4. 按一下 [其他 **功能**  >  **選項**]。
5. 在 [ **使用者經驗**] 底下，清除 [ **電子郵件簽名** ] 核取方塊，然後按一下 [ **儲存**]。

**重要：** 如果在清除此核取方塊之前新增了簽名，使用者仍可使用它。 要求他們移除。
