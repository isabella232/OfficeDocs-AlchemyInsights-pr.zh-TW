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
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532322"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="3184a-102">停用的 UPN 同步處理</span><span class="sxs-lookup"><span data-stu-id="3184a-102">UPN sync disabled</span></span>

<span data-ttu-id="3184a-103">如果您啟動同步處理到 Azure AD 之前 2016 年 3 月 30 日，執行下列 Azure AD PowerShell cmdlet 啟用 UPN 為您的組織只有 [柔相符項目：</span><span class="sxs-lookup"><span data-stu-id="3184a-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="3184a-104">**設定 MsolDirSyncFeature-功能 EnableSoftMatchOnUpn-啟用 $True**</span><span class="sxs-lookup"><span data-stu-id="3184a-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="3184a-105">UPN 柔相符項目會自動開啟啟動同步處理到 Azure AD 上或在 2016 年 3 月 30 日之後的組織。</span><span class="sxs-lookup"><span data-stu-id="3184a-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="3184a-106">若要深入了解啟用的 UPN 與其他同步處理功能的軟性相符項目，請參閱[Azure AD Connect 同步處理服務功能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。</span><span class="sxs-lookup"><span data-stu-id="3184a-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

