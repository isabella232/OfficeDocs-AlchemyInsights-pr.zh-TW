---
title: 檢視工作流程時拒絕存取
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460598"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="fcd06-102">檢視工作流程時拒絕存取</span><span class="sxs-lookup"><span data-stu-id="fcd06-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="fcd06-103">如果 SharePoint 群組的成員資格] 未設為任何人使用 「 拒絕存取 」 錯誤訊息嘗試將電子郵件傳送至 SharePoint 群組的 SharePoint 2013 工作流程可能會失敗。</span><span class="sxs-lookup"><span data-stu-id="fcd06-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="fcd06-104">**若要解決此問題，請執行下列步驟：**</span><span class="sxs-lookup"><span data-stu-id="fcd06-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="fcd06-105">可讓所有人都可以看到的 SharePoint 群組的成員。</span><span class="sxs-lookup"><span data-stu-id="fcd06-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="fcd06-106">SharePoint 群組移除 [收件者] 或 [副本] 行的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="fcd06-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="fcd06-107">明確地將使用者新增至 [收件者] 或 [副本] 行如果成員資格不能變更可見度 SharePoint 群組。</span><span class="sxs-lookup"><span data-stu-id="fcd06-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="fcd06-108">若要檢視的詳細資訊請參考[HTTP 未經授權至 /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="fcd06-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

