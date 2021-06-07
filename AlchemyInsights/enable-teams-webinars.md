---
title: 啟用 Teams 網路研討會
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760836"
---
# <a name="enable-teams-webinars"></a>啟用 Teams 網路研討會

預設啟用網路研討會。 您可以透過使用 Teams PowerShell 命令管理可以排程和註冊 Teams 網路研討會的人員。

- 所有可以建立會議的使用者也可以建立網路研討會會議。 如果您想要管理可以排程 Teams 網路研討會的人員，請使用 *AllowMeetingRegistration*。 
- 根據預設，*WhoCanRegister* 為啟用狀態且設為 **所有人**。 如果您想要關閉會議註冊，請將 *AllowMeetingRegistration* 設為 **FALSE**。

若要變更這些設定，您必須安裝 [Teams PowerShell](/microsoftteams/teams-powershell-install)。 同時，會議原則會在 Teams 網路研討會上強制執行。 舉例來說，如果在會議設定將匿名參加設為關閉，匿名使用者就無法參加網路研討會。

若要深入了解設定可以註冊網路研討會的人員，請參閱 [設定可以註冊網路研討會的人員](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)。 如需 Microsoft 清單設定的詳細資料，請參閱 [控制 Microsoft 清單設定](/sharepoint/control-lists)。