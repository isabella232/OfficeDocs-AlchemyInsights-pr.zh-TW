---
title: 無法設定或查看 AllowSelfServicePurchase 原則
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735190"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>無法設定或查看 AllowSelfServicePurchase 原則

當您嘗試設定或查看 AllowSelfServicePurchase 原則時，會收到下列錯誤訊息：

*HandleError：無法使用 PolicyId ' AllowSelfServicePurchase ' 取得產品原則，ErrorMessage-基礎 connection 已關閉：傳送時發生意外的錯誤。*

這可能是因為舊版本的傳輸層安全性 (TLS) 。 若要連接 MSCommerce 服務，您必須使用 TLS 1.2 或更新版本。  

請嘗試下列步驟，將 TLS 通訊協定啟用/設定為1.2、驗證及重試。
 1. 在 PowerShell 命令提示字元處 (PS C： \) 輸入下列命令，將 TLS 通訊協定設定為版本1.2：

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. 使用下列命令，確認 TLS 通訊協定 (s) 在使用中：

    `[Net.ServicePointManager]::SecurityProtocol` 

3. 視需要重試 Get 或 Update 命令。

