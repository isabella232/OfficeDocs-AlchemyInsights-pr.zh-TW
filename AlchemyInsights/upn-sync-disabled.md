---
title: 已停用 UPN 同步處理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726095"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="9d273-102">已停用 UPN 同步處理</span><span class="sxs-lookup"><span data-stu-id="9d273-102">UPN sync disabled</span></span>

<span data-ttu-id="9d273-103">如果您在2016年3月30日之前開始同步處理至 Azure AD，請執行下列 Azure AD PowerShell Cmdlet，只為您的組織啟用 UPN 軟搭配：</span><span class="sxs-lookup"><span data-stu-id="9d273-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="9d273-104">**Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-Enable $True**</span><span class="sxs-lookup"><span data-stu-id="9d273-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="9d273-105">對於在2016年3月30日之後開始同步處理至 Azure AD 的組織，會自動開啟 UPN soft match。</span><span class="sxs-lookup"><span data-stu-id="9d273-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="9d273-106">若要深入瞭解如何在 UPN 和其他同步處理功能上啟用 soft match，請參閱[AZURE AD Connect sync 服務功能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。</span><span class="sxs-lookup"><span data-stu-id="9d273-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

