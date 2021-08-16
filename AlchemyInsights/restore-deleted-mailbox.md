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
ms.openlocfilehash: 07ad754a927be92ece07f91c5a64d8084c96d0344925467a195033bdd3f445ac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075067"
---
# <a name="restore-a-deleted-mailbox"></a>還原被刪除的信箱

當使用者失去 Exchange Online 授權時，其信箱會保留30天，而且只要重新將授權指派給使用者，就能復原。
  
1. 在 Microsoft 365 系統管理中心中，移至 [**使用者** 作用中 \> **使用者**] 頁面。 選取有問題的使用者。

2. 在 [**授權與應用程式**] 索引標籤上，指派 Exchange Online 授權，然後選取 [**儲存變更**]。

如果您嘗試復原共用信箱或已刪除的使用者，它也可在30天內復原。 您可以在 [ **使用者** \> **刪除的使用者**] 底下找到這些使用者; 共用信箱不需要授權。 請參閱 [還原使用者](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)。

從使用者的信箱復原電子郵件可以由系統管理員進入新的 Exchange 系統[管理中心](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353)。

最後，如果您嘗試復原非使用中的信箱，請 [依照這裡的指示](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox)進行。
  
