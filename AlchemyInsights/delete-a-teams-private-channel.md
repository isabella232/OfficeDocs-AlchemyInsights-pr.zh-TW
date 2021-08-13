---
title: 刪除 Teams 私人頻道
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 33bf8a5cdc3a8e8da78c9d02e11387a778a7acce483e4485f595d9e05b344433
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948262"
---
# <a name="delete-a-teams-private-channel"></a>刪除 Teams 私人頻道

如果您為基礎 SharePoint 網站啟用了SharePoint 保留原則，則 Microsoft 會注意到删除 Teams 私人頻道時出現的問題。 Microsoft 正在想辦法修正這個問題。 與此同時，您可以使用下列因應措施刪除私人頻道。

**從 Sharepoint 保留原則中排除小組/網站集合。**

1. 移至 Office 365 系統管理員入口網站，然後選取左側流覽窗格中的 **[顯示所有]**。
2. 在 **[系統管理中心]** 中，移至 **[安全性與合規性]** > **[資料遺失防護]** > **[原則]**。
3. 識別任何適用於 Sharepoint 網站的原則，並修改該原則，使包含私人頻道的團隊的 Sharepoint 網站不包含在保留原則下。
4. 儲存原則。
    原則設定最多可能需要 24 小時才能生效。
    排除網站之後，您可以刪除私人頻道。  
    
您 ***可能*** 可以在 Android 裝置上使用 Microsoft Teams 來刪除私人頻道。 

如需相關的 SharePoint 資訊，請參閱[無法刪除 SharePoint Online 或商務用 OneDrive 中的項目](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)。