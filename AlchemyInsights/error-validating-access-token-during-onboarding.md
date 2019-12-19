---
title: 在桌面分析登入期間驗證存取 token 錯誤時發生錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741130"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>桌面分析上架期間 」 時發生錯誤驗證存取權杖 」 錯誤

此錯誤通常是觀察到的驗證權杖到期時。 通常，重新整理頁面重新整理權杖。 不過，這個問題可以保存如果沒有任何條件式存取原則套用至所使用的帳戶到委任桌面分析。 您可以檢閱 [Azure AD 登入 Azure 入口網站中的記錄檔中是否有任何登入失敗的桌面分析上架所使用的帳戶。

如需條件式存取的詳細資訊，請瀏覽[規劃條件式存取部署](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)。