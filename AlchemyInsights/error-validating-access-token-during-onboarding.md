---
title: 在桌面機分析入職時，驗證存取權杖錯誤時發生錯誤
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813679"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>在桌面分析上架時發生「驗證存取權杖時發生錯誤」錯誤

驗證權杖到期時，通常會觀測到此錯誤。 通常重新整理頁面會重新整理標記。 不過，如果有任何條件式存取原則套用至用來進行板載桌面機 Analytics 的帳戶，此問題便會存在。 您可以在 Azure 入口網站中檢查 Azure AD 登入記錄檔，以查看用於桌面機分析上架的帳戶是否有任何登入失敗。

如需條件式存取的相關資訊，請造訪 [規劃您的條件式存取部署](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)。