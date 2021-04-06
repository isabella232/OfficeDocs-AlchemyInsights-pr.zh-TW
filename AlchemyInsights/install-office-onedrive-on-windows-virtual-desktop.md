---
title: 在 Windows 虛擬桌面上安裝 Office 和 OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590274"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="2c212-102">在 Windows 虛擬桌面上安裝 Office 和 OneDrive</span><span class="sxs-lookup"><span data-stu-id="2c212-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="2c212-103">[準備並自訂主 VHD 映像](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)。</span><span class="sxs-lookup"><span data-stu-id="2c212-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="2c212-104">如果尚未建立虛擬機器 (VM)，請建立它。</span><span class="sxs-lookup"><span data-stu-id="2c212-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="2c212-105">[在用電腦啟用模式中安裝 Office](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)。</span><span class="sxs-lookup"><span data-stu-id="2c212-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="2c212-106">共用電腦啟用可讓多個使用者存取 Office。</span><span class="sxs-lookup"><span data-stu-id="2c212-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="2c212-107">[在每一電腦模式下安裝 OneDrive](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)。</span><span class="sxs-lookup"><span data-stu-id="2c212-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="2c212-108">通常，OneDrive 是按使用者安裝的，但在這裡，它應該按機器安裝。</span><span class="sxs-lookup"><span data-stu-id="2c212-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>