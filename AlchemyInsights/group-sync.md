---
title: 群組同步
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 7e5ed69c34f8e7b922d7eef202af508152a7e04d7773581b32e43395571c6fbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53987638"
---
# <a name="group-sync"></a>群組同步

本文提供群組同步的相關指導方針。

1. 如果全域系統管理員或群組擁有者無法在 Azure 入口網站中修改群組屬性或新增成員或指派擁有者，請確認群組的授權來源為 Azure Active Directory (Azure AD)，全域系統管理員或群組擁有者才能修改該群組。
2. 嘗試刪除 Azure AD 中已同步的群組之前，請先確認您已[刪除所有指派的授權](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced)，以避免錯誤。

若要了解如何同步使用者、群組和連絡人，請參閱 [Azure AD Connect 同步](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)，並遵循[使用 Azure AD Connect 將內部部署群組同步到 Azure](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) 的步驟，以使用 AD Connect 同步內部部署群組。

遵循此指南[疑難排解同步期間的錯誤](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors)，以疑難排解同步期間的常見錯誤。

