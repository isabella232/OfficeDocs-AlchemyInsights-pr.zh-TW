---
title: Microsoft Defender for Office 365 反網路釣魚原則範例
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736186"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Microsoft Defender for Office 365 反網路釣魚原則範例

這些設定會啟用名為 *Domain 及 CEO* 的原則。 這個原則提供使用者和網域保護的模擬，然後將該原則套用至網域中使用者所收到的所有電子郵件。 首先，新增下列資訊以建立原則：

- **名稱**：網域與 CEO **描述**：確保 CEO 和您的網域未進行類比。
  **適用** 于：選取 **[收件者網域**]。 在 [ **任何**] 底下，選取 **[選擇**]，然後選取網域。 選取 **[+ 新增]**。 選取清單中網功能變數名稱稱旁邊的核取方塊 (例如， *contoso.com*) ]，然後選取 [ **新增**]。 選取 **[完成]**。
- 建立原則之後，您可以使用下列選項微調原則：
  - **新增要保護的使用者：** 在此範例中，至少要新增 CEO 的電子郵件地址。
  - **新增要保護的網域**：新增包含 CEO 的 office 的組織網域。
  - **選擇動作**：若要讓模擬的 **使用者傳送電子郵件**，請選取 [ **將郵件重新導向至另一個電子郵件地址**]，然後輸入安全性管理員 (的電子郵件地址，例如， *securityadmin@contoso.com*) 。 **若為類比網域傳送電子郵件**，請選取 **[隔離郵件**]。
  - **信箱智慧**：根據預設，當您建立新的反網路釣魚原則時，會選取此選項。 請將此設定保留為 **[開啟]**，以獲得最佳結果。
  - **新增信任的寄件者和網域：** 在此範例中，請勿定義任何覆寫。
- 檢查您的設定之後，請選取 [ **建立這個原則** ] 或 [ **儲存**] （視需要）。

若要深入瞭解，請參閱 [Microsoft 365 中的反網路釣魚原則](https://go.microsoft.com/fwlink/?linkid=2092235)。
