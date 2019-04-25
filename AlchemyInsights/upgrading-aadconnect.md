---
title: 932 升級 AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389654"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="d954c-102">升級 Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d954c-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="d954c-103">根據預設，自動升級為啟用，這有助於確保您正在執行最新版的 Azure AD Connect。</span><span class="sxs-lookup"><span data-stu-id="d954c-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="d954c-104">若要確認自動升級的設定，請使用**Get-ADSyncAutoUpgrade** cmdlet Azure AD PowerShell 中。</span><span class="sxs-lookup"><span data-stu-id="d954c-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="d954c-105">此 cmdlet 會傳回下列值之一：</span><span class="sxs-lookup"><span data-stu-id="d954c-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="d954c-106">**Enabled**： 啟用自動升級。</span><span class="sxs-lookup"><span data-stu-id="d954c-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="d954c-107">**停用**： 停用自動升級。</span><span class="sxs-lookup"><span data-stu-id="d954c-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="d954c-108">**擱置**： 系統已不再適用獲得自動升級。</span><span class="sxs-lookup"><span data-stu-id="d954c-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="d954c-109">您無法設定這個值;它是由系統設定。</span><span class="sxs-lookup"><span data-stu-id="d954c-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="d954c-110">如需詳細資訊，請參閱[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)。</span><span class="sxs-lookup"><span data-stu-id="d954c-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="d954c-111">若要下載最新版的 Azure AD Connect，移至[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)。</span><span class="sxs-lookup"><span data-stu-id="d954c-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
