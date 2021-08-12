---
title: 建立群組
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929296"
---
# <a name="create-a-group"></a>建立群組

本主題說明群組的建立。

**建立群組的許可權**

確定您有權建立新的群組。 全域系統管理員可以在 Azure 入口網站或存取面板中停用群組建立。 您可能需要系統管理員才能建立新群組，或提供您適當權限。

**管理群組建立權限**

1. 全域管理員可以管理群組建立許可權 (以) 或 Office 365 在 azure 入口網站或 Access 面板中建立的群組，方法是選擇 [使用者可以在 azure 入口網站中建立安全性群組] 或 [使用者可以在 azure 入口網站中建立 Office 365 群組] 選項，在 [**所有群組**] 的  >  **[一般**] (設定) 。
2. 如果您有 Azure Active Directory P1 進階版授權，您也可以限制群組建立，以選取使用者群組。

**停用新 Office 365 群組成員的歡迎使用通知**

在 Powershell 中將 **UnifiedGroupWelcomeMessageEnabled** 設定為 False，即可停用已傳送給加入 Office 365 群組之使用者的歡迎使用通知。 在[這裡](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)深入了解此設定。

