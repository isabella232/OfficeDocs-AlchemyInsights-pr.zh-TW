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
ms.openlocfilehash: 2d5f0486ed8d4cbd95603f223bc0e48c4dcf38abb001d1616ca968b1d6bba7de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044223"
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

如需部署端點 DLP 的其他需求，請參閱[開始使用端點資料外洩防護](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)。