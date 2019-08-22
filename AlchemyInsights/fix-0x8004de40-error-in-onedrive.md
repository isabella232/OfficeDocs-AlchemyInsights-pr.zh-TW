---
title: 修正 OneDrive 中的 0x8004de40 錯誤
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525050"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="2a42b-102">修正 OneDrive 中的 0x8004de40 錯誤</span><span class="sxs-lookup"><span data-stu-id="2a42b-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="2a42b-103">如果您收到 OneDrive 0x8004de40 錯誤：</span><span class="sxs-lookup"><span data-stu-id="2a42b-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="2a42b-104">重新啟動受影響的電腦連線到您啟用目錄的網域時。</span><span class="sxs-lookup"><span data-stu-id="2a42b-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="2a42b-105">如果重新開啟才不會修正這個問題，解除加入並重新加入您的裝置從 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="2a42b-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="2a42b-106">**附註**： 您應在公司網路上同時執行這些步驟。</span><span class="sxs-lookup"><span data-stu-id="2a42b-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="2a42b-107">當您不可以連線到您公司的基礎結構 （例如，當旅行） 時，不執行這些步驟。</span><span class="sxs-lookup"><span data-stu-id="2a42b-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="2a42b-108">開啟提升權限的命令提示字元。</span><span class="sxs-lookup"><span data-stu-id="2a42b-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="2a42b-109">若要開啟提升權限的命令提示字元處，按一下 [-**開始**，以滑鼠右鍵按一下 [**命令提示字元處**，，然後按一下 [**以管理員身分執行**。</span><span class="sxs-lookup"><span data-stu-id="2a42b-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="2a42b-110">輸入*dsregcmd /leave* ，然後按**Enter**鍵。</span><span class="sxs-lookup"><span data-stu-id="2a42b-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="2a42b-111">完成後，輸入*dsregcmd /join* ，然後按**Enter**鍵。</span><span class="sxs-lookup"><span data-stu-id="2a42b-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="2a42b-112">完成時，關閉命令提示字元。</span><span class="sxs-lookup"><span data-stu-id="2a42b-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="2a42b-113">將電腦重新開機並登入 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="2a42b-113">Reboot the computer, and log into OneDrive.</span></span>