---
title: Endpoint DLP 授權錯誤
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322122"
---
# <a name="endpoint-dlp-licensing-error"></a>Endpoint DLP 授權錯誤

嘗試設定端點 DLP 時，如果您收到下列錯誤：

`Your organization is missing the licenses required to manage these devices`.

確定您有下列其中一項訂閱或附加元件：

- Microsoft 365 E5
- Microsoft 365 A5 (教育版)
- Microsoft 365 E5 合規性
- Microsoft 365 A5 合規性
- Microsoft 365 E5 資訊保護和控管
- Microsoft 365 A5 資訊保護和控管

**附注**：這不適用於授權組合，如： Win E5 + O365 E5 + EMS e5。 您必須具有純 M365 E5 授權，才能設定此功能。

如需更多 Endpoint DLP 授權資訊，請參閱 [ENDPOINT DLP 授權。](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
