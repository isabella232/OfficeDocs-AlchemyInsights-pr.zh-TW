---
title: 限制 SharePoint Online 傳統模式
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551550"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="dedf7-102">限制 SharePoint Online 傳統模式</span><span class="sxs-lookup"><span data-stu-id="dedf7-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="dedf7-103">有些組織還是需要傳統模式體驗。</span><span class="sxs-lookup"><span data-stu-id="dedf7-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="dedf7-104">時沒有計劃来移除的細微層級的傳統模式，不會再可能會限制清單和文件庫的傳統模式整個組織 （承租人）。</span><span class="sxs-lookup"><span data-stu-id="dedf7-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="dedf7-105">系統管理員將有下列選項來管理個別清單和文件庫的傳統模式使用我們提供下列層級的細微退出參數：</span><span class="sxs-lookup"><span data-stu-id="dedf7-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="dedf7-106">網站集合</span><span class="sxs-lookup"><span data-stu-id="dedf7-106">site collection</span></span>
- <span data-ttu-id="dedf7-107">網站</span><span class="sxs-lookup"><span data-stu-id="dedf7-107">site</span></span>
- <span data-ttu-id="dedf7-108">清單</span><span class="sxs-lookup"><span data-stu-id="dedf7-108">list</span></span>
- <span data-ttu-id="dedf7-109">文件庫</span><span class="sxs-lookup"><span data-stu-id="dedf7-109">library</span></span>

<span data-ttu-id="dedf7-110">此外，使用某些功能的清單及不支援的最新的自訂項目將仍會自動切換到傳統模式。</span><span class="sxs-lookup"><span data-stu-id="dedf7-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="dedf7-111">開始 2019 年 4 月 1 日，若要停用租用戶層級的程序退出新式的清單和文件庫將會啟動並繼續執行 2019 5 月 31 日。</span><span class="sxs-lookup"><span data-stu-id="dedf7-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="dedf7-112">由於租用戶選擇不使用傳統模式中的文件庫與清單會自動將移至現代化。</span><span class="sxs-lookup"><span data-stu-id="dedf7-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="dedf7-113">如果您需要傳統模式的詳細資訊，請參閱[以下](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)和 PnP Powershell 指示[此處](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)所描述的選項和工具可用於目前使用傳統模式體驗。</span><span class="sxs-lookup"><span data-stu-id="dedf7-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
