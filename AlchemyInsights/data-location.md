---
title: 資料位置
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655273"
---
# <a name="data-location"></a><span data-ttu-id="7bf9b-102">資料位置</span><span class="sxs-lookup"><span data-stu-id="7bf9b-102">Data location</span></span>

<span data-ttu-id="7bf9b-103">您可以在系統管理中心中查看租使用者的位置，或透過 PowerShell 連接至 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="7bf9b-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="7bf9b-104">**系統管理中心：**</span><span class="sxs-lookup"><span data-stu-id="7bf9b-104">**Admin center:**</span></span>
1. <span data-ttu-id="7bf9b-105">登入系統[管理中心](https://admin.microsoft.com/Adminportal/Home)。</span><span class="sxs-lookup"><span data-stu-id="7bf9b-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="7bf9b-106">選取 [**設定** > **組織設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="7bf9b-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="7bf9b-107">在 [**資料位置**] 底下，選取 [**查看詳細**資料]。</span><span class="sxs-lookup"><span data-stu-id="7bf9b-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="7bf9b-108">**PowerShell:：**</span><span class="sxs-lookup"><span data-stu-id="7bf9b-108">**PowerShell:**</span></span>
1. <span data-ttu-id="7bf9b-109">使用 Windows PowerShell 連接至 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="7bf9b-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="7bf9b-110">執行[Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) Cmdlet 以顯示租使用者屬性的清單。</span><span class="sxs-lookup"><span data-stu-id="7bf9b-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="7bf9b-111">查看 OrganizationId 屬性。</span><span class="sxs-lookup"><span data-stu-id="7bf9b-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="7bf9b-112">當您有 EXO 和 SPO 的資料位置時，您可以判斷您的[資料所在位置](https://products.office.com/where-is-your-data-located)，您可以使用其他服務的資料位置。</span><span class="sxs-lookup"><span data-stu-id="7bf9b-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>