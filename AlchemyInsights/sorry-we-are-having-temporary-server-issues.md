---
title: 修正 Office app 對不起，我們有暫時的伺服器問題訊息
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764108"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="d2a0e-102">修正 Office 應用程式「對不起，我們有暫時的伺服器問題」訊息</span><span class="sxs-lookup"><span data-stu-id="d2a0e-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="d2a0e-103">如果您收到這封郵件，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="d2a0e-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d2a0e-104">檢查您的防火牆、防毒軟體及 proxy 設定，以確認他們不會封鎖 Office 應用程式的網際網路存取。</span><span class="sxs-lookup"><span data-stu-id="d2a0e-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="d2a0e-105">請參閱[URLs 及 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="d2a0e-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="d2a0e-106">移至 [**開始** > **執行**]，然後輸入**services.msc**。</span><span class="sxs-lookup"><span data-stu-id="d2a0e-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="d2a0e-107">請確定下列服務都在執行中：</span><span class="sxs-lookup"><span data-stu-id="d2a0e-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="d2a0e-108">網路連線裝置自動設定</span><span class="sxs-lookup"><span data-stu-id="d2a0e-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="d2a0e-109">網路清單服務</span><span class="sxs-lookup"><span data-stu-id="d2a0e-109">Network List Service</span></span>
    - <span data-ttu-id="d2a0e-110">網路位置知曉</span><span class="sxs-lookup"><span data-stu-id="d2a0e-110">Network Location Awareness</span></span>
    - <span data-ttu-id="d2a0e-111">Windows 事件記錄檔</span><span class="sxs-lookup"><span data-stu-id="d2a0e-111">Windows Event Log</span></span>

<span data-ttu-id="d2a0e-112">如果其中一項服務未執行，請嘗試啟動它。</span><span class="sxs-lookup"><span data-stu-id="d2a0e-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="d2a0e-113">如果您在啟動服務時發生問題，請以較高的權限開啟命令提示字元，以執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="d2a0e-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="d2a0e-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="d2a0e-114">**sfc /scannow**</span></span>

<span data-ttu-id="d2a0e-115">完成此命令後，請重新開機電腦。</span><span class="sxs-lookup"><span data-stu-id="d2a0e-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="d2a0e-116">如需詳細資訊，請參閱["對不起，我們無法連線到您的帳戶。啟動時，請稍後再試一次] 錯誤](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。</span><span class="sxs-lookup"><span data-stu-id="d2a0e-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>