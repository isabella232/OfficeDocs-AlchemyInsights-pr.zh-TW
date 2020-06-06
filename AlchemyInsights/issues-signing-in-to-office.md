---
title: 登入 Microsoft 365 應用程式時的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579892"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="276fe-102">Microsoft 365 應用程式中的空白登入畫面</span><span class="sxs-lookup"><span data-stu-id="276fe-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="276fe-103">若要修正此問題，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="276fe-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="276fe-104">安裝最新的[Windows](https://support.microsoft.com/help/4027667/windows-10-update)和[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)更新。</span><span class="sxs-lookup"><span data-stu-id="276fe-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="276fe-105">重設 internet Explorer 選項：移至**工具**  >  **網際網路選項**  >  **Advanced**  >  **Reset internet Explorer 設定**（請注意，您會失去自訂設定），然後再次嘗試登入 Office。</span><span class="sxs-lookup"><span data-stu-id="276fe-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="276fe-106">停用 Windows Defender 應用程式防護（WDAG）或任何類似的防火牆或防毒程式：</span><span class="sxs-lookup"><span data-stu-id="276fe-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="276fe-107">在 [控制台] 中，移至 [**程式**]，然後選擇 [**開啟或關閉 Windows 功能**]。</span><span class="sxs-lookup"><span data-stu-id="276fe-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="276fe-108">如果已啟用 Windows Defender Application Guard，請嘗試停用它。</span><span class="sxs-lookup"><span data-stu-id="276fe-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="276fe-109">**附注：** 您可能需要重新開機電腦。</span><span class="sxs-lookup"><span data-stu-id="276fe-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="276fe-110">確定任何應用程式或防火牆/反病毒程式都未封鎖 BrokerPlugin [AAD WAM 外掛程式](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)。</span><span class="sxs-lookup"><span data-stu-id="276fe-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="276fe-111">使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="276fe-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="276fe-112">**附注：** Office 2016 的登錄路徑已變更為16.0。</span><span class="sxs-lookup"><span data-stu-id="276fe-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="276fe-113">（Ex： \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="276fe-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="276fe-114">如需詳細資訊，請參閱在[Windows 10 上更新到 Office 2016 build 16.0.7967 後，登入的連線問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。</span><span class="sxs-lookup"><span data-stu-id="276fe-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>