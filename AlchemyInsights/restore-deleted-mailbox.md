---
title: 還原已刪除的信箱
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 284024bdf9728e8463fe69ef9c9c2695035faf2f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511355"
---
# <a name="restore-a-deleted-mailbox"></a>還原被刪除的信箱

當使用者失去 Exchange Online 授權時，其信箱會保留30天，而且只要重新將授權指派給使用者，就能復原。
  
 *這只會在30天內運作。*  
  
1. 在 Microsoft 365 系統管理中心中，移至 [**使用者**作用中 \> **使用者**] 頁面。 選取有問題的使用者。

2. 在 [**授權與應用程式**] 索引標籤上，指派 Exchange Online 授權，然後選取 [**儲存變更**]。

如果您嘗試復原共用信箱，它也可在30天內復原。 您可以在 [**使用者** \> **刪除的使用者**] 底下找到這些使用者; 共用信箱不需要授權。 如果您知道需要還原已刪除的使用者，請參閱[還原使用者](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)。
  