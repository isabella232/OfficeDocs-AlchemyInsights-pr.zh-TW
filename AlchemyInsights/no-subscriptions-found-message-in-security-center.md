---
title: 資訊安全中心的找不到訂閱訊息
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768419"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>資訊安全中心的找不到訂閱訊息

如果在存取 Microsoft Defender 資訊安全中心時收到「找不到訂閱」訊息，表示用來將該使用者登入入口網站的 Azure Active Directory (AAD) 沒有 Microsoft Defender ATP 授權。  

Windows E5 和 Office E5 授權是不同的授權。

如果已購買授權，但該授權未佈建給此 AAD 執行個體，請開啟支援案例。 您可能發生以下兩個情況之一： <br/>
-   可能發生授權佈建問題。<br/>
-   您不慎將授權佈建給與用來向服務進行驗證的 Microsoft AAD 不同的 Microsoft AAD。