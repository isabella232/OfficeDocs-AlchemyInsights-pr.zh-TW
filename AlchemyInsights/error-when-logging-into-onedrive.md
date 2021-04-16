---
title: 啟動 OneDrive 時發生0x8004de40 錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813643"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="b6cb7-102">啟動 OneDrive 時發生0x8004de40 錯誤</span><span class="sxs-lookup"><span data-stu-id="b6cb7-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="b6cb7-103">如果您在登入 OneDrive 時收到錯誤 **0x8004de40** ，請在連線至您的公司或學校網域時，重新開機電腦。</span><span class="sxs-lookup"><span data-stu-id="b6cb7-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="b6cb7-104">如果重新開機後收到此錯誤，請在連線至您的工作或學校網域時，嘗試此動作：</span><span class="sxs-lookup"><span data-stu-id="b6cb7-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="b6cb7-105">按一下 [開始]，  **然後在搜尋方塊中，** 于命令提示字元應用程式上按一下滑鼠右鍵，然後選取 [**以系統管理員身分執行**]。</span><span class="sxs-lookup"><span data-stu-id="b6cb7-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="b6cb7-106">如果系統提示您輸入系統管理員密碼或進行確認，請輸入密碼或按一下 [ **允許**]。</span><span class="sxs-lookup"><span data-stu-id="b6cb7-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="b6cb7-107">在 [命令提示字元] 視窗中，輸入 **dsregcmd/leave**  ，並等待命令完成。</span><span class="sxs-lookup"><span data-stu-id="b6cb7-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="b6cb7-108">然後輸入 **dsregcmd/join** ，並等待命令完成。</span><span class="sxs-lookup"><span data-stu-id="b6cb7-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="b6cb7-109">重新開機電腦。</span><span class="sxs-lookup"><span data-stu-id="b6cb7-109">Reboot your computer.</span></span>
