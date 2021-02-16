---
title: 啟用裝置
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255160"
---
# <a name="enable-device"></a><span data-ttu-id="7ecf2-102">啟用裝置</span><span class="sxs-lookup"><span data-stu-id="7ecf2-102">Enable Device</span></span>

<span data-ttu-id="7ecf2-103">**啟用裝置使用 Powershell 命令**</span><span class="sxs-lookup"><span data-stu-id="7ecf2-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="7ecf2-104">執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="7ecf2-104">Run the following commands:</span></span>

- <span data-ttu-id="7ecf2-105">若要取得 device 物件： `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="7ecf2-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="7ecf2-106">若要啟用裝置： `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="7ecf2-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="7ecf2-107">如需在受管理的網域上設定混合式加入的詳細資訊，請參閱 [設定混合式加入](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)。</span><span class="sxs-lookup"><span data-stu-id="7ecf2-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>
