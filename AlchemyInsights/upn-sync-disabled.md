---
title: 停用的 UPN 同步處理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767210"
---
# <a name="upn-sync-disabled"></a>停用的 UPN 同步處理

如果您啟動同步處理到 Azure AD 之前 2016 年 3 月 30 日，執行下列 Azure AD PowerShell cmdlet 啟用 UPN 為您的組織只有 [柔相符項目：
  
 **設定 MsolDirSyncFeature-功能 EnableSoftMatchOnUpn-啟用 $True**
  
UPN 柔相符項目會自動開啟啟動同步處理到 Azure AD 上或在 2016 年 3 月 30 日之後的組織。
  
若要深入了解啟用的 UPN 與其他同步處理功能的軟性相符項目，請參閱[Azure AD Connect 同步處理服務功能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。
  

