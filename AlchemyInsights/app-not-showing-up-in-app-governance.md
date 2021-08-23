---
title: 我的應用程式不會顯示在應用程式管理中
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362368"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>我的應用程式不會顯示在應用程式管理中

若應用程式未顯示在應用程式管理中，請檢查下列各項：

1. 移至 [AZURE AD](https://aad.portal.azure.com/) ，並在 [概覽] 頁面上的上方列中搜尋應用程式名稱，尋找應用程式的應用程式識別碼。

1. Access Graph Explorer，並使用此查詢取代相關的應用 ID: 程式，在服務主體內搜尋應用程式識別碼 <appId> < https://graph.microsoft.com/v1.0/servicePrincipals? $search = "appId： <appId> " >

1. 若未傳回任何結果，請使用此查詢來搜尋應用程式內的應用程式識別碼，並 <appId> 以相關的 ID: 應用程式加以取代 < https://graph.microsoft.com/v1.0/applications? $Search = "appId： <appId> " >

如果您遇到查詢問題，請參閱 [Get support](https://docs.microsoft.com/microsoft-365/business-video/get-help-support)。 

如需詳細資訊或深入瞭解應用程式管理中的應用程式，請參閱 [瞭解 visibility 和 insights](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)。

如需查看您的應用程式的詳細資訊，請參閱 [查看您的應用程式](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)。
