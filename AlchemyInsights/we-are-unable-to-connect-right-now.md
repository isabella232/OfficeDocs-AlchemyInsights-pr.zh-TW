---
title: 啟用此問題:-我們目前無法連線現在
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628233"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="e3e44-102">修正 Office 應用程式 」 我們目前無法連線現在的 「 郵件</span><span class="sxs-lookup"><span data-stu-id="e3e44-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="e3e44-103">如果您收到這封郵件，請嘗試下列作法：</span><span class="sxs-lookup"><span data-stu-id="e3e44-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e3e44-104">檢查您的防火牆、 防毒軟體，與 proxy 設定，以確認，它們都不會封鎖 Office 相關應用程式的網際網路存取。</span><span class="sxs-lookup"><span data-stu-id="e3e44-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="e3e44-105">請參閱[Office 365 Url 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="e3e44-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="e3e44-106">移至**開始** > **執行**，然後再類型**services.msc**。</span><span class="sxs-lookup"><span data-stu-id="e3e44-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="e3e44-107">請確認下列服務所有執行中：</span><span class="sxs-lookup"><span data-stu-id="e3e44-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="e3e44-108">網路連線的裝置自動設定</span><span class="sxs-lookup"><span data-stu-id="e3e44-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="e3e44-109">網路清單服務</span><span class="sxs-lookup"><span data-stu-id="e3e44-109">Network List Service</span></span>
    - <span data-ttu-id="e3e44-110">網路位置認知</span><span class="sxs-lookup"><span data-stu-id="e3e44-110">Network Location Awareness</span></span>
    - <span data-ttu-id="e3e44-111">Windows 事件記錄檔</span><span class="sxs-lookup"><span data-stu-id="e3e44-111">Windows Event Log</span></span>

<span data-ttu-id="e3e44-112">如果其中一個服務未執行，嘗試啟動它。</span><span class="sxs-lookup"><span data-stu-id="e3e44-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="e3e44-113">如果您有問題，啟動服務，以提高權限的權限開啟命令提示字元中執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="e3e44-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="e3e44-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="e3e44-114">**sfc /scannow**</span></span>

<span data-ttu-id="e3e44-115">此命令完成之後，重新啟動電腦。</span><span class="sxs-lookup"><span data-stu-id="e3e44-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="e3e44-116">如需詳細資訊，請參閱[「 很抱歉，我們無法連線至您的帳戶。請稍後再試 」 錯誤，當您啟動從 Office 365 的 Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。</span><span class="sxs-lookup"><span data-stu-id="e3e44-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>