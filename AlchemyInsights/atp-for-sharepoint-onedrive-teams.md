---
title: 適用於 SharePoint、OneDrive 及 Microsoft Teams 的 ATP
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508403"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>適用於 SharePoint、OneDrive 及 Microsoft Teams 的 ATP

請遵循下列步驟來啟用高級威脅防護：

1. 移至 [https://protection.office.com](https://protection.office.com) 並以全域管理員或安全性管理員帳戶登入。

2. 在 [**威脅管理**] 底下的左側流覽窗格中，選擇 [**原則** \> **安全附件**]。

3. 選取 **[開啟適用於 SharePoint、OneDrive 與 Microsoft Teams 的 ATP]**。

4. [建立活動警示原則](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts)，以在我們偵測到惡意檔時收到通知。

如需完整指示，請參閱本[主題](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)。

**附注**：依設計，ATP 不會掃描 SharePoint Online、商務 OneDrive 或 Microsoft 小組中的每一個檔案。 使用共用活動、訪客活動及威脅信號來識別惡意檔案的處理常式會以非同步方式掃描檔案。 如需詳細資訊，請參閱本[主題](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。
