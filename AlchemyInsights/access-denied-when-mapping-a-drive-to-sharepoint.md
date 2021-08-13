---
title: 將磁片對應至 SharePoint 時，存取權遭到拒絕
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 1ed67ec926c3e73f7a16b927729255505dfe93a0ae442a5dff9400afafb41d8e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938722"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>修正對應至網路磁碟機的 SharePoint 程式庫的問題

當您流覽到對應的網路磁碟機時，可能會出現下列其中一則訊息：
  
- **\\無法存取路徑。您可能沒有使用此網路資源的許可權。請洽詢此伺服器的管理員，以找出您是否有存取許可權。**

- **拒絕存取。在此位置開啟檔案之前，您必須先將網站新增至信任的網站清單，流覽至網站，然後選取 [自動登入] 選項。**

[取得協助疑難排解對應的網路磁碟機](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)。
  
將文件庫對應為網路磁碟機，只會在 Internet Explorer 中進行暫存和支援。 相反地，請[使用新的 OneDrive 同步處理用戶端](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)（包括所[需的](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)檔案）同步處理 SharePoint 檔案。 不必使用本機儲存空間，即可在 OneDrive 中存取所有檔案。
  