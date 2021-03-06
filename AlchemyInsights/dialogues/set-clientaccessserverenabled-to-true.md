---
title: 將 ClientAccessServerEnabled 設定為 True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509584"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="56e6d-102">將 ClientAccessServerEnabled 設定為 True</span><span class="sxs-lookup"><span data-stu-id="56e6d-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="56e6d-103">如果您無法開啟加密的電子郵件，而是查看 **rpmsg** 附件，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="56e6d-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="56e6d-104">連線至 Exchange Online PowerShell。</span><span class="sxs-lookup"><span data-stu-id="56e6d-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="56e6d-105">若要連線至 Exchange Online PowerShell，您必須使用全域管理員或 Exchange 系統管理員帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="56e6d-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="56e6d-106">a.</span><span class="sxs-lookup"><span data-stu-id="56e6d-106">a.</span></span> <span data-ttu-id="56e6d-107">開啟 [Windows PowerShell]，然後執行下列命令： `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="56e6d-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="56e6d-108">b.</span><span class="sxs-lookup"><span data-stu-id="56e6d-108">b.</span></span> <span data-ttu-id="56e6d-109">在 [ **Windows PowerShell 憑證要求** ] 對話方塊中，輸入您的公司或學校帳戶，以及密碼 c。</span><span class="sxs-lookup"><span data-stu-id="56e6d-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="56e6d-110">按一下 [確定]。</span><span class="sxs-lookup"><span data-stu-id="56e6d-110">Click **OK**.</span></span> 

2. <span data-ttu-id="56e6d-111">執行下列命令以建立新的會話：</span><span class="sxs-lookup"><span data-stu-id="56e6d-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="56e6d-112">a.</span><span class="sxs-lookup"><span data-stu-id="56e6d-112">a.</span></span> <span data-ttu-id="56e6d-113">執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="56e6d-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="56e6d-114">執行 `Get-IRMConfiguration` 命令。</span><span class="sxs-lookup"><span data-stu-id="56e6d-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="56e6d-115">檢查 **ClientAccessServerEnabled** 設定。</span><span class="sxs-lookup"><span data-stu-id="56e6d-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="56e6d-116">a.</span><span class="sxs-lookup"><span data-stu-id="56e6d-116">a.</span></span> <span data-ttu-id="56e6d-117">如果 **ClientAccessServerEnabled** 設定設為 **False**，請執行下列 Cmdlet： `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="56e6d-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="56e6d-118">請務必使用下列命令來關閉 powershell 會話： `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="56e6d-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="56e6d-119">如需詳細資訊，請參閱 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)。</span><span class="sxs-lookup"><span data-stu-id="56e6d-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

