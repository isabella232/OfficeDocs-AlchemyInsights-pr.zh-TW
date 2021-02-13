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
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232695"
---
# <a name="block-user-made-email-signatures"></a>封鎖使用者建立的電子郵件簽名

下列解決方案只適用于在 web 上的 Outlook 中建立的電子郵件簽名。 如果您有內部部署 Exchange 伺服器，您就只能封鎖 Outlook 應用程式中的簽章。

1. 在系統管理中心中，選擇 [系統 **管理中心**] [  >  **Exchange**]。
2. 按一下 [**許可權**] [  >  **Outlook Web App 原則**]。
3. 選取原則，然後按一下鉛筆圖示進行編輯。
4. 按一下 [其他 **功能**  >  **選項**]。
5. 在 [ **使用者經驗**] 底下，清除 [ **電子郵件簽名** ] 核取方塊，然後按一下 [ **儲存**]。

**重要：** 如果在清除此核取方塊之前新增了簽名，使用者仍可使用它。 要求他們移除。
