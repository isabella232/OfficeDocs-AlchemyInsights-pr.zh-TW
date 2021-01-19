---
title: 系統管理員同意問題
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888301"
---
# <a name="admin-consent-issues"></a>系統管理員同意問題

1. 啟用系統 [管理員同意工作流程](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) 以允許使用者直接從同意畫面要求系統管理員核准。

1. 如果您或您的應用程式的使用者在同意程式中看到意外的錯誤，請參閱本文以取得疑難排解步驟： [同意對應用程式執行同意時](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)，會發生未預期的錯誤。

1. 深入瞭解 [Microsoft identity 平臺的系統管理員同意](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)、 [同意提示](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) 的運作方式，以及如何 [評估要求以進行租使用者管理員的同意](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)。

1. 與 Microsoft identity platform 整合的應用程式遵循授權模式，可讓使用者和系統管理員控制資料的存取方式。 授權模型的實施已在 Microsoft identity platform 端點上更新，它會變更應用程式必須與 Microsoft identity platform 互動的方式。 請參閱 [Microsoft identity platform 端點中的許可權與同意](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) ，以取得此授權模型（包括範圍、許可權和同意）的概述。