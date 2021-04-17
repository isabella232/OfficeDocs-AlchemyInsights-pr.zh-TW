---
title: Active Directory 未同步處理
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822842"
---
# <a name="active-directory-not-syncing"></a>Active Directory 未同步處理

如果您收到同步處理錯誤，例如「沒有最近的同步處理」，或是注意到 Office 管理員入口網站中的目錄同步處理狀態為「上次同步處理超過3天」，可能是因為 AADConnect 的設定不正確或許可權不足，無法執行同步處理。  

使用快速設定重新安裝 AADConnect，可快速解決問題：

1. [下載最新版本的 AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)。

2. [依照快速安裝的指示進行](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)。

如需有關 AADConnect 服務帳戶的詳細資訊，請參閱 [Azure AD Connect：帳戶和權限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。
