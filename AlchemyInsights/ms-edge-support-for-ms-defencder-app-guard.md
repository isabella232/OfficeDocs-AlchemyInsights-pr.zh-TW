---
title: Microsoft Edge 對 Microsoft Defender 應用程式防護的支援
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576437"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="59059-102">Microsoft Edge 對 Microsoft Defender 應用程式防護的支援</span><span class="sxs-lookup"><span data-stu-id="59059-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="59059-103">針對 Windows 10 和 Microsoft Edge 設計，Application Guard 使用硬體隔離方法，可讓使用者從主機作業系統分開的隔離的 Hyper-V 容器內流覽不可信的網站。</span><span class="sxs-lookup"><span data-stu-id="59059-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="59059-104">企業系統管理員會定義信任的網站、雲端資源和內部網路的清單。</span><span class="sxs-lookup"><span data-stu-id="59059-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="59059-105">當使用者訪問不在清單上的網站時，Microsoft Edge 會在容器中開啟網站。</span><span class="sxs-lookup"><span data-stu-id="59059-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="59059-106">這表示，如果網站會變成惡意的電腦，則主機電腦將保持受保護狀態，而攻擊者將無法取得企業資料。</span><span class="sxs-lookup"><span data-stu-id="59059-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="59059-107">在 Microsoft Edge 版本81中支援在容器中安裝分機，而且可以透過原則加以控制。</span><span class="sxs-lookup"><span data-stu-id="59059-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="59059-108">ExtensionInstallForcelist 原則中所使用的 updateURL 位址，應新增為應用程式防護所使用之網路隔離原則中的非特定資源。</span><span class="sxs-lookup"><span data-stu-id="59059-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="59059-109">如需詳細資訊，請參閱 microsoft [Defender Application Guard 的 Microsoft Edge support](https://go.microsoft.com/fwlink/?linkid=2134229)。</span><span class="sxs-lookup"><span data-stu-id="59059-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
