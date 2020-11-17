---
title: 建立群組
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086290"
---
# <a name="create-a-group"></a>建立群組

本主題說明群組的建立。

**建立群組的許可權**

確定您有權建立新的群組。 全域管理員可以停用 Azure 入口網站或存取面板中的群組建立。 您可能需要管理員為您建立新的群組，或為您提供適當的許可權。

**管理群組建立許可權**

1. 全域管理員可以在 azure 入口網站或 Access 面板中，透過選擇「使用者可以在 azure 入口網站中建立安全性群組」或「使用者 **可以在 azure** 入口網站中建立 Office 365 群組」  >  **)  (** 選項，管理群組建立許可權 (以) 或 Office 365 群組的安全性相關的原因。
2. 您也可以限制群組建立，以選取一組使用者，如果您擁有 Azure Active Directory P1 優質授權。

**停用新 Office 365 群組成員的歡迎使用通知**

在 Powershell 中將 **UnifiedGroupWelcomeMessageEnabled** 設定為 False，即可停用傳送給新增至 Office 365 群組之使用者的歡迎使用通知。 若要深入瞭解 [，請參閱此設定](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)。

