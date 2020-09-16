---
title: 用來播放影片的 CDN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: 6bc87783375a206a84c96eb7ddd58db5bfd31728
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756958"
---
# <a name="cdn-used-for-video-playback"></a>用來播放影片的 CDN

來自 Stream 和外部應用程式的即時事件或來自 Yammer/Teams 的裝置即時事件，將會自動使用 Azure CDN。 上傳到 Stream 的隨選影片尚未使用 Azure CDN 進行播放。 Stream 中的非即時影片是從與您的租用戶所在地理區域中的租用戶關聯的 Azure Media Services 來源伺服器播放。 如需詳細資訊，請參閱：

- [用來播放影片的 CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
