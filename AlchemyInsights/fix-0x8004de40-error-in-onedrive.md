---
title: 修正 OneDrive 中的0x8004de40 錯誤
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649739"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="2cbf3-102">修正 OneDrive 中的0x8004de40 錯誤</span><span class="sxs-lookup"><span data-stu-id="2cbf3-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="2cbf3-103">如果您是執行 Windows 7，但收到此錯誤，請 [更新以啟用 tls 1.1 和 tls 1.2 做為 Windows WinHTTP 中的預設安全通訊協定](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)。</span><span class="sxs-lookup"><span data-stu-id="2cbf3-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="2cbf3-104">如果您正在執行 Windows 10，而且 OneDrive 收到0x8004de40 錯誤：</span><span class="sxs-lookup"><span data-stu-id="2cbf3-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="2cbf3-105">在連線至您的 Acitve 目錄網域時，重新開機受影響的電腦。</span><span class="sxs-lookup"><span data-stu-id="2cbf3-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="2cbf3-106">如果重新開機未修正問題，請從 Azure AD 中脫離裝置並重新加入裝置。</span><span class="sxs-lookup"><span data-stu-id="2cbf3-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="2cbf3-107">**附注**：您應該在公司網路上執行這些步驟。</span><span class="sxs-lookup"><span data-stu-id="2cbf3-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="2cbf3-108">當您未連線到公司基礎結構時，請勿執行這些步驟，例如，旅行) 時 (。</span><span class="sxs-lookup"><span data-stu-id="2cbf3-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="2cbf3-109">選取 [ **開始**]，用滑鼠右鍵按一下 [ **命令提示** 字元]，然後選取 [ **以系統管理員身分執行**]，開啟提升許可權的命令提示字元</span><span class="sxs-lookup"><span data-stu-id="2cbf3-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="2cbf3-110">輸入 *dsregcmd/leave* ，然後按 **enter** 鍵。</span><span class="sxs-lookup"><span data-stu-id="2cbf3-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="2cbf3-111">完成時，請輸入 *dsregcmd/join* ，然後按 **enter**。</span><span class="sxs-lookup"><span data-stu-id="2cbf3-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="2cbf3-112">完成後，請關閉命令提示字元。</span><span class="sxs-lookup"><span data-stu-id="2cbf3-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="2cbf3-113">重新開機電腦，並登入 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="2cbf3-113">Reboot the computer, and log into OneDrive.</span></span>