---
title: 不使用密碼登入 Windows 10
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719944"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="9a5af-102">不使用密碼登入 Windows 10</span><span class="sxs-lookup"><span data-stu-id="9a5af-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="9a5af-103">若要避免在 Windows 啟動時輸入密碼，建議您使用其中一個 Windows Hello 安全登入選項，如 PIN、面孔識別或指紋（如果有的話）。</span><span class="sxs-lookup"><span data-stu-id="9a5af-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="9a5af-104">如果您真的想要停用安全登入，請參閱下列的「自動登入 Windows 10」指示。</span><span class="sxs-lookup"><span data-stu-id="9a5af-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="9a5af-105">**保護帳戶密碼的 Windows Hello 備選項**</span><span class="sxs-lookup"><span data-stu-id="9a5af-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="9a5af-106">移至 [ **設定] > 帳戶 > 登入選項** ] (或按一下 [ [這裡](ms-settings:signinoptions?activationSource=GetHelp)) ]。</span><span class="sxs-lookup"><span data-stu-id="9a5af-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="9a5af-107">將會列出可用的登入選項。</span><span class="sxs-lookup"><span data-stu-id="9a5af-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="9a5af-108">例如：</span><span class="sxs-lookup"><span data-stu-id="9a5af-108">For example:</span></span>

![登入選項。](media/sign-in-options.png)

<span data-ttu-id="9a5af-110">按一下或點擊其中一個選項加以設定。</span><span class="sxs-lookup"><span data-stu-id="9a5af-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="9a5af-111">當您下次啟動或解除鎖定 Windows 時，您就可以使用新的選項，而不是密碼。</span><span class="sxs-lookup"><span data-stu-id="9a5af-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="9a5af-112">**自動登入至 Windows 10**</span><span class="sxs-lookup"><span data-stu-id="9a5af-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="9a5af-113">**附注**：自動登入非常方便，但會帶來安全性風險，尤其是當您的電腦可由多人存取時。</span><span class="sxs-lookup"><span data-stu-id="9a5af-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="9a5af-114">按一下或點擊工作列中的 [ **開始** ] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="9a5af-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="9a5af-115">輸入 **netplwiz** ，然後按 Enter 鍵，以開啟 [使用者帳戶] 視窗。</span><span class="sxs-lookup"><span data-stu-id="9a5af-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="9a5af-116">在 [ **使用者帳戶**] 中，按一下 Windows 啟動時要自動登入的帳戶。</span><span class="sxs-lookup"><span data-stu-id="9a5af-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="9a5af-117">取消選取 [使用者必須輸入使用者名稱和密碼才能使用此電腦] 核取方塊。</span><span class="sxs-lookup"><span data-stu-id="9a5af-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![使用者必須輸入 [使用者名稱] 和 [密碼] 選項。](media/users-must-enter-username.png)

5. <span data-ttu-id="9a5af-119">按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="9a5af-119">Click **OK**.</span></span> <span data-ttu-id="9a5af-120">系統會要求您輸入並確認您所選取之帳戶的密碼。</span><span class="sxs-lookup"><span data-stu-id="9a5af-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="9a5af-121">按一下 [確定]\*\*\*\* 完成。</span><span class="sxs-lookup"><span data-stu-id="9a5af-121">Click **OK** to finish.</span></span> <span data-ttu-id="9a5af-122">下次 Windows 10 開始時，它會自動登入您選取的帳戶。</span><span class="sxs-lookup"><span data-stu-id="9a5af-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
