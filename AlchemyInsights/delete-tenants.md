---
title: 刪除租使用者
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993884"
---
# <a name="delete-tenant"></a>刪除租使用者

若要刪除 Azure AD，請確定：
- 您是目錄上的全域系統管理員。
- 您未使用具有預設目錄（如 contoso.onmicrosoft.com）的帳戶登入已登入的帳戶，例如 admin@contoso.onmicrosoft.com。
- 在刪除之前，移除目錄中的任何使用中應用程式。 若要移除作用中的應用程式，請流覽至應用程式註冊，並移除現有的應用程式。
- 任何 Microsoft 線上服務（如 Microsoft Azure、Office 365 或目錄上的 Azure AD Premium 相關聯）都沒有作用中的訂閱。 透過 Azure 支援和帳單轉接您的訂閱或加急取消使用中的訂閱。 深入瞭解如何取消 Office 365 和 Azure 訂閱。 如需關聯或將現有訂閱新增至租使用者的指引，請參閱 [關聯或加入 AZURE AD 租使用者的 azure 訂閱](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)。
- 沒有主動授權。 若要移除授權，請參閱 how [to Remove 訂閱 To remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)。
- 在嘗試刪除 Azure AD 時，在目錄中沒有其他作用中的使用者，而是以全域系統管理員身分。 移除任何其他作用中的使用者，而且也需要移除租使用者的自訂功能變數名稱上的任何相依性，例如使用 admin@contoso.com 建立的使用者。

如需更詳細的步驟，請執行下列操作：
- 刪除 "Azure Active Directory" 或 "訂閱"，請參閱[Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)。
- 移除目錄中的應用程式，請參閱 [移除應用程式](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)。 
