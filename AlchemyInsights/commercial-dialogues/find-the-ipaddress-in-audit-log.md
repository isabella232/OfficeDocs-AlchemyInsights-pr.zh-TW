---
title: 在審計記錄檔中尋找 IP 位址
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303568"
---
# <a name="find-the-ip-address-in-audit-log"></a>在審計記錄檔中尋找 IP 位址

對應至使用者或系統管理員所執行之活動的 IP 位址會顯示在審計記錄檔中。 也會記錄用戶端資訊。 以下說明如何識別 IP 位址：

1. 請執行下列其中一個動作：
   - 在 Microsoft 365 合規性中心 <https://compliance.microsoft.com> ，移至 [**解決方案** \> **審核**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com> ，移至 [**審計**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://security.microsoft.com/auditlogsearch> 。

    **附注**：如果您看到需要開啟審計的通知，請繼續進行，然後立即開啟。 如果未啟用此功能，搜尋結果將無法從先前的日期提取資料。

2. 在 [ **審計** ] 頁面上，確認已選取 [ **搜尋] 索引** 標籤，然後設定下列設定：
   - **日期和時間範圍**：選取 [ **開始** ] 和 [ **結束** ] 方塊中的 [日期/時間範圍]。
   - **活動**：如果您對特定的活動感興趣，請從清單中進行選取，然後按一下 [是]。否則，預設值會 **顯示所有活動的結果** 會傳回所有活動。 請注意，選取某些動作可能無法供選取;不過，如果已選取 [ **顯示所有活動的結果** ]，就會傳回這些審計專案。
   - **使用者**：接受空白預設值以傳回所有使用者的結果，或輸入一或多個使用者。

3. 完成後，請按一下 [ **搜尋**]。 活動會顯示在 [新的 **審計搜尋** ] 頁面上。

4. 在結果中，按一下 [ **篩選結果** ]，然後在 [活動篩選] 方塊中輸入 **Set-Mailbox** 。

5. 選取結果中的審計記錄，以開啟 [ **詳細資料** ] 快顯視窗。

如需詳細資訊，請參閱 [搜尋審核記錄檔以調查常見的支援問題](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。
