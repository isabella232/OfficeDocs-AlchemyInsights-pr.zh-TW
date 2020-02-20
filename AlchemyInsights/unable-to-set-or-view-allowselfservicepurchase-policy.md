---
title: 無法設定或檢視 AllowSelfServicePurchase 原則
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158551"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>無法設定或檢視 AllowSelfServicePurchase 原則

當嘗試設定或檢視 AllowSelfServicePurchase 原則，您會收到下列錯誤訊息：

*HandleError： 無法擷取產品原則與 PolicyId 'AllowSelfServicePurchase' ErrorMessage-基礎連接已關閉： 傳送發生意外的錯誤。*

這可能是由於較舊版本的傳輸層安全性 (TLS)。 若要連接的 MSCommerce 服務，您需要使用 TLS 1.2 或更高版本。  

請嘗試下列步驟來啟用/集 1.2 TLS 通訊協定、 確認，然後重試。
 1. 在 PowerShell 命令提示字元 (PS C:>\)輸入下列命令，以 TLS 通訊協定設 1.2 版：

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. 確認 TLS 通訊協定，在使用中，使用下列命令：

    `[Net.ServicePointManager]::SecurityProtocol` 

3. 視需要再試一次 [取得] 或 [更新命令。

