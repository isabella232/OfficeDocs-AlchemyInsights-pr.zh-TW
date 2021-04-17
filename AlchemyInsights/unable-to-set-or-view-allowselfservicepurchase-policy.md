---
title: 無法設定或查看 AllowSelfServicePurchase 原則
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826082"
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

