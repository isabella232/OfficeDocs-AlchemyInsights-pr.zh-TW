---
title: 啟用問題-現在無法連線
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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716163"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="fb462-102">修正 Office 應用程式「無法立即連接」訊息</span><span class="sxs-lookup"><span data-stu-id="fb462-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="fb462-103">如果您收到這封郵件，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="fb462-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="fb462-104">檢查您的防火牆、防毒軟體及 proxy 設定，以確認他們不會封鎖 Office 應用程式的網際網路存取。</span><span class="sxs-lookup"><span data-stu-id="fb462-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="fb462-105">請參閱[Microsoft URLs 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="fb462-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="fb462-106">移至 [**開始** > **執行**]，然後輸入**services.msc**。</span><span class="sxs-lookup"><span data-stu-id="fb462-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="fb462-107">請確定下列服務都在執行中：</span><span class="sxs-lookup"><span data-stu-id="fb462-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="fb462-108">網路連線裝置自動設定</span><span class="sxs-lookup"><span data-stu-id="fb462-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="fb462-109">網路清單服務</span><span class="sxs-lookup"><span data-stu-id="fb462-109">Network List Service</span></span>
    - <span data-ttu-id="fb462-110">網路位置知曉</span><span class="sxs-lookup"><span data-stu-id="fb462-110">Network Location Awareness</span></span>
    - <span data-ttu-id="fb462-111">Windows 事件記錄檔</span><span class="sxs-lookup"><span data-stu-id="fb462-111">Windows Event Log</span></span>

<span data-ttu-id="fb462-112">如果其中一項服務未執行，請嘗試啟動它。</span><span class="sxs-lookup"><span data-stu-id="fb462-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="fb462-113">如果您在啟動服務時發生問題，請以較高的權限開啟命令提示字元，以執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="fb462-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="fb462-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="fb462-114">**sfc /scannow**</span></span>

<span data-ttu-id="fb462-115">完成此命令後，請重新開機電腦。</span><span class="sxs-lookup"><span data-stu-id="fb462-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="fb462-116">如需詳細資訊，請參閱["對不起，我們無法連線到您的帳戶。當您從 Microsoft 365 啟動 Office 時，請稍後再試一次](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。</span><span class="sxs-lookup"><span data-stu-id="fb462-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>