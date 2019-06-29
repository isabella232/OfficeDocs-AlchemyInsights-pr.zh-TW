---
title: 932升級 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365881"
---
# <a name="upgrade-azure-ad-connect"></a>升級 Azure AD Connect

根據預設, 會為 Azure AD Connect 啟用自動升級, 這有助於確保您執行的是最新版本。 若要驗證自動升級設定, 請在 Azure AD PowerShell 中使用**ADSyncAutoUpgrade** Cmdlet。 此 Cmdlet 會傳回下列其中一個值:

- **Enabled**: 啟用自動升級。

- **Disabled**: 已停用自動升級。

- 已**擱置**: 系統無法再接受自動升級。 您無法設定此值;它是由系統所設定。

如需詳細資訊, 請參閱[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)。

若要下載最新版本的 Azure AD Connect, 請[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)移至。
