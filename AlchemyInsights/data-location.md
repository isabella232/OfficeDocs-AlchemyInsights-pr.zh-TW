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
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207252"
---
# <a name="data-location"></a><span data-ttu-id="3e4b2-102">資料位置</span><span class="sxs-lookup"><span data-stu-id="3e4b2-102">Data location</span></span>

<span data-ttu-id="3e4b2-103">在系統管理中心或連線到 Exchange Online 透過 PowerShell，您可以檢視您的 Office 365 租用戶的位置。</span><span class="sxs-lookup"><span data-stu-id="3e4b2-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="3e4b2-104">**系統管理中心：**</span><span class="sxs-lookup"><span data-stu-id="3e4b2-104">**Admin center:**</span></span>
1. <span data-ttu-id="3e4b2-105">登入[系統管理中心](https://admin.microsoft.com/Adminportal/Home)。</span><span class="sxs-lookup"><span data-stu-id="3e4b2-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="3e4b2-106">選取 [**設定** > **組織設定檔**。</span><span class="sxs-lookup"><span data-stu-id="3e4b2-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="3e4b2-107">在 [**資料位置**]，選取 [**檢視詳細資料**]。</span><span class="sxs-lookup"><span data-stu-id="3e4b2-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="3e4b2-108">**PowerShell:**</span><span class="sxs-lookup"><span data-stu-id="3e4b2-108">**PowerShell:**</span></span>
1. <span data-ttu-id="3e4b2-109">使用 Windows PowerShell 連線到 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="3e4b2-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="3e4b2-110">執行[Get-organizationalunit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit)指令程式，來顯示您的租用戶內容的清單。</span><span class="sxs-lookup"><span data-stu-id="3e4b2-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="3e4b2-111">查看 OrganizationId 屬性。</span><span class="sxs-lookup"><span data-stu-id="3e4b2-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="3e4b2-112">當您有 EXO 和 SPO 的資料位置時，您可以判斷您可能會從[您的資料所在的位置](https://products.office.com/where-is-your-data-located)使用其他服務的資料位置。</span><span class="sxs-lookup"><span data-stu-id="3e4b2-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>