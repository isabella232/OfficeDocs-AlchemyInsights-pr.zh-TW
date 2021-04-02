---
title: 在已加入網域的裝置上將 Microsoft Edge 設定為預設瀏覽器
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426794"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="f4b45-102">在已加入網域的裝置上將 Microsoft Edge 設定為預設瀏覽器</span><span class="sxs-lookup"><span data-stu-id="f4b45-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="f4b45-103">將 Microsoft Edge 設定為預設瀏覽器：</span><span class="sxs-lookup"><span data-stu-id="f4b45-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="f4b45-104">[建立預設關聯設定檔](https://go.microsoft.com/fwlink/?linkid=2132437)，並儲存在本機或網路共用上。</span><span class="sxs-lookup"><span data-stu-id="f4b45-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="f4b45-105">開啟群組原則編輯器，然後前往 [電腦設定 **]**  >  [系統管理範本 **]**  >  [Windows 元件 **]**  >  [檔案總管 **]**。</span><span class="sxs-lookup"><span data-stu-id="f4b45-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="f4b45-106">選取 [設定預設關聯設定檔 **]**。</span><span class="sxs-lookup"><span data-stu-id="f4b45-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="f4b45-107">選取 [原則設定 **]**，然後選取 [已啟用 **]**。</span><span class="sxs-lookup"><span data-stu-id="f4b45-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="f4b45-108">在 [選項 **]** 下，輸入預設關聯設定檔的位置，然後選取 [確定 **]**。</span><span class="sxs-lookup"><span data-stu-id="f4b45-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
