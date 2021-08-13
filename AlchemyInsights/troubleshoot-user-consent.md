---
title: 疑難排解使用者的同意
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007889"
---
# <a name="troubleshoot-user-consent"></a>疑難排解使用者的同意

1. 您可以設定使用者同意透過 Azure 入口網站或 PowerShell 的應用程式。 如需詳細資訊，請參閱 [使用者同意設定](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 。
1. 管理員也可以使用[Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings)代表單一使用者授與委派許可權。 如需詳細資訊，請參閱 [代表使用者取得存取權](https://docs.microsoft.com/graph/auth-v2-user)。
1. [使用者同意錯誤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)：本文討論在同意應用程式期間可能發生的錯誤。 如果您正在疑難排解未包含任何錯誤訊息的意外同意提示，請參閱 [AZURE AD 的驗證案例](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。