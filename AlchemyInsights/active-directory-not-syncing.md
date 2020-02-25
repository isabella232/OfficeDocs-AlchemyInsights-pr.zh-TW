---
title: 不進行同步處理的 active Directory
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265131"
---
# <a name="active-directory-not-syncing"></a>不進行同步處理的 active Directory

如果您會收到同步處理錯誤，例如 「 沒有最近同步處理 」，或通知 Office 系統管理入口網站中的目錄同步處理狀態會說: 「 上次同步處理 3 天之內，」 可能是 AADConnect 已設定不正確或不足若要執行同步處理的權限。  

重新 AADConnect 安裝使用快速設定可能會解決此問題： 快速：

1. [下載最新版的 AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)。

2. [遵循指示來快速安裝](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)。

如需 AADConnect 服務帳戶的詳細資訊，請參閱[Azure AD Connect： 帳戶和權限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。
