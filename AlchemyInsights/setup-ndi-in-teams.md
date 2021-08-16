---
title: 開啟 NDI 技術
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
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023513"
---
# <a name="turn-on-ndi-technology"></a>開啟 NDI 技術

NDI 技術需要為使用者開啟兩個步驟：

1. 租使用者管理員必須啟用 CsTeamsMeetingPolicy 中的 ' AllowNDIStreaming ' 屬性。

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. 在此變更填滿之後，使用者必須從 **設定 > 許可權** 中為其特定用戶端開啟 NDI®技術。

如需詳細資訊，請參閱[USE NDI 技術協會 in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)。
