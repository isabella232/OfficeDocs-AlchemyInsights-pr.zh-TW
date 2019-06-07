---
title: 932 升級 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757282"
---
# <a name="upgrade-azure-ad-connect"></a>升級 Azure AD Connect

根據預設，自動升級為啟用，這有助於確保您正在執行最新版的 Azure AD Connect。 若要確認自動升級的設定，請使用**Get-ADSyncAutoUpgrade** cmdlet Azure AD PowerShell 中。 此 cmdlet 會傳回下列值之一： 

- **Enabled**： 啟用自動升級。

- **停用**： 停用自動升級。

- **擱置**： 系統已不再適用獲得自動升級。 您無法設定這個值;它是由系統設定。 

如需詳細資訊，請參閱[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)。

若要下載最新版的 Azure AD Connect，移至[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)。
