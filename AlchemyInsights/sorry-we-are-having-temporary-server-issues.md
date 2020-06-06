---
title: 修正 Microsoft 365 app 抱歉，我們有暫時的伺服器問題訊息
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582694"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="2dc4f-102">修正 Microsoft 365 應用程式「對不起，我們有暫時的伺服器問題」訊息</span><span class="sxs-lookup"><span data-stu-id="2dc4f-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="2dc4f-103">如果您收到這封郵件，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="2dc4f-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2dc4f-104">檢查您的防火牆、防毒軟體及 proxy 設定，以確認他們不會封鎖對 Microsoft 365 應用程式的網際網路存取。</span><span class="sxs-lookup"><span data-stu-id="2dc4f-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="2dc4f-105">請參閱[URLs 及 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="2dc4f-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="2dc4f-106">移至 [**開始**  >  **執行**]，然後輸入**services.msc**。</span><span class="sxs-lookup"><span data-stu-id="2dc4f-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="2dc4f-107">請確定下列服務都在執行中：</span><span class="sxs-lookup"><span data-stu-id="2dc4f-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="2dc4f-108">網路連線裝置自動設定</span><span class="sxs-lookup"><span data-stu-id="2dc4f-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="2dc4f-109">網路清單服務</span><span class="sxs-lookup"><span data-stu-id="2dc4f-109">Network List Service</span></span>
    - <span data-ttu-id="2dc4f-110">網路位置知曉</span><span class="sxs-lookup"><span data-stu-id="2dc4f-110">Network Location Awareness</span></span>
    - <span data-ttu-id="2dc4f-111">Windows 事件記錄檔</span><span class="sxs-lookup"><span data-stu-id="2dc4f-111">Windows Event Log</span></span>

<span data-ttu-id="2dc4f-112">如果其中一項服務未執行，請嘗試啟動它。</span><span class="sxs-lookup"><span data-stu-id="2dc4f-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="2dc4f-113">如果您在啟動服務時發生問題，請以較高的權限開啟命令提示字元，以執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="2dc4f-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="2dc4f-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="2dc4f-114">**sfc /scannow**</span></span>

<span data-ttu-id="2dc4f-115">完成此命令後，請重新開機電腦。</span><span class="sxs-lookup"><span data-stu-id="2dc4f-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="2dc4f-116">如需詳細資訊，請參閱["對不起，我們無法連線到您的帳戶。啟動時，請稍後再試一次] 錯誤](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。</span><span class="sxs-lookup"><span data-stu-id="2dc4f-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>