---
title: OneDrive 登入錯誤 AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947485"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive 登入錯誤 AADSTS50011

如果您收到錯誤 "AADSTS50011：登入 OneDrive app 時，要求中指定的回復 URL 與回復不符"，請檢查下列各項：

您的 OneDrive 版本必須等於或大於20.052 版本。Xxxx。 若要檢查您的版本，請按一下 [通知] 區域中的 [藍色 OneDrive] 圖示，然後選取 [ **説明] & 設定] > 設定 >** 。

您的網路可能會封鎖流量， **g.live.com** 和 **oneclient.sfx.ms** 。 如果流量遭到封鎖，OneDrive 無法自行更新。 請與您的網路系統管理員合作，以確保您可以存取這些 URLs。 使用 Microsoft 365 方案的客戶應該可以存取[這些端點](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide)。

如果您需要手動取得目前版本的 OneDrive，請造訪 [https://aka.ms/getonedrive](https://aka.ms/getonedrive) 。
