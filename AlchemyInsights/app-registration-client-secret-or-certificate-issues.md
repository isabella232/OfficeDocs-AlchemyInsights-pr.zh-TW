---
title: 應用程式註冊用戶端密碼或憑證問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123115"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>應用程式註冊用戶端密碼或憑證問題

應用程式用戶端密碼即將過期？

不論已註冊的應用程式的建立方式為何，不論是透過應用程式註冊入口網站中的標準註冊程式，還是在您的租使用者中使用應用程式同意建立服務主體，都必須先建立新的用戶端密碼，然後再進行相關的應用程式程式碼更新。 最大有效期限是2年。 就像是提醒，必須記錄此機密值，否則會在保留入口網站中的 [應用程式註冊] 頁面後不再顯示。 如需詳細資訊，請參閱 [快速入門：在 microsoft identity platform 中註冊應用程式](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) ，以及 [microsoft Identity platform 的最佳作法](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)。

若要深入瞭解，請參閱 [在入口網站中建立 AZURE AD app & 服務主體-Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)。
