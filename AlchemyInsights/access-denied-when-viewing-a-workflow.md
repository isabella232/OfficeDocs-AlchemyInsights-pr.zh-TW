---
title: 檢視工作流程時，拒絕存取
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747739"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="f0eb6-102">檢視工作流程時，拒絕存取</span><span class="sxs-lookup"><span data-stu-id="f0eb6-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="f0eb6-103">如果 SharePoint 群組的成員資格不設為所有人，嘗試將電子郵件傳送至 SharePoint 群組的 SharePoint 2013 工作流程可能會失敗與 「 存取被拒 」 錯誤訊息。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="f0eb6-104">**若要解決此問題，請執行下列步驟：**</span><span class="sxs-lookup"><span data-stu-id="f0eb6-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="f0eb6-105">允許所有人都可以查看 SharePoint 群組的成員。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="f0eb6-106">SharePoint 群組移除 [收件者] 或 [副本] 行的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="f0eb6-107">明確地將使用者新增至 [收件者] 或 [副本] 行如果無法變更 SharePoint 群組成員資格可見性。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="f0eb6-108">若要檢視的詳細資訊請參閱[HTTP 未經授權至 /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  