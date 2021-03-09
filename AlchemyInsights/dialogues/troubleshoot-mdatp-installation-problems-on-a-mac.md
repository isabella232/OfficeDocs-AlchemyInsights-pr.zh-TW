---
title: 疑難排解 Mac 上的 MDATP 安裝問題
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568527"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="cf97a-102">疑難排解 Mac 上的 MDATP 安裝問題</span><span class="sxs-lookup"><span data-stu-id="cf97a-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="cf97a-103">若手動安裝失敗，安裝精靈的 [ **摘要** ] 頁面會顯示下列錯誤：</span><span class="sxs-lookup"><span data-stu-id="cf97a-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="cf97a-104">「安裝時發生錯誤。</span><span class="sxs-lookup"><span data-stu-id="cf97a-104">"An error occurred during installation.</span></span> <span data-ttu-id="cf97a-105">安裝程式發生錯誤，導致安裝失敗。</span><span class="sxs-lookup"><span data-stu-id="cf97a-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="cf97a-106">請與軟體製造商聯繫以取得協助。」</span><span class="sxs-lookup"><span data-stu-id="cf97a-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="cf97a-107">在 MDM 部署中，頁面也會顯示一般安裝失敗。</span><span class="sxs-lookup"><span data-stu-id="cf97a-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="cf97a-108">雖然我們沒有向使用者顯示確切的錯誤，我們還是會在 **/Library/Logs/Microsoft/mdatp/install.log** 中保留具有安裝進度的記錄檔。</span><span class="sxs-lookup"><span data-stu-id="cf97a-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="cf97a-109">每個安裝會話都會附加到此記錄檔。</span><span class="sxs-lookup"><span data-stu-id="cf97a-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="cf97a-110">若只要輸出上一個安裝會話，請使用 `sed` 。</span><span class="sxs-lookup"><span data-stu-id="cf97a-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="cf97a-111">若要深入瞭解，請參閱 [疑難排解 Microsoft DEFENDER ATP For Mac 的安裝問題](https://go.microsoft.com/fwlink/?linkid=2144615)。</span><span class="sxs-lookup"><span data-stu-id="cf97a-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
