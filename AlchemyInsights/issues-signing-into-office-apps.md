---
title: 登入 Microsoft 365 應用程式時的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695170"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="e4be2-102">修正 Microsoft 365 應用程式「您電腦的信任的平臺模組無法正常運作」訊息</span><span class="sxs-lookup"><span data-stu-id="e4be2-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="e4be2-103">若要修正此錯誤，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="e4be2-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="e4be2-104">安裝最新的 [Windows](https://support.microsoft.com/help/4027667/windows-10-update) 和 [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)更新。</span><span class="sxs-lookup"><span data-stu-id="e4be2-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="e4be2-105">使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="e4be2-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e4be2-106">**附注：** Office 2016 的登錄路徑已變更為16.0。</span><span class="sxs-lookup"><span data-stu-id="e4be2-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e4be2-107"> (Ex： \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e4be2-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="e4be2-108">嘗試 [使用者](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) 復原程式以修正受信任的平臺模組 (TPM) 失敗。</span><span class="sxs-lookup"><span data-stu-id="e4be2-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="e4be2-109">使用下列步驟設定 EnableADAL = 0：</span><span class="sxs-lookup"><span data-stu-id="e4be2-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="e4be2-110">以滑鼠右鍵按一下 [Windows 開始] 按鈕，選擇 [ **執行**]，輸入 **regedit**，然後選擇 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="e4be2-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="e4be2-111">選取 **[是]** 以允許登錄編輯程式對您的裝置進行變更。</span><span class="sxs-lookup"><span data-stu-id="e4be2-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="e4be2-112">在登錄編輯程式中，在 HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity. 下新增 **EnableADAL** ，其設定為 **0** 的 DWORD 值。</span><span class="sxs-lookup"><span data-stu-id="e4be2-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="e4be2-113">如需詳細資訊，請參閱在 [Windows 10 上更新到 Office 2016 build 16.0.7967 後，登入的連線問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。</span><span class="sxs-lookup"><span data-stu-id="e4be2-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>