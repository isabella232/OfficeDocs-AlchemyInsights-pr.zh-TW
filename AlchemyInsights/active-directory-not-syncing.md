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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314195"
---
# <a name="active-directory-not-syncing"></a>Active Directory 未同步處理

如果您收到同步處理錯誤，例如「沒有最近的同步處理」，或是注意到 Office 系統管理入口網站中的目錄同步處理狀態是「上次同步處理超過3天」，可能是 AADConnect 設定不當或許可權不足，無法執行同步處理。  

使用快速設定重新安裝 AADConnect，可快速解決問題：

1. [下載最新版本的 AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)。

2. [依照快速安裝的指示進行](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)。

Azure AD Connect 必須安裝在 Windows Server 2012 或更新版本。 此伺服器必須加入網域，且可以是網域控制站或成員伺服器。 如需 Azure AD 連線需求和先決條件的完整清單，請參閱[AZURE ad 連線的必要條件](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)。

如需有關 AADConnect 服務帳戶的詳細資訊，請參閱 [Azure AD Connect：帳戶和權限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。
