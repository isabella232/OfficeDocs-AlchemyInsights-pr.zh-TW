---
title: nk2-import-import-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780050"
---
# <a name="how-to-import-nk2-files"></a>如何匯入 nk2 檔案 

當您第一次啟動 Microsoft Outlook 2013、Outlook 2016、Outlook 2019 或 Outlook for Microsoft 365 時，您的昵稱快取快取 (儲存在預設郵件存放區 *中的 nk2*檔案中) 會匯入到隱藏的郵件中。

若要將 nk2 檔案匯入 Outlook 2013、Outlook 2016、Outlook 2019 或 Outlook for Microsoft 365，請確定 nk2 檔案位於下列資料夾中：%appdata%\Microsoft\Outlook

**附注**： nk2 檔案必須與您目前的 outlook 2013 或 outlook 2016 設定檔同名。 設定檔名稱預設為 "Outlook"。 若要檢查設定檔名稱，請遵循下列步驟： 
1. 按一下 **[開始]**，然後按一下 **[控制台]**。
2. 連按兩下 [ **郵件**]。
3. 在 [郵件設定] 對話方塊中，選取 [ **顯示設定檔**]。
4. 選取 [**啟動**  >  **執行**]。
5. 在 [ **開啟** ] 方塊中，輸入 *outlook.exe/importnk2*]，然後選取 **[確定]**。 

當您匯入 nk2 檔之後，檔案的內容會合並至儲存在信箱中的現有昵稱快取。

**附注**：下一次啟動 outlook 2013、outlook 2016、outlook 2019 或 Outlook for Microsoft 365 時，會以 .old 副檔名重新命名 nk2 檔案。 如果想要重新匯入 nk2 檔，請先移除 .old 副檔名。

如需詳細資訊，請參閱匯 [入或複製自動完成清單到另一部電腦](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)。