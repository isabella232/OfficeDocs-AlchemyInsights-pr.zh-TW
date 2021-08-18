---
title: 端點 DLP 未部署至使用者的裝置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 56783b007b5eebc7ca671247f24f5b513b9d8f5c321f59a63170425c2d376a94
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900239"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>端點 DLP 未部署至使用者的裝置

如果端點資料外洩防護 (DLP) 設定尚未套用至使用者的裝置，請確認您符合這些需求：

- Windows 10 x64 組建 1809 或更新版本已安裝在裝置上。
- 已安裝反惡意程式碼用戶端版本 4.18.2009.7 或更新版本。
- 裝置為以下 **其中一種**：
    
    - 已使用 Azure Active Directory (Azure AD) 而聯結的
    - 已使用混合式 Azure AD 而聯結的
    - AAD 已註冊

- 若要強制執行原則動作，請確定端點裝置上已安裝 Microsoft Chromium Edge 瀏覽器。

如需部署端點 DLP 的其他需求，請參閱[開始使用端點資料外洩防護](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)。