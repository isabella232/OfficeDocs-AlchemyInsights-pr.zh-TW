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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581866"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="4dfa4-102">修正 Microsoft 365 應用程式「無法立即連線」訊息</span><span class="sxs-lookup"><span data-stu-id="4dfa4-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="4dfa4-103">如果您收到這封郵件，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="4dfa4-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="4dfa4-104">檢查您的防火牆、防毒軟體及 proxy 設定，以確認他們不會封鎖對 Microsoft 365 應用程式的網際網路存取。</span><span class="sxs-lookup"><span data-stu-id="4dfa4-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="4dfa4-105">請參閱[Microsoft URLs 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="4dfa4-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="4dfa4-106">移至 [**開始**  >  **執行**]，然後輸入**services.msc**。</span><span class="sxs-lookup"><span data-stu-id="4dfa4-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="4dfa4-107">請確定下列服務都在執行中：</span><span class="sxs-lookup"><span data-stu-id="4dfa4-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="4dfa4-108">網路連線裝置自動設定</span><span class="sxs-lookup"><span data-stu-id="4dfa4-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="4dfa4-109">網路清單服務</span><span class="sxs-lookup"><span data-stu-id="4dfa4-109">Network List Service</span></span>
    - <span data-ttu-id="4dfa4-110">網路位置知曉</span><span class="sxs-lookup"><span data-stu-id="4dfa4-110">Network Location Awareness</span></span>
    - <span data-ttu-id="4dfa4-111">Windows 事件記錄檔</span><span class="sxs-lookup"><span data-stu-id="4dfa4-111">Windows Event Log</span></span>

<span data-ttu-id="4dfa4-112">如果其中一項服務未執行，請嘗試啟動它。</span><span class="sxs-lookup"><span data-stu-id="4dfa4-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="4dfa4-113">如果您在啟動服務時發生問題，請以較高的權限開啟命令提示字元，以執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="4dfa4-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="4dfa4-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="4dfa4-114">**sfc /scannow**</span></span>

<span data-ttu-id="4dfa4-115">完成此命令後，請重新開機電腦。</span><span class="sxs-lookup"><span data-stu-id="4dfa4-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="4dfa4-116">如需詳細資訊，請參閱["對不起，我們無法連線到您的帳戶。當您從 Microsoft 365 啟動 Office 時，請稍後再試一次](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。</span><span class="sxs-lookup"><span data-stu-id="4dfa4-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>