---
title: 932升級 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104803"
---
# <a name="upgrade-azure-ad-connect"></a>升級 Azure AD 連線

根據預設，會針對 Azure AD 連線啟用自動升級，這有助於確保您執行的是最新版本。 若要驗證自動升級設定，請使用 Azure AD PowerShell 中的 **ADSyncAutoUpgrade** Cmdlet。 Cmdlet 會傳回下列其中一個值：

- **Enabled**：已啟用自動升級。

- **Disabled**：已停用自動升級。

- 已 **擱置**：系統無法再接收自動升級。 您無法設定此值;它是由系統設定。

如需詳細資訊，請參閱 [自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)。

若要下載最新版本的 Azure AD 連線，請移至 [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) 。
