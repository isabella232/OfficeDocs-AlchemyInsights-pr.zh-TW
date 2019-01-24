---
title: 停用的 UPN 同步處理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460606"
---
# <a name="upn-sync-disabled"></a>停用的 UPN 同步處理

如果您啟動同步處理至 Azure AD 之前 2016 年 3 月 30 執行下列 Azure AD PowerShell cmdlet 來啟用 UPN 柔相符的項目僅組織：
  
 **設定 MsolDirSyncFeature-功能 EnableSoftMatchOnUpn-啟用 $True**
  
UPN 柔相符項目會自動開啟啟動同步處理至當天或之後 2016 年 3 月 30，Azure AD 的組織。
  
若要深入了解啟用軟體符合 UPN 與其他的同步處理功能，請參閱[Azure AD 連線同步處理服務功能](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。
  

