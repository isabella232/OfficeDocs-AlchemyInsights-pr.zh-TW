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
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921699"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="eaf84-102">停用的 UPN 同步處理</span><span class="sxs-lookup"><span data-stu-id="eaf84-102">UPN sync disabled</span></span>

<span data-ttu-id="eaf84-103">如果您啟動同步處理至 Azure AD 之前 2016 年 3 月 30 執行下列 Azure AD PowerShell cmdlet 來啟用 UPN 柔相符的項目僅組織：</span><span class="sxs-lookup"><span data-stu-id="eaf84-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="eaf84-104">**設定 MsolDirSyncFeature-功能 EnableSoftMatchOnUpn-啟用 $True**</span><span class="sxs-lookup"><span data-stu-id="eaf84-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="eaf84-105">UPN 柔相符項目會自動開啟啟動同步處理至當天或之後 2016 年 3 月 30，Azure AD 的組織。</span><span class="sxs-lookup"><span data-stu-id="eaf84-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="eaf84-106">若要深入了解啟用軟體符合 UPN 與其他的同步處理功能，請參閱[Azure AD 連線同步處理服務功能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。</span><span class="sxs-lookup"><span data-stu-id="eaf84-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

