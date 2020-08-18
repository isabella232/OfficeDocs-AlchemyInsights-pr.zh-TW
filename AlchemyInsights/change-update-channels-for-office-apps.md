---
title: 變更 Office 應用程式的更新通道
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 43a3cdefe5a9bc1726984a3195dce7aaea08d892
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786844"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="1b672-102">變更 Office 應用程式的更新通道</span><span class="sxs-lookup"><span data-stu-id="1b672-102">Change update channels for Office apps</span></span>

<span data-ttu-id="1b672-103">對於新的 Office 安裝，請使用 Office 軟體下載設定選取所需的更新頻道，然後安裝 (或重新安裝) Office 應用程式。  </span><span class="sxs-lookup"><span data-stu-id="1b672-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="1b672-104">如需詳細資訊， 請參閱 [管理 Office 365 中的軟體下載設定](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365)。</span><span class="sxs-lookup"><span data-stu-id="1b672-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="1b672-105">**附註** 使用 Office 軟體下載設定選取的更新通道適用于使用 O365 入口網站執行新安裝的所有使用者。</span><span class="sxs-lookup"><span data-stu-id="1b672-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="1b672-106">如需更多資訊，請參閱 [在 PC 或 Mac 上下載並安裝或重新安裝 Microsoft 365 或 Office 2019](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)。</span><span class="sxs-lookup"><span data-stu-id="1b672-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="1b672-107">對於現有的 Office 安裝，請使用 Office 部署工具 (ODT) 切換到其他更新通道：</span><span class="sxs-lookup"><span data-stu-id="1b672-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="1b672-108">從 [Microsoft 下載中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下載最新版的 Office 部署工具 (setup.exe)。</span><span class="sxs-lookup"><span data-stu-id="1b672-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="1b672-109">識別要切換到的通道名稱。</span><span class="sxs-lookup"><span data-stu-id="1b672-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="1b672-110">如需詳細資訊，請參閱 [Office 部署工具的設定選項](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)。</span><span class="sxs-lookup"><span data-stu-id="1b672-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="1b672-111">建立指定適當的通道名稱的組態 XML 檔案，例如 update.xml。</span><span class="sxs-lookup"><span data-stu-id="1b672-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  

`<Configuration>`<br>
`<Updates Channel="Current"/>`<br>
`</Configuration>`<br>

4. <span data-ttu-id="1b672-112">在已提升權限的命令提示字元下，切換至 setup.exe 所在的資料夾，接著執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="1b672-112">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="1b672-113">a.</span><span class="sxs-lookup"><span data-stu-id="1b672-113">a.</span></span> <span data-ttu-id="1b672-114">setup.exe /configure update.xml</span><span class="sxs-lookup"><span data-stu-id="1b672-114">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="1b672-115">啟動 Office 應用程式 (例如 Excel)，然後選取 **[檔案]** > **帳戶**。</span><span class="sxs-lookup"><span data-stu-id="1b672-115">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="1b672-116">在 [產品資訊] 區段，選取 **[更新選項]** > \*\* [立即更新]\*\*。</span><span class="sxs-lookup"><span data-stu-id="1b672-116">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="1b672-117">如需更多資訊，請參閱 [如何切換現有 Office 應用程式的更新頻道](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel)。</span><span class="sxs-lookup"><span data-stu-id="1b672-117">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="1b672-118">要切換選定使用者群組的更新通道或使用組態管理員 (SCCM)，請使用 GPO 設定更新通道設定。</span><span class="sxs-lookup"><span data-stu-id="1b672-118">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="1b672-119">如需詳細資訊，請參閱 [Microsoft 365 Apps 更新通道的概觀](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy)。</span><span class="sxs-lookup"><span data-stu-id="1b672-119">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="1b672-120">如需詳細資訊，請參閱 [如何管理 Office 365 專業增強版 (IT 專業人員)](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) 和 [使用 Microsoft Endpoint Configuration Manager 管理 Microsoft 365 Apps 的更新](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)。</span><span class="sxs-lookup"><span data-stu-id="1b672-120">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>