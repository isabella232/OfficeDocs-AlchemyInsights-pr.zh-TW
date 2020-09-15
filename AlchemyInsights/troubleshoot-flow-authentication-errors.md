---
title: 疑難排解流程驗證錯誤
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3c4ad806ed446803d8c1e0ba17b3a06d591985d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690558"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="1b9be-102">疑難排解流程驗證錯誤</span><span class="sxs-lookup"><span data-stu-id="1b9be-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="1b9be-103">在許多情況下，資料流程會因為驗證錯誤而失敗。</span><span class="sxs-lookup"><span data-stu-id="1b9be-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="1b9be-104">如果您有這種錯誤類型，錯誤訊息會包含「未授權」，或是錯誤代碼401或403出現。</span><span class="sxs-lookup"><span data-stu-id="1b9be-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="1b9be-105">您通常可以透過更新 connection 修正驗證錯誤：</span><span class="sxs-lookup"><span data-stu-id="1b9be-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="1b9be-106">在 [網頁入口網站] 的頂端，按一下或點擊齒輪圖示以開啟 [設定] 功能表，然後按一下或點擊 [ **連接**]。</span><span class="sxs-lookup"><span data-stu-id="1b9be-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="1b9be-107">向您看到未授權錯誤訊息的連線。</span><span class="sxs-lookup"><span data-stu-id="1b9be-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="1b9be-108">在連線旁，按一下或點擊 [ **驗證密碼** ] 連結（有關未驗證的連線訊息）。</span><span class="sxs-lookup"><span data-stu-id="1b9be-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="1b9be-109">遵循顯示的指示來驗證您的認證，並回到您的流程執行失敗，然後按一下或點擊 [ **重新提交**]。</span><span class="sxs-lookup"><span data-stu-id="1b9be-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="1b9be-110">如需詳細資訊，請參閱 [疑難排解流程](https://go.microsoft.com/fwlink/?linkid=872110)。</span><span class="sxs-lookup"><span data-stu-id="1b9be-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

