---
title: 將 SharePoint Online 限制為傳統模式
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
ms.openlocfilehash: 52c63d8909796f8d0d114a46c5255e4073e8c47d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369764"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="d379d-102">將 SharePoint Online 限制為傳統模式</span><span class="sxs-lookup"><span data-stu-id="d379d-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="d379d-103">某些組織仍然需要傳統模式體驗。</span><span class="sxs-lookup"><span data-stu-id="d379d-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="d379d-104">雖然沒有任何計畫在細微層級移除傳統模式, 但是無法再將整個組織 (租使用者) 限制為清單和文件庫的傳統模式。</span><span class="sxs-lookup"><span data-stu-id="d379d-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="d379d-105">系統管理員可以使用下列選項, 以傳統模式管理個別清單和文件庫, 使用在下列層級提供的細微選項:</span><span class="sxs-lookup"><span data-stu-id="d379d-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="d379d-106">網站集合</span><span class="sxs-lookup"><span data-stu-id="d379d-106">site collection</span></span>
- <span data-ttu-id="d379d-107">網站</span><span class="sxs-lookup"><span data-stu-id="d379d-107">site</span></span>
- <span data-ttu-id="d379d-108">清單</span><span class="sxs-lookup"><span data-stu-id="d379d-108">list</span></span>
- <span data-ttu-id="d379d-109">庫</span><span class="sxs-lookup"><span data-stu-id="d379d-109">library</span></span>

<span data-ttu-id="d379d-110">此外, 也會使用目前不支援的某些功能和自訂的清單, 將會自動切換為傳統模式。</span><span class="sxs-lookup"><span data-stu-id="d379d-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="d379d-111">2019年4月1日開始, 停用租使用者層級的程式會退出現代化清單, 而文件庫將會啟動並繼續進行5月 31 2019 日。</span><span class="sxs-lookup"><span data-stu-id="d379d-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="d379d-112">因為租使用者自願登出而成為傳統模式的清單和文件庫, 將會自動移至現代。</span><span class="sxs-lookup"><span data-stu-id="d379d-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="d379d-113">如果您需要傳統模式, 請參閱這裡[](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)的詳細資訊和 PnP [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) Powershell 說明, 以說明您目前可以使用傳統模式體驗的選項和工具。</span><span class="sxs-lookup"><span data-stu-id="d379d-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
