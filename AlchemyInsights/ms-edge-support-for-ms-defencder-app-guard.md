---
title: Microsoft Edge 對 Microsoft Defender 應用程式防護的支援
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576437"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edge 對 Microsoft Defender 應用程式防護的支援

針對 Windows 10 和 Microsoft Edge 設計，Application Guard 使用硬體隔離方法，可讓使用者從主機作業系統分開的隔離的 Hyper-V 容器內流覽不可信的網站。

企業系統管理員會定義信任的網站、雲端資源和內部網路的清單。 當使用者訪問不在清單上的網站時，Microsoft Edge 會在容器中開啟網站。 這表示，如果網站會變成惡意的電腦，則主機電腦將保持受保護狀態，而攻擊者將無法取得企業資料。

在 Microsoft Edge 版本81中支援在容器中安裝分機，而且可以透過原則加以控制。 ExtensionInstallForcelist 原則中所使用的 updateURL 位址，應新增為應用程式防護所使用之網路隔離原則中的非特定資源。

如需詳細資訊，請參閱 microsoft [Defender Application Guard 的 Microsoft Edge support](https://go.microsoft.com/fwlink/?linkid=2134229)。
