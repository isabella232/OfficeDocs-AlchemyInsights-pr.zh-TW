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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816339"
---
# <a name="create-a-group"></a>建立群組

本主題說明群組的建立。

**建立群組的許可權**

確定您有權建立新的群組。 全域系統管理員可以在 Azure 入口網站或存取面板中停用群組建立。 您可能需要系統管理員才能建立新群組，或提供您適當權限。

**管理群組建立權限**

1. 全域管理員可以在 azure 入口網站或 Access 面板中，透過選擇「使用者可以在 azure 入口網站中建立安全性群組」或「使用者 **可以在 azure** 入口網站中建立 Office 365 群組」  >  **)  (** 選項，管理群組建立許可權 (以) 或 Office 365 群組的安全性相關的原因。
2. 您也可以限制群組建立，以選取一組使用者，如果您擁有 Azure Active Directory P1 優質授權。

**停用新 Office 365 群組成員的歡迎使用通知**

在 Powershell 中將 **UnifiedGroupWelcomeMessageEnabled** 設定為 False，即可停用傳送給新增至 Office 365 群組之使用者的歡迎使用通知。 在[這裡](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)深入了解此設定。

