---
title: Active Directory 未同步處理
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697620"
---
# <a name="active-directory-not-syncing"></a>Active Directory 未同步處理

如果您收到同步處理錯誤，例如「沒有最近的同步處理」，或是注意到 Office 管理員入口網站中的目錄同步處理狀態為「上次同步處理超過3天」，可能是因為 AADConnect 的設定不正確或許可權不足，無法執行同步處理。  

使用快速設定重新安裝 AADConnect，可快速解決問題：

1. [下載最新版本的 AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)。

2. [依照快速安裝的指示進行](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)。

如需有關 AADConnect 服務帳戶的詳細資訊，請參閱 [Azure AD Connect：帳戶和權限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。
