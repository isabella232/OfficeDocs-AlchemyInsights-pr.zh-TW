---
title: Mac 版 Teams 增益集
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2020
ms.locfileid: "46617056"
---
# <a name="teams-add-in-for-mac"></a>Mac 版 Teams 增益集

若要為 Mac 作業系統使用者疑難排解遺漏 Teams 增益集的問題，請遵循下列步驟：

**步驟 1：** 如果您使用混合式 Exchange 內部部署 (需要 2016 CU3 或更新版本)，請使用 Test-HMA.ps1 工具來確認已正確設定混合式新式驗證。 如需詳細資訊，請參閱[針對 iOS 和 Android 版 Outlook 驗證混合式新式驗證設定](https://aka.ms/AA980zq)。  

**注意：** 使用 UPN 位址格式 (例如，[username@contoso.com](mailto:username@contoso.com))，而非domain\username。 執行此動作，即使是對擁有 Exchange Online 信箱的使用者也這麼做。

**步驟 2：** 讓使用者在 Mac 版 Outlook 中移至 [工具 **]**  >  [帳戶 **]**，然後尋找並選取帳戶。 確認列出的使用者名稱為 UPN 格式 (例如，[username@contoso.com](mailto:username@contoso.com))。

**步驟 3：** 確認使用者為取得授權的 Microsoft Teams 使用者。 使用者必須使用 Mac 版 Office 365 訂閱，產品版本 16.24 或更新版本。