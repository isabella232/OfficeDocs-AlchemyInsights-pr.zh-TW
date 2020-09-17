---
title: 932升級 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806030"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="74687-102">升級 Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="74687-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="74687-103">根據預設，會針對 Azure AD Connect 啟用自動升級，這有助於確保您執行的是最新版本。</span><span class="sxs-lookup"><span data-stu-id="74687-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="74687-104">若要驗證自動升級設定，請使用 Azure AD PowerShell 中的 **ADSyncAutoUpgrade** Cmdlet。</span><span class="sxs-lookup"><span data-stu-id="74687-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="74687-105">Cmdlet 會傳回下列其中一個值：</span><span class="sxs-lookup"><span data-stu-id="74687-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="74687-106">**Enabled**：已啟用自動升級。</span><span class="sxs-lookup"><span data-stu-id="74687-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="74687-107">**Disabled**：已停用自動升級。</span><span class="sxs-lookup"><span data-stu-id="74687-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="74687-108">已**擱置**：系統無法再接收自動升級。</span><span class="sxs-lookup"><span data-stu-id="74687-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="74687-109">您無法設定此值;它是由系統設定。</span><span class="sxs-lookup"><span data-stu-id="74687-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="74687-110">如需詳細資訊，請參閱 [自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)。</span><span class="sxs-lookup"><span data-stu-id="74687-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="74687-111">若要下載最新版本的 Azure AD Connect，請移至 [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) 。</span><span class="sxs-lookup"><span data-stu-id="74687-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
