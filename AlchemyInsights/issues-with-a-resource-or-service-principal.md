---
title: 資源或服務主體的問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/28/2021
ms.locfileid: "50716122"
---
# <a name="issues-with-a-resource-or-service-principal"></a>資源或服務主體的問題

1. 如果您剛剛開始， [Azure Active directory 中的應用程式和服務主體物件](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) 會描述 Azure active directory 中的應用程式註冊、應用程式物件和服務主體：其用途、使用方式，以及它們之間的相互關聯方式。 同時也會呈現多承租人範例案例，以說明應用程式的應用程式物件與對應服務主體物件之間的關係。
2. 您可以 [在 Azure Active Directory 中讀取應用程式和服務主體物件](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)，深入瞭解應用程式和服務主體之間的關係。
3. [操作方法：使用入口網站建立可以存取資源的 AZURE ad 應用程式和服務主體](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) 顯示如何建立新的 Azure Active Directory (azure ad) 應用程式和服務主體，可搭配角色的存取控制使用。
4. 使用 [服務主體 API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)，您可以以程式設計方式管理應用程式的實例，並控制應用程式在您的租使用者中可以執行的作業。
5. [servicePrincipal 資源類型](https://docs.microsoft.com/graph/api/resources/serviceprincipal) 會列出 servicePrincipal 資源類型的所有屬性和方法。
6. [AZURE Ad graph 和 Microsoft graph 之間的資源類型差異](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) 會強調 Azure ad Graph 和 microsoft graph 資源之間的差異。 它會顯示具有不同名稱或無法使用的資源。它也會強調 Microsoft Graph Beta 版中可用的資源，但不是在第1.0 版中。

**來賓使用者的問題**

- [快速入門：將來賓使用者新增至 azure 入口網站中的目錄](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) 顯示如何透過 azure 入口網站將新的來賓使用者新增至 Azure AD 目錄、傳送邀請，以及查看來賓使用者的邀請函兌換處理常式的外觀。
- [教程：在 Azure Active DIRECTORY B2C 中建立使用者資料流程](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) 您可以透過使用 Azure 入口網站來建立某些建議的使用者流程。 如果您正在尋找如何在應用程式中設定資源擁有者密碼認證 (ROPC) 流程的相關資訊，請參閱在 Azure AD B2C 中設定資源擁有者密碼認證流程。
