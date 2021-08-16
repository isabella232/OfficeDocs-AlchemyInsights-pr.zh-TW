---
title: 用來播放影片的 CDN
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: 399be421994437d4cd2df644531334c58d177ec3293e7e379d84cd8326823a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54071107"
---
# <a name="cdn-used-for-video-playback"></a>用來播放影片的 CDN

來自 Stream 和外部應用程式的即時事件或來自 Yammer/Teams 的裝置即時事件，將會自動使用 Azure CDN。 上傳到 Stream 的隨選影片尚未使用 Azure CDN 進行播放。 Stream 中的非即時影片是從與您的租用戶所在地理區域中的租用戶關聯的 Azure Media Services 來源伺服器播放。 如需詳細資訊，請參閱：

- [用來播放影片的 CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
