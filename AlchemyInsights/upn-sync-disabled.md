---
title: 已停用 UPN 同步處理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749505"
---
# <a name="upn-sync-disabled"></a>已停用 UPN 同步處理

如果您在2016年3月30日之前開始同步處理至 Azure AD，請執行下列 Azure AD PowerShell Cmdlet，只為您的組織啟用 UPN 軟搭配：
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-Enable $True**
  
對於在2016年3月30日之後開始同步處理至 Azure AD 的組織，會自動開啟 UPN soft match。
  
若要深入瞭解如何在 UPN 和其他同步處理功能上啟用 soft match，請參閱 [AZURE AD Connect sync 服務功能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。
  

