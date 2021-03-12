---
title: 存取拒絕郵件的疑難排解
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704885"
---
# <a name="troubleshoot-access-denied-messages"></a>存取拒絕郵件的疑難排解

如果有人收到「拒絕存取」訊息給 SharePoint 中的共用資料夾，則網站集合管理員可能已啟用「限制存取」使用者許可權鎖定模式。」 若要關閉此功能： 
  
1. 流覽至網站，按一下 [設定] 圖示，然後按一下 [ **網站設定**]。
    
2. 按一下 [網站集合管理] 下方的 [網站集合功能]。
    
3. 在 [ **限制存取] 使用者許可權鎖定模式** 旁，按一下 [ **停用**]。
    
如果網站是發佈網站，也可以對共用資料夾進行存取被拒絕的訊息。 如需詳細資訊，請參閱 [存取共用資料夾時拒絕存取](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)。
  
在嘗試查看存取要求時，如果有人收到「拒絕存取」訊息，使用者必須新增為網站集合管理員或網站擁有者群組的成員。 如需詳細資訊，請參閱拒絕存取「 [存取要求」清單](https://go.microsoft.com/fwlink/?linkid=2004220)。
  
若使用者從內部部署的 Active Directory 中移除之後收到「拒絕存取」訊息，並將其新增回來，請參閱 [在將使用者帳戶同步處理至 Microsoft 365 時，存取權被拒絕](https://go.microsoft.com/fwlink/?linkid=2004318)。
  

