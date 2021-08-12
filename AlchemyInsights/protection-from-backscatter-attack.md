---
title: 防禦退信攻擊
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8c6b1cfe79d322702279877ff351397a366fa246710c04e25181a675ad2fdeab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911221"
---
# <a name="protection-from-backscatter-attack"></a>防禦退信攻擊

退信攻擊是您對於未寄送過的郵件所收到的未傳遞報告 (也稱為 NDR 或退回的郵件)。 濫發垃圾郵件者偽造 (詐騙) 其郵件的 **寄件者：** 地址，他們通常會使用實際的電子郵件地址來增加郵件的可信度。 因此，當濫發垃圾郵件者將郵件傳送給不存在的收件者時，目的地電子郵件伺服器基本上會遭到誘拐而透過 NDR 將無法傳遞的郵件退回給 **寄件者：** 地址中的偽造寄件者。

其他資訊可以在 [EOP 中的退信攻擊](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)中找到。

**啟用退信攻擊保護**

若要啟用退信攻擊保護，請遵循下列路徑。

**protection.office.com > 威脅管理 > 原則 > 反垃圾郵件 > 選取垃圾郵件篩選原則並編輯原則 > 垃圾郵件屬性 > 標示為垃圾郵件 > NDR 退信攻擊 > 設為 [開啟]**

如果您認為帳戶已遭到入侵，請參閱下列內容：

- [回應遭入侵的電子郵件帳戶](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [從 Office 365 中的 [受限使用者] 入口網站移除封鎖的使用者](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



