---
title: 移除 Office 的先前 MSI 版本
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
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680606"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="bc43a-102">移除 Office 的先前 MSI 版本</span><span class="sxs-lookup"><span data-stu-id="bc43a-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="bc43a-103">在安裝 Office 365 ProPlus 之前，建議先移除先前 Windows Installer (MSI) 版本的 Office。</span><span class="sxs-lookup"><span data-stu-id="bc43a-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="bc43a-104">以下說明如何執行此動作：</span><span class="sxs-lookup"><span data-stu-id="bc43a-104">Here's how to do this:</span></span>

1. <span data-ttu-id="bc43a-105">如果您使用 MSI 來安裝 Office，您可以使用 Office 部署工具 (ODT) 卸載 Office。</span><span class="sxs-lookup"><span data-stu-id="bc43a-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="bc43a-106">您可以在 **configuration.xml** 檔案中使用 RemoveMSI 元素。</span><span class="sxs-lookup"><span data-stu-id="bc43a-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="bc43a-107">請遵循本文中的指示： [Office 365 Security & 合規性中心。](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="bc43a-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>