---
title: 適用於 Office 365 的 Microsoft Defender，適用於 SharePoint、OneDrive 和 Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: c42786559d527a5ef9a0a8cfad1476f4d122b6d5570ca5b9ea138b21a153ae96
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896326"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>適用於 Office 365 的 Microsoft Defender，適用於 SharePoint、OneDrive 和 Microsoft Teams

請遵循下列步驟，為 Office 365 啟用 Microsoft Defender：

1. 移至 [https://protection.office.com](https://protection.office.com) 並以全域管理員或安全性管理員帳戶登入。

2. 在 [**威脅管理**] 底下的左側流覽窗格中，選擇 [**原則** \> **保管庫附件**]。

3. **針對 SharePoint、OneDrive 及 Microsoft Teams，選取 [為 Office 365 開啟 Defender**]。

4. [建立活動警示原則](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) ，以在我們偵測到惡意檔時收到通知。

如需完整的指示，請參閱[開啟 SharePoint、OneDrive 和 Microsoft Teams 的保管庫附件](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)。

**附注**：依設計，Microsoft Defender for Office 365 不會掃描 SharePoint Online、商務用 OneDrive 或 Microsoft Teams 中的每一個檔案。 使用共用活動、訪客活動及威脅信號來識別惡意檔案的處理常式會以非同步方式掃描檔案。 如需詳細資訊，請參閱[保管庫 SharePoint、OneDrive 和 Microsoft Teams 的附件](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。
