---
title: 還原已刪除的信箱
ms.author: pebaum
author: pebaum
ms.date: 9/12/2017
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 92761e4679a155781555daec023ee9602d62a857
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35356084"
---
# <a name="restore-a-deleted-mailbox"></a>還原被刪除的信箱

當使用者失去其 Exchange Online 授權時, 其信箱會保留30天, 而且只要重新指派授權給使用者, 即可進行復原。
  
 *這只會在30天內運作。*  在管理入口網站中, 移至:
  
1. **使用者**\> **** 作用中的使用者。 選取 [有問題的使用者]。

2. 按 [**編輯**] 修改產品授權

3. 指派 Exchange Online 授權, 然後按 [**儲存**]

如果您嘗試復原共用信箱, 它也可在30天內復原。 您可以在 [**使用者** \> **已刪除**的使用者] 底下找到它們。共用信箱不需要授權。 如果您意識到您需要還原已刪除的使用者, 請參閱[restore a user In Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user)。
  