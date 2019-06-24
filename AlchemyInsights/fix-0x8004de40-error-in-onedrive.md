---
title: 修正 OneDrive 中的0x8004de40 錯誤
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133968"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="19d90-102">修正 OneDrive 中的0x8004de40 錯誤</span><span class="sxs-lookup"><span data-stu-id="19d90-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="19d90-103">如果您收到 OneDrive 的0x8004de40 錯誤:</span><span class="sxs-lookup"><span data-stu-id="19d90-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="19d90-104">在連線至您的 Acitve Directory 網域時, 重新開機受影響的電腦。</span><span class="sxs-lookup"><span data-stu-id="19d90-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="19d90-105">如果重新開機無法修正問題, 請將裝置從 Azure AD 脫離並重新加入。</span><span class="sxs-lookup"><span data-stu-id="19d90-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="19d90-106">**附注**: 執行這些步驟時, 您應該在公司網路上。</span><span class="sxs-lookup"><span data-stu-id="19d90-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="19d90-107">當您無法連線到公司基礎結構 (例如出差時) 時, 請勿執行這些步驟。</span><span class="sxs-lookup"><span data-stu-id="19d90-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="19d90-108">開啟提升許可權的命令提示字元。</span><span class="sxs-lookup"><span data-stu-id="19d90-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="19d90-109">若要開啟提升許可權的命令提示字元, 請按一下 [**開始**], 用滑鼠右鍵按一下 [**命令提示**字元], 然後按一下 [以**管理員身分執行**]。</span><span class="sxs-lookup"><span data-stu-id="19d90-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="19d90-110">輸入*dsregcmd/leave* , 然後按**enter**鍵。</span><span class="sxs-lookup"><span data-stu-id="19d90-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="19d90-111">完成時, 請輸入*dsregcmd/join* , 然後按**enter**。</span><span class="sxs-lookup"><span data-stu-id="19d90-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="19d90-112">完成後, 請關閉命令提示字元。</span><span class="sxs-lookup"><span data-stu-id="19d90-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="19d90-113">重新開機電腦, 然後登入 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="19d90-113">Reboot the computer, and log into OneDrive.</span></span>