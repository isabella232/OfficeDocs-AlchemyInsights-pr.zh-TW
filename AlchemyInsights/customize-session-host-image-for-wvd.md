---
title: 自訂 Windows 虛擬桌面的工作階段主機影像
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003902"
- "6957"
ms.openlocfilehash: 23bf130aad5bafa6756f0adfc2e58a130c2f6c4e
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681464"
---
# <a name="customize-a-session-host-image-for-windows-virtual-desktop"></a><span data-ttu-id="243ac-102">自訂 Windows 虛擬桌面的工作階段主機影像</span><span class="sxs-lookup"><span data-stu-id="243ac-102">Customize a session host image for Windows Virtual Desktop</span></span>

<span data-ttu-id="243ac-103">使用 Windows 虛擬桌面的主虛擬硬碟映射來準備虛擬機器 (VM) 有兩種方式：</span><span class="sxs-lookup"><span data-stu-id="243ac-103">There are two ways to prepare a virtual machine (VM) by using a master Virtual Hard Disk image for Windows Virtual Desktop:</span></span>

1. <span data-ttu-id="243ac-104">[從 Azure 中的受管理映射建立 VM](https://go.microsoft.com/fwlink/?linkid=2127906)，然後略過 [軟體的準備和安裝](https://go.microsoft.com/fwlink/?linkid=2128064)。</span><span class="sxs-lookup"><span data-stu-id="243ac-104">[Create a VM from a managed image in Azure](https://go.microsoft.com/fwlink/?linkid=2127906), and then skip ahead to the [preparation and installation of software](https://go.microsoft.com/fwlink/?linkid=2128064).</span></span>
1. <span data-ttu-id="243ac-105">下載影像、布建[HYPER-V VM](https://go.microsoft.com/fwlink/?linkid=2127907)，然後自訂以符合您的需求，以在[本機建立圖像](https://go.microsoft.com/fwlink/?linkid=2128065)。</span><span class="sxs-lookup"><span data-stu-id="243ac-105">[Create the image locally](https://go.microsoft.com/fwlink/?linkid=2128065) by downloading the image, [provisioning a Hyper-V VM](https://go.microsoft.com/fwlink/?linkid=2127907), and then customizing it to suit your needs.</span></span>

<span data-ttu-id="243ac-106">若要深入瞭解，請參閱 [準備和自訂主 VHD 映射](https://go.microsoft.com/fwlink/?linkid=2127838)。</span><span class="sxs-lookup"><span data-stu-id="243ac-106">To learn more, see [Prepare and customize a master VHD image](https://go.microsoft.com/fwlink/?linkid=2127838).</span></span>