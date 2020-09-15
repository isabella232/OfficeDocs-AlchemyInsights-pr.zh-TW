---
title: 變更公用資料夾許可權
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714238"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="bcbbf-102">變更公用資料夾許可權</span><span class="sxs-lookup"><span data-stu-id="bcbbf-102">Changing public folder permissions</span></span>

<span data-ttu-id="bcbbf-103">使用者和 Outlook 中的系統管理員可以變更公用資料夾許可權。</span><span class="sxs-lookup"><span data-stu-id="bcbbf-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="bcbbf-104">管理員也可以執行下列動作，以控制從 Exchange 系統管理中心 (EAC) 的許可權：</span><span class="sxs-lookup"><span data-stu-id="bcbbf-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="bcbbf-105">在 Microsoft 365 系統管理中心中，移至 [系統 **管理中心**] [ \> **Exchange**]。</span><span class="sxs-lookup"><span data-stu-id="bcbbf-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="bcbbf-106">選取 [ **公用資料夾**]。</span><span class="sxs-lookup"><span data-stu-id="bcbbf-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="bcbbf-107">您可以從那裡將安全性群組指派給許可權，以變更個別公用資料夾的許可權。</span><span class="sxs-lookup"><span data-stu-id="bcbbf-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="bcbbf-108">若要讓使用者變更公用資料夾許可權，使用者必須擁有該資料夾的擁有者許可權。</span><span class="sxs-lookup"><span data-stu-id="bcbbf-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="bcbbf-109">請依照 [如何診斷並修正公用資料夾許可權問題的程式](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) 所述，以疑難排解公用資料夾的許可權問題。</span><span class="sxs-lookup"><span data-stu-id="bcbbf-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="bcbbf-110">**附注**：當您嘗試變更公用資料夾的許可權時，可能會遇到一些已知的問題。</span><span class="sxs-lookup"><span data-stu-id="bcbbf-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="bcbbf-111">如需詳細資訊，請參閱下列文章。</span><span class="sxs-lookup"><span data-stu-id="bcbbf-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="bcbbf-112">無法將許可權套用至 EAC 中的公用資料夾子資料夾</span><span class="sxs-lookup"><span data-stu-id="bcbbf-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- <span data-ttu-id="bcbbf-113">[當您存取公用資料夾時，未在 [本機樹系中找到信箱] 錯誤](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)</span><span class="sxs-lookup"><span data-stu-id="bcbbf-113">["The mailbox is not found in the local forest" error when you access public folders](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)</span></span>
