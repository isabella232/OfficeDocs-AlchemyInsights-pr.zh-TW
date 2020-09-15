---
title: 在查看工作流程時存取遭到拒絕
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688793"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="2e401-102">在查看工作流程時存取遭到拒絕</span><span class="sxs-lookup"><span data-stu-id="2e401-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="2e401-103">如果 SharePoint 群組的成員資格未設定為 [所有人]，則 SharePoint 2013 嘗試將電子郵件傳送至 SharePoint 群組的工作流程會失敗，並顯示「拒絕存取」錯誤訊息。</span><span class="sxs-lookup"><span data-stu-id="2e401-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="2e401-104">**若要解決此問題，請執行下列步驟：**</span><span class="sxs-lookup"><span data-stu-id="2e401-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="2e401-105">允許所有人查看 SharePoint 群組的成員。</span><span class="sxs-lookup"><span data-stu-id="2e401-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="2e401-106">從電子郵件的 [收件者] 或 [抄送] 行中移除 SharePoint 群組。</span><span class="sxs-lookup"><span data-stu-id="2e401-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="2e401-107">如果無法變更 SharePoint 群組的成員資格可見度，請明確將使用者新增至 [收件者] 或 [副本] 行。</span><span class="sxs-lookup"><span data-stu-id="2e401-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="2e401-108">若要查看更多詳細資料 [，請參閱 HTTP 未經授權的/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="2e401-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  