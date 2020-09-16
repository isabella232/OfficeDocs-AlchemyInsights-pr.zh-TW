---
title: 控制 Office 應用程式自動更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747767"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="a1b57-102">控制 Office 應用程式自動更新</span><span class="sxs-lookup"><span data-stu-id="a1b57-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="a1b57-103">根據預設，從網際網路自動下載並在背景中套用 Office 應用程式的更新，不需要任何使用者介入。</span><span class="sxs-lookup"><span data-stu-id="a1b57-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="a1b57-104">不過，系統管理員可以使用 Office [更新] 設定來控制應用更新的方式。</span><span class="sxs-lookup"><span data-stu-id="a1b57-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="a1b57-105">[更新] 設定允許系統管理員啟用或停用自動更新、顯示或隱藏 Office 中的 **[立即更新]** 按鈕、設定更新期限等。</span><span class="sxs-lookup"><span data-stu-id="a1b57-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="a1b57-106">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="a1b57-106">For detailed information, see:</span></span>

- [<span data-ttu-id="a1b57-107">設定 Office 更新設定</span><span class="sxs-lookup"><span data-stu-id="a1b57-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="a1b57-108">未啟用 Office 自動更新</span><span class="sxs-lookup"><span data-stu-id="a1b57-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="a1b57-109">定義安裝 Office 之後如何更新</span><span class="sxs-lookup"><span data-stu-id="a1b57-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="a1b57-110">若要查看套用至用戶端電腦的現有更新設定，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="a1b57-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="a1b57-111">若要開啟 [登錄編輯程式]，請移至 **[開始]** > **[執行]** > **regedit**。</span><span class="sxs-lookup"><span data-stu-id="a1b57-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="a1b57-112">切換到下列位置，並查看 Office [更新] 設定：</span><span class="sxs-lookup"><span data-stu-id="a1b57-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="a1b57-113">a.</span><span class="sxs-lookup"><span data-stu-id="a1b57-113">a.</span></span> <span data-ttu-id="a1b57-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="a1b57-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="a1b57-115">b.</span><span class="sxs-lookup"><span data-stu-id="a1b57-115">b.</span></span> <span data-ttu-id="a1b57-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="a1b57-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="a1b57-117">**附註** 如果已設定 OfficeMgmtCOM 機碼，可能會在 **Office** > **帳戶** > \*\* Office 更新\*\*中看到「由系統管理員管理更新」的訊息。</span><span class="sxs-lookup"><span data-stu-id="a1b57-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="a1b57-118">如需更多資訊，請參閱[使用 Microsoft Endpoint Configuration Manager 管理 Microsoft 365 Apps 的更新](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)。</span><span class="sxs-lookup"><span data-stu-id="a1b57-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  