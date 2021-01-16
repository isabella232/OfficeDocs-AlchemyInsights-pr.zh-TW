---
title: 將群組指派給 Azure AD 角色
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875364"
---
# <a name="assigning-groups-to-azure-ad-role"></a>將群組指派給 Azure AD 角色

若要將 Azure AD 群組和 Azure AD 中的授權單位來源指派給 Azure AD 角色，請執行下列步驟：

1. 選立新群組 - 若要建立新的群組：

    a. 以 **特殊權限角色管理員** 或 **全域系統管理員** 權限登入 Azure AD 系統管理中心。
    b. 選取 **[Azure Active Directory] > [群組] > [所有群組] > [新增群組]**。
    c. 建立群組。

2. 在建立群組期間或建立群組之後，將角色指派給群組。

    a. 若要在建立群組時，將角色指派給群組，請切換 **[可以將 Azure AD 角色指派給群組]** 並建立群組。
    b. 若要在建立群組之後，將角色指派給該群組，請瀏覽至新建立群組的 **[指派的角色]** 索引標籤，然後將角色指派給群組。  

**管理指派給 Azure AD 角色的群組成員資格**

若要防止提高權限，根據預設，只有特殊權限管理員和全域系統管理員可以修改指派角色的群組成員資格。 不過，他們可以選擇指派群組的擁有者，並委派這個工作。

如需將雲端群組指派給 Azure AD 角色的詳細資訊，請參閱[將 AD 角色指派給雲端群組](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) (部分機器翻譯)。 如需疑難排解將角色指派給雲端群組的詳細資料，請參閱 [疑難排解將角色指派給雲端群組](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting) (部分機器翻譯)。





